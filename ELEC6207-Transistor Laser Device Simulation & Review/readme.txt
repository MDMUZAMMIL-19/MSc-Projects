# Transistor Laser: Device Simulation & Review

Module: ELEC6207 — Quantum Devices and Technology

## Problem

Review and simulate a Transistor Laser (TL) — a three-port device combining HBT switching speed with semiconductor laser optical output — and address its historically limiting failure mode: current gain collapsing to near zero once the device starts lasing.

## Approach

- Reviewed the motivation for TLs (bypassing RC-delay/interconnect bottlenecks in conventional CMOS) and the device physics of adding Multi-Quantum Wells (MQWs) to an HBT base region to convert recombination current into optical output.
- Simulated a baseline InGaAlAs/InP deep-ridge TL in Crosslight PICS 3D (drift-diffusion + thermionic-emission carrier transport, 4×4 k·p MQW gain modelling with Lorentz broadening), reproducing the known gain-drop failure: 25 mW optical power but a near-zero (9.4×10⁻⁶) common-emitter current gain.
- Diagnosed the root cause as a conduction-band energy barrier trapping electrons in the MQW region, and fixed it by inserting an **n-doped InAlAs layer beneath the MQW**, decoupling the base current path from the emitter-injected electrons feeding the laser.
- Further optimized the design by thinning the p-base layer (to 75 nm) to reduce electron loss to the base contact, and by simulating a **selective-oxidation current-confinement aperture** to funnel carriers away from defective etched sidewalls, cutting the lasing threshold.
- Characterized the trade-off between n-InAlAs doping level, current gain, and PI (power-current) slope efficiency, and varied the confinement aperture width and base-layer thickness to map the full device design space.

## Tools

Crosslight PICS 3D (drift-diffusion, thermionic-emission, k·p band-structure and laser rate-equation solver)