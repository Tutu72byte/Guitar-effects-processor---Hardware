Complete hardware development of an embedded music signal processing module (Guitar Effect Pedal) from structural block diagram to circuit schematic,
pcb design and generation of manufacturing files using KiCad. The projects consists of:

1) Library Creation: Created dedicated project libraries (TIE2026.kicad_sym and TIE2026.pretty) containing custom schematic symbols and footprints.

2) Schematic design: The circuit diagram contains a Microcontroller, SPI Flash Memory, ADC/DAC audio processing stages,
   an interactive touchscreen interface and a switching power supply (9V in, 5V and 3.3V converters and regulators and a 2.5V bias).
   Incorporated specific JTAG and power rail test pads for hardware debugging.

3) PCB Topology & Stack-up: Configured a 4-layer board stack-up (1.6mm total thickness)
   featuring controlled trace spacing (0.1mm) and a dedicated internal ground plane split between analog ground (GND_A)
   and digital ground (GND), thus managing a low-noise layout by segregating the analog circuitry onto the analog ground plane linked via the 10m-Ohms shunt R28.

4) Routing for High-Speed Signals & Impedance Control: Implemented single-ended 50 Ohms data lines for the Flash
   memory and 100 Ohms differential lines for the video interface.

5) Manufacturing Output: Generated industry-standard production packages, including extended
   Gerber files, Drill files, a Pick-and-Place component file and a Bill of Materials (BOM).
