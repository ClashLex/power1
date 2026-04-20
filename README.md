# ⚡ ELEMENTAL POWERS & 🌌 SPATIAL PORTALS

A collection of webcam-based hand-tracking AR experiments developed by Exploring through Vibecoding. These projects transform your browser into an interactive canvas, letting you shoot elemental particle effects from your fingertips or manipulate a 3D holographic portal in physical space.

🔴 **[Live Demo 1: Elemental Powers](https://clashlex.github.io/power1/)** <br>
🔴 **[Live Demo 2: 3D Spatial Portal](https://clashlex.github.io/power1/threejs.html)**<br>
🔴 **[Live Demo 3: 3D Spatial Portal](https://clashlex.github.io/power1/V3.html)**

---

## 🛠️ How It Works

Both experiments utilize **MediaPipe Hands** to track your hand joints in real-time via your webcam, mapping your physical movements to digital interactions in the browser.

### 🔴 Demo 1: Elemental Powers (2D Canvas)
Overlays high-performance 2D particle effects, lightning bolts, and glowing auras directly onto your camera feed based on specific gestures.
* **Open hand** → Emit power continuously
* **Pinch (index + thumb)** → Draw persistent energy trails

**Powers (`1`–`6` keys or sidebar buttons)**

| Key | Power | Effect |
|:---:|:---|:---|
| `1` | 🔥❄️ Dual | Fire (left) + Ice (right) |
| `2` | ⚡ Storm | Lightning bolts from fingertips |
| `3` | 🔴🔵 Aura | Red/blue energy clash |
| `4` | 🌀 Plasma | Swirling plasma streams |
| `5` | ✨ Divine | Golden particle glow |
| `6` | 🌑 Void | Dark matter vortex |

**Toggles (right panel or keys)**

| Key | Toggle |
|:---:|:---|
| `s` | 🦴 Skeleton overlay |
| `g` | 💡 Hand glow |
| `t` | 〰️ Particle trails |
| `d` | 🌑 Dark mode (black background) |
| `m` | 🔮 Mirror / flip camera |

---

### 🔴 Demo 2: Spatial Portal (Three.js & WebGL)
Turns your hands into controllers for a floating 3D window. Holding up your fingers spawns a virtual glass plane in the space between them, applying custom GLSL shaders to the reality behind the portal.

* **Two-Hand Gesture:** Hold up both index fingers to spawn the portal between your hands. Move your hands apart or together to dynamically scale the window.
* **One-Hand Pinch:** Pinch your thumb and index finger to create a mini, single-handed portal.

**Active Shaders / Filters**

| Filter | Effect |
|:---|:---|
| **Normal** | Crystal-clear glass passthrough |
| **Noir** | High-contrast cinematic grayscale |
| **Neon Wireframe** | Real-time Sobel edge detection, rendering reality as glowing cyan lines |
| **Risograph** | Retro posterized color banding with magenta tints |

---

## 💻 Tech Stack

* **Hand Tracking:** Google MediaPipe Hands
* **Rendering (Demo 1):** HTML5 `<canvas>` API
* **Rendering (Demo 2):** Three.js (Orthographic Camera, Video Textures) & Custom GLSL Fragment/Vertex Shaders
* **Styling:** CSS3 (Glassmorphism UI, Blur backdrops)

## 🚀 Usage

> **Requires:** A modern browser with WebGL support and webcam access permissions. Chrome or Edge is highly recommended for optimal MediaPipe performance.

To run locally:
1. Clone the repository.
2. Because webcam access is blocked on local `file:///` protocols, you must serve the files using a local web server (e.g., VS Code Live Server, Python `http.server`, or Node `http-server`).
3. Allow camera permissions when prompted.
4. 
