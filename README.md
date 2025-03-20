# D-flipflop

D Flip-Flop Design Using Tristate Buffers in 45nm Technology

This repository contains the design of a D Flip-Flop implemented using tristate buffers in a 45nm CMOS process. The design was created using Cadence Virtuoso, including both schematic and analog layout. The flip-flop is a sequential logic element commonly used in digital circuits for data storage.

Design info
Technology: 45nm CMOS process
Tool: Cadence Virtuoso 
Height: 11 tracks, providing sufficient space for internal routing and ensuring routability for clock and data signals.
  - Designed in adherence to 45nm design rules, with careful attention to matching, parasitic reduction, and layout optimization.
  - Power rails (VDD and VSS) are placed at the top and bottom, with 9 tracks available for internal Metal 1 routing.
  - Successfully cleared DRC and LVS verification, confirming manufacturability and equivalence to the schematic.
  - Positive-edge-triggered D flip-flop.
  - Built using tristate buffers for efficient implementation.

Files in This Repository
- `DFFF_schematic.png`: Schematic of the D flip-flop, showing the transistor-level design with tristate buffers.
- `DFFF_layout.gds`: GDSII file of the analog layout, exportable to Cadence Virtuoso or other EDA tools for viewing.
- `DFFF_layout_screenshot.png`: Screenshot of the layout view in Cadence Virtuoso
- `simulation_results.pdf`: Simulation waveforms showing the functionality of the D flip-flop.

How to Use
1. Schematic and Layout Viewing: The schematic can be viewed directly as an image (`DFFF_schematic.png`).
  To view the layout, import the `DFFF_layout.gds` file into an EDA tool like Cadence Virtuoso. Use the 45nm process design kit (PDK) to ensure compatibility.
2. Simulation: The design can be simulated in Cadence Virtuoso using the appropriate 45nm PDK. Set up a testbench with a clock (CLK), data input (D), and monitor the output "Q"
3. Modification: The GDSII file can be imported and modified in Virtuoso for further optimization or integration into a larger design.

## Design Notes
- The D flip-flop uses a master-slave configuration with tristate buffers to reduce the number of transistors while maintaining functionality.
- The layout is DRC-clean and LVS-verified for the 45nm process.
- Transistor sizing was chosen to balance speed, power, and area, but further optimization may be possible depending on the target application.


Acknowledgments
Designed as part of a VLSI design project using Cadence Virtuoso.


