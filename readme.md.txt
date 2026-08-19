# Piezoresistive Accelerometer Interface Circuit

**Module:** ELEC6203 — Microsensor Technologies

## Problem

Design a complete interface circuit for a Measurement Specialties 3028 piezoresistive accelerometer (4.5 mV/g sensitivity) so that its raw millivolt-level output is conditioned into a usable, low-power sensor signal.

## Approach

- Modelled the sensor as a full-bridge Wheatstone circuit (4 active elements) in NI Multisim, matching the datasheet sensitivity of 4.5 mV/g at ΔR = 0.072 Ω.
- Built a differential amplifier (gain 110) to boost the signal, then evaluated impedance matching vs. bridging between sensor and amplifier — confirming that matched impedance halves the output voltage, so the design uses high input impedance instead.
- Replaced the differential amp with a 3-op-amp instrumentation amplifier for higher CMRR and input impedance, reaching the target sensitivity of 100 ± 5 mV/g.
- Added a 2nd-order Sallen-Key band-pass filter (20–170 Hz, −40 dB/decade roll-off) to reject out-of-band vibration.
- Optimized total current draw by scaling filter resistor/capacitor values (R×10, C÷10) to preserve the RC time constant while cutting current 90%.

## Key results

| Metric | Value |
|---|---|
| Sensitivity (raw sensor) | 4.5 mV/g |
| Sensitivity (after INA) | 100 ± 5 mV/g |
| Filter roll-off | ≈ −35 to −40 dB/decade |
| System current draw (initial) | 135.46 µA |
| System current draw (optimized) | 12.026 µA |

## Tools

NI Multisim (circuit simulation, AC sweep, transient analysis)

## Files

- `report.pdf` — full write-up with all 7 lab questions
- `figures/` — Wheatstone bridge, INA schematic, band-pass filter design, AC sweep plots