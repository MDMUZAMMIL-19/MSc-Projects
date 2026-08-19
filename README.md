## MSc Electronics Engineering — Project Portfolio

Mohammad Muzammil Imam — MSc Electronic Engineering, University of Southampton
[LinkedIn](https://linkedin.com/in/mdmuzammil-imam) · mozamilimam@gmail.com

Eight simulation and characterization projects spanning device physics, RF/microsensor circuit design, nanofabrication, and photonics — covering the full stack from TCAD device simulation to circuit-level signal conditioning. Each folder below is self-contained with its own write-up, figures, and (where applicable) simulation files.

| Project | Module | What it does | Key result | Tools |
|---|---|---|---|---|
| [TCAD MOSFET Simulation](./ELEC6256-tcad-mosfet) | ELEC6256 | Silvaco ATHENA/ATLAS device simulation, electrical + physical parameter extraction, and device-scaling optimization | Ion/Ioff improved 1.78×10⁷ → 6.11×10⁷ via coordinated gate-length, oxide, and doping scaling | Silvaco TCAD, HP4145 |
| [MOSFET Electrical Characterization](./ELEC6201-mosfet-characterization) | ELEC6201 | Lab measurement of 2N7000 MOSFET I-V characteristics; DMOS fabrication process review | Extracted **Vth = 1.65 V**, Ron matched to datasheet within measurement precision | SMU, two-probe method |
| [Accelerometer Interface Circuit](./ELEC6203-microsensor-interface) | ELEC6203 | Full sensor signal chain: Wheatstone bridge → instrumentation amplifier → band-pass filter, for a piezoresistive accelerometer | Sensitivity boosted 4.5 mV/g → 100±5 mV/g; current draw optimized 135.46 µA → 12.026 µA | NI Multisim |
| [Solar Cell Simulation & Optimization](./ELEC3202-solar-cell) | ELEC3202 | PC1D simulation of a Si solar cell; surface texturing and DLAR anti-reflective coating design | PCE improved 9% → 15.2% with textured + coated front surface | PC1D, Wafer Ray Tracer |
| [Microfluidic Biosensor Design](./ELEC6204-microfluidic-biosensor) | ELEC6204 | COMSOL FEM simulation of a lab-on-chip flow sensor; convection-diffusion transport and chamber geometry optimization | Geometric optimization (ellipsoidal void) doubled pressure gradient while reaching steady-state sensor response in ~50 s | COMSOL Multiphysics |
| [Nanofabrication & Photolithography](./ELEC6206-nanofabrication) | ELEC6206 | Photolithography simulation: exposure/resist modelling, NA/DOF trade-offs, focus-exposure matrix, and Optical Proximity Correction | Process window EL = 0.742, DOF = 0.691 µm; corrected corner-rounding via OPC serif insertion | Lithography simulation suite |
| [Quantum Dot Optical Characterization](./ELEC6207-qd-characterization) | ELEC6207 | Spectroscopic characterization of CdSe/ZnS core-shell quantum dots; Tauc plot bandgap extraction | Bandgaps of **2.37 eV / 2.09 eV** → particle diameters of 2.47 nm / 4.14 nm | MATLAB, spectrometer |
| [Transistor Laser Review & Simulation](./ELEC6207-transistor-laser) | ELEC6207 | Literature review and device simulation of an InGaAlAs/InP deep-ridge transistor laser | Novel n-InAlAs cladding design achieves current gain > 4.3 at 11.1 mW optical output, solving the classic TL "gain-drop" problem | Crosslight PICS 3D |

## Background

MSc thesis research (separate repo) is in TCAD simulation of Schottky-barrier MoS₂ transistors. These projects were completed as part of the taught modules alongside that work, and together cover device physics (TCAD), RF/analog circuit design, photonics, and nanofabrication process simulation.

## Repository structure

Each project folder follows the same layout:

```
ELEC####-project-name/
├── README.md          # Problem, approach, key result, tools used
├── report.pdf          # Full coursework write-up
└── figures/             # Key plots (I-V curves, TCAD cross-sections, spectra, etc.)
```
