# Discrete Differential Amplifier PCB ⚡

A complete hardware design project featuring a custom discrete operational/differential amplifier built entirely from bipolar junction transistors (BJTs) and passive components. This repository documents the full design lifecycle, from schematic capture and SPICE simulation to PCB routing and 3D visualization.

## Project Overview
The core circuit utilizes a classic differential pair architecture:
* **Input Stage:** NPN Differential Pair (2N3904) for signal comparison.
* **Gain Stage:** PNP Transistor (2N3906) for voltage amplification.
* **Output Stage:** NPN Emitter Follower (2N3904) for current buffering and driving the load.

## Features
* **Analog Circuit Design:** Custom biasing and component selection for stable DC operating points.
* **Pre-Layout Simulation:** Nodal voltage analysis and functional verification before routing.
* **PCB Layout:** Single-layer (bottom copper) trace routing optimized for DIY etching or low-cost manufacturing.
* **3D Visualization:** Rendered hardware layout for physical dimension and clearance checks.

## Tech Stack & Tools
* **EDA Software:** Proteus Design Suite (ISIS Schematic Capture & ARES PCB Layout)
* **Active Components:** 3x 2N3904 (NPN), 1x 2N3906 (PNP)
* **Passive Components:** Through-hole carbon film resistors, 100pF ceramic capacitor.

## Repository Contents
* `Schematic/` - Contains the Proteus simulation file (`.pdsprj` or similar) and schematic PDF.
* `PCB_Layout/` - Contains the 2D copper trace layout and Gerber files for manufacturing.
* `Images/` - Visual documentation including the schematic, 3D rendered board, and raw trace layouts.

## Manufacturing (DIY or Fab)
The PCB is routed specifically to be friendly for home manufacturing (toner transfer method) or standard 1-layer fabrication. 
1. Open the PCB trace image or Gerber files located in the `PCB_Layout` folder.
2. Transfer the layout to a copper-clad board.
3. Etch, drill, and populate with standard TO-92 and axial through-hole components.
