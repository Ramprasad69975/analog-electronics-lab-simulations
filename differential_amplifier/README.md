# Differential Amplifier Simulation (BJT, LTspice)

## Overview

This repository contains a simulation setup and LTspice netlist for a classic **differential amplifier using bipolar junction transistors (BJT)**. The simulation demonstrates basic small-signal differential operation and helps visualize input/output behavior.

## Features

- NPN BJT (e.g., BC107) differential pair  
- Split supply rails (±12V)  
- Sinusoidal input source  
- Easily modifiable parameters  

## LTspice Netlist Example

Below is an example LTspice netlist for your differential amplifier. You can save this as `diffamp.asc` (schematic) or `diffamp.cir` (netlist) in your project:

Differential Amplifier - BJT Version

Models
.model BC107 NPN(IS=1E-14 BF=250 VAF=50 IKF=0.3 ISE=1E-13 NE=1.5 BR=3)

Voltage Sources
VCC VCC 0 12V
VEE VEE 0 -12V

Input sine (on Q1 base)
Vin IN 0 SINE(0 100m 1k)

Circuit
Q1 N1 OUT1 0 BC107
Q2 N2 OUT2 0 BC107

Biasing
R1 IN N1 10k
R2 IN N2 10k

Collector resistors
RC1 OUT1 VCC 1.5k
RC2 OUT2 VCC 1.5k

Tail resistor (for shared emitter configuration)
RE 0 OUT1 1k
RE2 0 OUT2 1k

Output load
RL OUT2 0 100

Simulation Control
.tran 0 10m
.end
