# Interactive Starry Sky Visualization

## Abstract
This project implements an **interactive 3D starfield visualization** in the browser, enhanced with shooting stars, atmospheric effects, and narrative overlays.  
It leverages the **Three.js API (WebGL wrapper)** to render real-time graphics, while standard HTML, CSS, and JavaScript are used for the user interface and introductory animations.  

The project explores the intersection of **artistic expression** and **technical implementation**, simulating a night sky tied to specific geographic coordinates and a chosen date.

## Objectives
1. To employ the **Three.js API** for real-time rendering of a 3D starfield in the browser.
2. To integrate **interactive UI elements** (intro sequence, overlay text, and animated prompts).
3. To simulate **dynamic celestial events**, such as shooting stars, using custom geometry and physics-inspired motion.
4. To combine **narrative storytelling** with immersive web-based visualization.

## Features
- **Introductory overlay** with animated text (typing effect) and particle system.
- **Interactive trigger** (“View the Sky” button) to transition into the 3D environment.
- **3D Starfield rendering** via Three.js:
  - ~5000 stars generated procedurally with random distribution.
  - Continuous slow rotation of the starfield to simulate night sky motion.
- **Shooting stars simulation**:
  - Randomized trajectories, opacity fading, and life cycle management.
- **Contextual narrative overlays**:
  - Center phrase and bottom message tied to specific date and location.
  - Coordinates and time reference included:  
    *Granada (Lat: 37.168461 | Lon: -3.604725), May 1st 2025.*

## Implementation Details
- **HTML/CSS**: Defines the layout, overlay system, and retro-inspired styling.
- **JavaScript**: 
  - Manages animations, user input, and overlay transitions.
  - Implements a typing effect for sequential intro lines.
  - Handles event-driven starfield creation and shooting star lifecycle.
- **Three.js API**:
  - Provides the rendering pipeline (scenes, cameras, geometry, shaders).
  - Wraps low-level **WebGL API** functionality for accessible 3D graphics in the browser.

## Requirements
- A modern web browser supporting WebGL.
- Internet connection to load Three.js via CDN:
  ```html
  <script src="https://cdn.jsdelivr.net/npm/three@0.160.0/build/three.min.js"></script>
