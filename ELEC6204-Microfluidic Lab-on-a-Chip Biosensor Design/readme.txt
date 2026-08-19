# Microfluidic Lab-on-a-Chip Biosensor Design

Module: ELEC6204 — Microfluidics and Lab-on-a-Chip

## Problem

Design and optimize the geometry of a flow-based microfluidic biosensor chamber so that analyte transport (convection + diffusion) reaches the sensor surface efficiently and produces a stable, quantifiable signal.

## Approach

- Built a 3D FEM model in COMSOL solving coupled Navier-Stokes (laminar flow) and convection-diffusion transport equations, with a surface reaction boundary condition modelling analyte adsorption at the sensor.
- Compared static-diffusion-only operation (signal decays as local analyte depletes) against flow-based operation (signal reaches a stable steady state via continuous analyte replenishment).
- Investigated how the rate constant (kads) and diffusion coefficient (D) push the sensor between reaction-limited and diffusion-limited regimes, and explained why diffusion-limited operation is more robust for real-world calibration.
- Optimized chamber geometry by subtracting an ellipsoidal void from the flow channel, forcing streamlines closer to the sensor surface — validated via pressure/velocity field and concentration-profile simulations before and after.
- Computed Reynolds and Péclet numbers to confirm the design operates in a stable, laminar, convection-dominated regime.

## Key results

- Optimized geometry reached a stable steady-state sensor signal within ~50 seconds (vs. continuous decay in the unoptimized/static case)
- Geometric optimization nearly doubled the pressure gradient at the inlet but substantially increased flux to the sensor surface
- Confirmed linear scaling of sensor flux with inlet concentration (Co) across a 1–100 mol/m³ range — validating the sensor as a reliable concentration probe
- Re ≈ 1.14 (laminar), Pe ≫ 1 (convection-dominated) — a predictable, well-characterized flow regime

## Tools

COMSOL Multiphysics (FEM, Navier-Stokes + convection-diffusion)