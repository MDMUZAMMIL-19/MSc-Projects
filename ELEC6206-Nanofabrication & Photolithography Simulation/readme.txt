# Nanofabrication & Photolithography Simulation

Module: ELEC6206 — Nanofabrication & Microscopy

## Problem

Simulate the full optical lithography process — aerial image formation, resist exposure, development, and proximity effects — to understand how illumination, mask, and process parameters trade off against resolution and process window, then apply Optical Proximity Correction (OPC) to fix a real pattern-fidelity defect.

## Approach

- Simulated resist exposure at varying depth (Z), dose, illumination wavelength (single vs. multi-wavelength), and collimation angle, tracking how each parameter affects resist sidewall taper, resolution, and process robustness.
- Explored dark-field vs. bright-field mask behaviour and periodic mask replication (aerial image self-imaging / Talbot-like effects) as a function of Z-position and NA.
- Quantified the resolution-limiting relationship R = 0.6·λ/NA experimentally by tuning target linewidth down to the sidelobe-interference limit, and separately studied NA vs. depth-of-focus (DOF) trade-offs and defocus sensitivity.
- Modelled substrate reflectivity (Si vs. SiO₂) and standing-wave effects on resist sidewalls, then designed a Bottom Anti-Reflective Coating (BARC) and identified its optimal thickness (~185–195 nm) via a reflectivity minimum.
- Built a full focus-exposure matrix (process window) to extract exposure latitude, DOF, and best dose/focus for a target critical dimension (CD).
- Diagnosed and corrected a real OPC defect: rounding of sharp 90° corners in a projected FET layout, fixed by inserting "serif" correction rectangles at the affected corners.

## Tools

Optical lithography simulation suite (aerial image, resist, and OPC modules)