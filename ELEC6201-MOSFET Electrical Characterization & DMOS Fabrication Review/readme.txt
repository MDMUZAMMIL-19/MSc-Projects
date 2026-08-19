# MOSFET Electrical Characterization & DMOS Fabrication Review

Module: ELEC6201 — MOSFET Characterization

## Problem

Characterize the electrical behaviour of a commercial 2N7000 N-MOSFET through bench measurement, and connect the measured behaviour to the underlying DMOS fabrication process used to build high-voltage power devices.

## Approach

- Measured fixed resistances via the two-probe method and validated against I-V gradient extraction using an SMU, identifying where parasitic series resistance dominates measurement accuracy at low resistance values.
- Extracted the full family of MOSFET characteristics for the 2N7000: Ids-Vds output curves at fixed Vgs, Ids-Vgs transfer curves, threshold voltage, and Rds(on) across gate-source voltages — cross-checked against the manufacturer datasheet.
- Reviewed the DMOS (Double-Diffused MOS) fabrication process step-by-step (device isolation, gate stack formation, self-aligned source/drain, silicide, FEOL/BEOL) and identified the specific process modifications (dual lateral diffusion, epitaxial drift region, p-body implant) that differentiate DMOS from planar NMOS for power applications.
- Reviewed literature on wide-bandgap (WBG) power devices and single-electron transistor (SET) fabrication as alternative scaling paths beyond conventional CMOS.

## Tools

SMU, HP4145 parameter analyzer, two-probe resistance measurement