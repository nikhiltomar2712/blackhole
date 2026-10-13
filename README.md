# Singularity

**Schwarzschild Null-Geodesic Renderer**

An interactive real-time visualization of a Schwarzschild black hole rendered in the browser using WebGL and Three.js.

Live demo: [nikhiltomar2712.github.io/blackhole](https://nikhiltomar2712.github.io/blackhole/)

---

## Features

- **Null geodesic integration** — light rays are traced through the Schwarzschild metric
- **Photon ring** at \(1.5\,r_s\)
- **Black hole shadow** diameter \(\approx 5.2\,r_s\)
- **Innermost Stable Circular Orbit (ISCO)** at \(3\,r_s\)
- **Accretion disk** with relativistic Doppler boosting and gravitational redshift
- **30° disk tilt** for a cinematic near-equatorial view
- Interactive camera:
  - **Drag** → orbit
  - **Scroll / pinch** → approach / retreat
- Bloom post-processing and procedural starfield + nebula background
- Responsive HUD showing observer radius, inclination, and azimuth

---

## Technical Notes

- Built with [Three.js](https://threejs.org/) (r160)
- Custom GLSL ray-marching shader that integrates null geodesics
- EffectComposer + UnrealBloomPass for the glow
- Requires WebGL / GPU acceleration

---

## Controls

| Input              | Action          |
|--------------------|-----------------|
| Drag               | Orbit camera    |
| Scroll / Pinch     | Approach / retreat |
| Auto-orbit         | Starts after a few seconds of inactivity |

---

## License

MIT © Nikhil Tomar
