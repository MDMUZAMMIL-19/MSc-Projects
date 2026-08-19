# Solar Cell Simulation & Front-Surface Optimization

Module: ELEC3202 — PC1D Solar Cell Simulation Exercise

## Problem

Simulate a crystalline silicon solar cell's dark/illuminated I-V behaviour, characterize its efficiency-limiting parameters, and optimize the front-surface design to close the gap toward the theoretical AL-BSF efficiency limit (~19.5%).

## Approach

- Simulated dark and illuminated I-V curves in PC1D, extracting Isc, Voc, fill factor, and power conversion efficiency (PCE) for a baseline device.
- Studied illumination-intensity and temperature dependence, extracting the diode ideality factor (n ≈ 1.22) and dark saturation current (Io) from ln(-Isc) vs. Voc plots — and quantified how rising temperature narrows the bandgap, raises Io, and depresses Voc/fill factor/PCE.
- Used a ray-tracing tool to simulate front/rear surface texturing (upright pyramids) plus a double-layer anti-reflection coating (SiNx + Al₂O₃ front, SiO₂ + Al rear), comparing absorbance/reflectance/transmittance spectra against an untextured, uncoated baseline.
- Compared external and internal quantum efficiency (EQE/IQE) between textured and untextured cells to isolate how much of the improvement comes from reduced reflection vs. increased optical path length.

## Tools

PC1D, Wafer Ray Tracer

