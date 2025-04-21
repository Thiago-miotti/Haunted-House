# 👻 Haunted House - Three.js Project

Welcome to my spooky 3D **Haunted House** project! This scene was created using [Three.js](https://threejs.org/) as part of my learning journey with WebGL. It features dynamic lighting, animated "ghosts", realistic materials, and atmospheric effects such as fog and a sunset skybox.

![Haunted House Preview](./static/Captura%20de%20tela%202025-04-21%20165107.png)

## 🏗️ Features

- **Real-time 3D rendering** using Three.js
- A small haunted house built with walls, a roof, and a detailed door using multiple texture maps (color, AO, normal, metalness, roughness, displacement)
- Procedurally generated **graves** scattered around the house, each with random rotations and positions
- Hand-crafted **bushes** placed near the door
- Custom **textures** applied for floor, walls, roof, bushes, graves, and the door
- **Animated ghosts** circling the house using trigonometric motion and floating effects
- Beautiful **sunset sky** created using `Sky.js` addon
- Realistic **fog** effect using `FogExp2` to enhance the eerie atmosphere
- Real-time **GUI controls** using `lil-gui` for debugging materials (toggle with the `H` key)
- Responsive camera and window resizing support
- **OrbitControls** to freely explore the scene
- Fully configured **shadows** using `PCFShadowMap` and shadow camera settings

## 🖼️ Textures

Textures used in this project include:

- PBR materials for floor, wall, roof, bush, grave, and door
- Texture maps: Color, Normal, AO (Ambient Occlusion), Metalness, Roughness, Height/Displacement
- Textures are repeated and wrapped to tile across surfaces seamlessly

## 👻 Ghost Animation

Each ghost is represented as a `PointLight` with a distinct color and animation path:
- Ghosts float around the house in circular paths
- Their Y-position bounces using sinusoidal functions for a ghostly movement

## 🌌 Environment

- The sky is generated using the `Sky` object from Three.js addons
- Sunset effect is achieved by setting the `sunPosition` and tweaking turbidity, rayleigh scattering, and Mie scattering values
- Exponential fog (`FogExp2`) creates a moody, immersive look

## 🧰 Technologies Used

- [Three.js](https://threejs.org/)
- [OrbitControls](https://threejs.org/docs/#examples/en/controls/OrbitControls)
- [Sky.js](https://threejs.org/examples/#webgl_shaders_sky)
- [lil-gui](https://github.com/georgealways/lil-gui)

## 🎮 Controls

- Move the camera with your mouse (OrbitControls)
- Resize the window to adjust the canvas automatically
- Press **`H`** to toggle the material debug panel (GUI)

## 🚀 Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/threejs-haunted-house.git
   cd threejs-haunted-house
