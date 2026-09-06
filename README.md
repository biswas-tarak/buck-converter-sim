# Buck-converter-sim
Buck converter simulation and characterization in PLECS
## Overview

This project models a DC-DC buck converter and investigates its steady-state behavior under different duty cycles. The simulation was used to verify the relationship between PWM duty cycle and output voltage, and to observe inductor current and output voltage ripple.

## Converter Parameters

| Parameter | Value |
|---|---:|
| Input Voltage | 10 V |
| Inductor | 10 mH |
| Output Capacitor | 100 µF |
| Load Resistance | 10 Ω |
| Switching Frequency | 10 kHz |
| Simulation Time | 10 ms |

## Simulation Results

The converter was tested at three different duty cycles.

| Duty Cycle | Average Output Voltage | Output Voltage Ripple (p-p) | Average Inductor Current | Inductor Current Ripple (p-p) |
|---:|---:|---:|---:|---:|
| 25% | ~2.498 V | 22.80 mV | ~0.250 A | 186.48 mA |
| 50% | ~5.003 V | 32.00 mV | ~0.501 A | 250.34 mA |
| 75% | ~7.502 V | 23.49 mV | ~0.752 A | 186.90 mA |

The results show the expected approximately linear relationship between duty cycle and average output voltage for the buck converter.

## Key Concepts Demonstrated

- PWM-based control of a buck converter
- Inductor energy storage and transfer
- Output voltage regulation
- Continuous inductor current
- Output voltage and inductor current ripple
- Effect of duty cycle on converter output

## Tools

- PLECS

## Project Files

`Buck_Converter.plecs` — Complete PLECS simulation model.
