# Mirroria 3D

An interactive 3D model of Mirroria, built with [three.js](https://threejs.org/) (r186). The whole project is a single self-contained HTML file: every model is generated procedurally in code, and nothing is loaded from external sources.

Current version: **v4.2**

![Mirroria 3D screenshot](docs/screenshot.webp)

## Getting started

- Download `index.html` and open it in a modern browser (Chrome, Edge, Firefox, etc.). No server or build step is needed.
- The browser must support WebGL. The High and Ultra quality presets enable extra post-processing and need a stronger GPU.
- **Logo (optional):** name the official logo image `logo.png` and put it in the same folder as `index.html`: it appears in the top-left corner automatically. The logo is not included in this repository.

## Features

- **Landmarks:** 25 landmarks in five groups: Exterior · Mirror Pyramid, District A · Core, District B · Mirramoon & Gardens, District C · Leisure & Living, and Vera Desert. Selecting a landmark flies the camera to it and opens its card.
- **Time of day:** Day, Dusk (with a sandstorm haze), Night
- **Shell:** Full, Glass (see-through), Cutaway
- **Views:** Overview, Top-down, From Below, Inside City, From Desert, Apex Close-up
- **Toggles:** Exploded view, Auto-rotate, Landmark labels, Animation, Lock inside view
- **Quality:** Smooth (2K shadows), High (4K shadows, ambient occlusion, sun shafts, glass-lattice shadows), Ultra (8K soft shadows, high-sample ambient occlusion, supersampling)
- **Export:** Screenshot, 4K Screenshot, Export GLB

## Controls

| Input | Action |
| --- | --- |
| Left-drag / one finger | Rotate 360° |
| Right-drag / two fingers | Pan |
| Wheel / pinch | Zoom toward the cursor, all the way down to street detail |
| Double-click the model | Make that point the centre of rotation |
| Click a label or the list | Fly to the landmark and show its card |
| W A S D / arrow keys | Move: forward / back along the view, strafe left / right |
| Q / E · hold Shift | Down / up · move faster |
| R / Space | Back to overview / auto-rotate |
| 1 2 3 | Day / dusk storm / night |
| I | Lock / unlock the inside view: zoom, movement and double-click never leave the mirror shell |
| C / F | Cutaway shell / exploded view |
| Z / X | Hide or show the landmark list / control panel |
| L | Hide or show landmark labels |
| H | Immersive mode: hide the whole interface, press again to restore |

## Notes

- Shapes and layout follow official screenshots, the in-game map and patch notes. Details that were never shown are stylised guesses, and the landmark cards say so.
- `index.html` is a build output: three.js and the project code are bundled and minified into a single inline `<script>`.

## Changelog

- **v4.2:** English localisation of the interface, landmark cards and in-scene signs. Sign text now wraps and keeps its proportions, and label widths are measured from the rendered text.
- **v4.1:** First version in this repository, with a Simplified Chinese interface.
