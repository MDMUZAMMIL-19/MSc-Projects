# Spectroscopic Characterization of Quantum Dots

Module: ELEC6207 — Quantum Devices and Technology

## Problem

Optically characterize CdSe-core/ZnS-shell quantum dots to extract their bandgap and physical size from measured absorbance spectra, and connect the quantum-confinement physics to real photovoltaic applications (luminescent downshifting).

## Approach

- Built a spectroscopy bench (halogen light source, fiber optics, collimation lenses, spectrometer) and acquired transmittance and reflectance spectra (400–800 nm) for two QD samples (green, orange).
- Corrected raw spectra for dark-current background noise and calculated absorbance via energy conservation (A = 1 − T − R), applying a polynomial fit to isolate the true excitonic peak from measurement noise.
- Extracted bandgap energy via Tauc plot analysis (linear fit to the absorption edge) in MATLAB, cross-validated against the direct photon-energy-at-peak-wavelength method.
- Converted bandgap/peak wavelength to physical QD diameter and size distribution (σD) using an empirical polynomial model and FWHM-based spectral standard deviation.
- Analyzed and diagnosed a systematic measurement artefact (the "refractive glass effect" causing an intensity spike/negative absorbance on sample insertion) and proposed setup improvements (high-NA objective, solid immersion lens, DBR) to improve future SNR.
- Reviewed how QD-based luminescent downshifting (LDS) improves solar cell EQE at UV/blue wavelengths, and surveyed complementary mechanisms (Multiple Exciton Generation, Intermediate Band Solar Cells, Luminescent Solar Concentrators).

## Tools

MATLAB (Tauc plot fitting, absorbance calculation), OceanView spectroscopy software