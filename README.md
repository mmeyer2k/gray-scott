# ⚗️ Gray-Scott Reaction Diffusion

A real-time WebGL simulation of the [Gray-Scott model](https://groups.csail.mit.edu/mac/projects/amorphous/GrayScott/) — a two-chemical reaction-diffusion system that spontaneously generates patterns found in nature: coral, leopard spots, zebrafish stripes, and more.

**[🔗 Live Demo](https://mmeyer2k.github.io/gray-scott/)**

## What is this?

Two chemicals, U and V, diffuse across a 2D grid and react:

```
dU/dt = Du·∇²U  − U·V²  + f·(1−U)
dV/dt = Dv·∇²V  + U·V²  − (f+k)·V
```

Tiny changes in the *feed rate* (f) and *kill rate* (k) produce wildly different patterns. The whole thing runs on the GPU via WebGL.

## Features

- 🎨 8 named presets (Coral, Spots, Stripes, Maze, Worms, Mitosis, Zebra, Chaos)
- 🖌️ Paint new seeds with mouse/touch
- 🎭 6 color palettes
- ⚡ Adjustable simulation speed (1–32 steps/frame)
- 💾 Save as PNG
- 📱 Mobile-friendly

## Tech

Pure HTML + WebGL 1.0. No dependencies, no build step. Float textures via `OES_texture_float`.

## License

MIT
