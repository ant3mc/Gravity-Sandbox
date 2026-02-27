
# Gravity Sandbox

Interactive unusual gravity simulation with customizable physics, planet properties, and boundaries. Place planets, set initial velocities, and watch them dance under the influence of gravity.

## Features

- **Multiple gravity functions**: Quadratic (r²), Linear (r), Power 3/2 (r^1.5), Exponential variants (e^(√r/4), e^(∛r), e^(⁴√r)).
- **Adjustable parameters**: Gravitational constant, central mass, planet count (1-9), planet radius, max force, max speed, mass multiplier.
- **Boundary types**: Toroidal (wrap around), Bounce off edges, Radius limit (circle).
- **Manual placement mode**: Drag to set position and initial velocity.
- **Load/save configurations**: Load planet states from a text file; save after manual mode.
- **Individual planet settings**: Custom mass and color for each planet.
- **Real-time parameter adjustment**: Use arrow keys (or touch zones) to change gravity constant and central mass during simulation.
- **Dual-language UI**: English / Russian (switchable).
- **Responsive design**: Works on desktop and mobile (touch-optimized).

## How to Play

1. Open the game in a browser.
2. Adjust settings on the main screen:
   - Choose gravity function, number of planets, start mode (random static or manual drag).
   - Set boundary type and collision type.
   - Configure advanced settings via the **Settings** button (planet radius, max force, central mass, etc.).
   - Fine-tune each planet’s mass and color under **Planet Settings**.
3. Click **Start Game**.
   - In **Random Static** mode, planets are placed randomly with zero initial velocity.
   - In **Manual Input** mode, you’ll be prompted to place each planet by dragging on the canvas:
     - Tap/click to set the planet’s position (a circle appears).
     - Drag to draw a vector indicating initial velocity (arrow length = speed).
     - Release to create the planet.
     - After placing all planets, you’ll be asked whether to save the configuration.
4. Watch the simulation! Use arrow keys (or touch zones) to tweak gravity constant and central mass in real time.
5. Double-tap/click the center area or press `Escape` to return to the main menu.

**While in manual placement mode**:

- Use arrow keys to move cursor, `Space`/`Enter` to place, `Escape` to cancel.
- Drag with mouse/finger to set velocity.

## Configuration File Format

When saving or loading a configuration (`.txt` file), the format is:

N F G C M

m1 x1 y1 vx1 vy1

m2 x2 y2 vx2 vy2

...

- `N` : number of planets (1-9)
- `F` : gravity function type (1-6, matching the select options)
- `G` : gravitational constant
- `C` : central mass
- `M` : planet mass multiplier (applied to all masses listed below)
- For each planet: `mass x y vx vy` (mass is the base mass, before multiplier)

## Installation

1. Download the `gravi.html` file from the repository.
2. Open it in any modern web browser (Chrome, Firefox, Edge, Safari).
3. No server or internet connection required after download.

## Development

The game is written in pure HTML, CSS, and JavaScript (ES6) without any external libraries. All physics and UI are self-contained.

To contribute or modify:
- Clone the repository.
- Edit the `gravi.html` file directly.
- Test locally by opening the file in a browser.

## License

Copyright (c) 2026 ant3mc  
This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.  
For the full license text, see the `LICENSE` file or visit [GNU AGPL-3.0](https://www.gnu.org/licenses/agpl-3.0.txt).

*Enjoy the gravity!*


