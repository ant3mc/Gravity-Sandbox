# Gravity Game (Gravity Sandbox)

An interactive simulation of gravitational interactions between planets with various physics( including unusual) and visualization settings.

## 🚀 Key Features

### 🌌 Gravity Physics Models
- **5 gravitational interaction functions, with different distance functions- f(r) :**
  - Exponential 1: e^(√r / 4)
  - Quadratic (standard Newtonian: r²)
  - Linear (r)
  - Power (r^1.5)
  - Exponential 2: e^(∛r)
- **Computational optimization:** Precomputed tables for exponential functions
- **Customizable parameters:** Gravitational constant, maximum gravitational force

- **2 to 9 planets** simultaneously
- **Individual settings** for each planet:
  - Mass (1000-100000)
  - Color (16 preset colors)
 Many global settings.

### ⚡ Start Modes
1. **Static random placement** - planets generated automatically
2. **Manual input** - interactive planet placement with initial velocity setting

### 🔄 Collision Types
1. **Elastic collisions** - with momentum and energy conservation
2. **Center collision** - teleportation when planet centers get too close
3. **No collisions** - planets pass through each other

### 🗺️ Boundary Conditions
1. **Toroidal boundaries** - exiting one edge = entering from opposite side
2. **Edge bounce** - elastic reflection from screen edges
3. **Radius limit** - automatic teleportation when exiting boundaries

### 🌍 Central Mass
- Configurable mass at system center (0-10 million)

### In manual placement mode:
- **Click/tap and drag** - set position and initial velocity
- **Double tap** - undo last placement
- **Indicator** shows current placement progress

## 💾 Settings Persistence
- Automatic saving of:
  - Planet colors
  - Planet radius
  - Maximum gravitational force
  - Maximum speed
  - Language choice
- Data saved in browser's localStorage

## 📜 License
The program is distributed under the **GNU AGPL-3.0-or-later** license.

## 🔧 Technical Features
- **Pure HTML/CSS/JavaScript** - no build required
- **Canvas-based** rendering
- **Adaptive computation step** based on scene complexity
- **Inactivity timeout** (5 minutes) for resource conservation
- **Fully offline-capable**

Use double-click to return to menu
```
## ⚠️ Known Limitations
- Maximum planet count limited to 9 for performance
- When using exponential functions without precomputed tables: maximum 7 planets
- Not recommended for very old browsers
---
**Author:** ant3mc  
**Version:** 1.0 (2025)  
**License:** GNU AGPL-3.0-or-later

*Gravity Sandbox - free software for exploring physics laws in interactive form.*  
