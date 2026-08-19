# TCAD MOSFET Simulation & Scaling Study

Module: ELEC6256 — MOSFET Simulation Exercise

## Problem

Extract electrical and physical parameters of a simulated MOSFET in Silvaco TCAD, benchmark them against analytical hand calculations, and then use device scaling to improve performance metrics (Ion/Ioff, leakage, subthreshold swing) toward an ITRS-roadmap-informed target.

## Approach

- Built and simulated an NMOS device in Silvaco ATHENA (process) + ATLAS (device), extracting Ion, Ioff, Vth, and subthreshold swing from transfer characteristics using the HP4145 analyzer tool in TonyPlot.
- Extracted physical parameters (gate oxide thickness, body/gate doping, gate length) directly from the ATHENA doping profile using cutline and ruler tools.
- Derived the same electrical parameters analytically (flat-band voltage, threshold voltage, subthreshold swing, saturation/subthreshold current) from first-principles MOSFET equations and compared against the simulated values — reconciling the gap via Silvaco's use of real mesh/doping physics vs. idealized long-channel formulas.
- Plotted the electronic band structure (conduction band, valence band, Fermi level) at the Si-SiO₂-polysilicon interface, and separately swept flat-band voltage against gate workfunction to confirm the ΦMS relationship.
- Ran a device-scaling study: swept gate length down to identify the leakage-current cliff, then iteratively tuned P-well boron implant dose, gate oxide growth time/temperature, Vth-adjust implant, and S/D dopant doses to jointly minimize leakage and maximize Ion while holding Vth and subthreshold swing in a sane range.

## Tools

Silvaco ATHENA/ATLAS, TonyPlot, HP4145 parameter analyzer