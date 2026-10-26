# 3D Chemistry Lab Simulation

An interactive 3D web application that simulates a chemical kinetics laboratory. Users run virtual experiments and use the collected data to determine **reaction orders** and **activation energy**, directly in the browser.

**[Live demo](https://raduexe18.github.io/chemistry-lab-3d-sim/)**

**Award:** 3rd Place at the Student Scientific Communication Sessions (Faculty of Chemical Engineering) and Honorable Mention (Faculty of Automatic Control), Polytechnic University of Bucharest.

## Features

- Interactive 3D laboratory scene rendered with **Three.js** (WebGL).
- Dynamic liquid rendering based on **Constructive Solid Geometry (CSG)**, used for real-time volume calculations.
- Automatic data processing with **linear regression**, with the results plotted as charts.
- Formulas rendered with **MathJax**.

## Tech stack

| Purpose | Library |
|---------|---------|
| Language | TypeScript 5 |
| Build tool / dev server | Vite 5 |
| 3D rendering | Three.js, `three-csg-ts` |
| Regression | `regression` |
| Charts | Chart.js |
| Math formulas | MathJax |

## Getting started

### Prerequisites

- Node.js 18 or newer and npm

### Install and run

```bash
npm install
npm run dev
```

The dev script in `package.json` starts Vite on **port 80**. On Linux and macOS, port 80 needs administrator rights. If you get a permission error, run on another port instead:

```bash
npx vite --port 5173
```

### Production build

```bash
npm run build
npm run preview
```

The build output is written to the `dist/` folder.

## Project structure

```
.
├── index.html        # Entry page
├── public/           # Static assets
├── src/              # TypeScript source code
├── vite.config.js    # Vite configuration
└── .github/workflows # CI configuration
```

<!-- TODO: after checking src/, replace the line above with 4-6 lines naming the real modules (scene setup, liquid/CSG, experiment logic, regression/charts). -->

## Live demo

Try it in your browser, no installation needed: **https://raduexe18.github.io/chemistry-lab-3d-sim/**

<!-- TODO: add 2-3 screenshots or a short GIF of the experiments here. -->


## Project status

University project, created for the Student Scientific Communication Sessions.
