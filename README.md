# Meridian · Interactive Gyrocompass

Meridian is the PH 217 browser simulation of a classical pendulous gyrocompass. A 3D model shows how Earth’s rotation, gravity acting on a mass rigidly attached below the tilt pivot, and damping combine to bring the spinning axis toward true north. The simulation tracks both azimuth and tilt using coupled nonlinear equations.

[Open the Netlify demo](https://celebrated-phoenix-b6e1d1.netlify.app/)

## Run locally

Download or clone this repository and open `index.html` in a modern browser. It contains the simulation code, styles and graphics libraries, so it runs offline without installation or a local server.

## Use the simulator

1. Set the rotor’s angular velocity and axial moment of inertia, the pendulous mass and its offset from the tilt pivot, the damping factor, the initial azimuth, and the latitude. Set the mass to **0 kg** to remove pendulous gravity control or clear the **Earth rotation on** checkbox to compare the same setup on a nonrotating Earth.
2. Choose a **Simulation duration** of **1–48 simulated hours**. The default is 12 hours. Each change computes a fresh trajectory.
3. Press **Play** or drag **Explore time** to inspect any point in the run. Playback speed changes how quickly the run is shown.
4. Switch between the azimuth and tilt time plots or the azimuth–tilt portrait. Export the current graph as a PNG or download the trajectory and its parameters as a CSV, sampled every five simulated seconds.

## Model

The solver integrates the heading and tilt equations for an ideal stationary instrument with a symmetric rotor and viscous damping. It uses adaptive Radau IIA integration in the browser. The 3D geometry is schematic and the rotor spin is slowed for display.

## Repository contents

- `index.html` contains the complete website used in the Netlify demo.
- `README.md` describes this release.
- `LIBRARY-CREDITS.txt` and `THREE-LICENSE.txt` contain the notices for the bundled Three.js and Plotly.js libraries.

[AmoghAgrawal1249 on GitHub](https://github.com/AmoghAgrawal1249)
