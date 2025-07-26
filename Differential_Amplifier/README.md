# Differential Amplifier

## What Is a Differential Amplifier?

A **differential amplifier** is an electronic amplifier that amplifies the difference between two input voltages while rejecting any voltage common to both inputs. It is a foundational building block in analog circuit design and is commonly used in operational amplifiers, instrumentation amplifiers, analog comparators, and various signal-processing applications.

## Key Features

- Amplifies the voltage difference between two input signals
- Rejection of common-mode signals (noise or interference that appears on both inputs)
- Core component in analog integrated circuits

## Modes of Operation

Differential amplifiers can operate in two primary modes:

### 1. Differential Mode
- **Definition:** Both inputs receive signals that are equal in magnitude but opposite in phase.
- **Operation:** The amplifier boosts the voltage difference between the two inputs.
- **Use case:** Accurate amplification of small signal differences (useful for sensor and audio signal processing).

### 2. Common Mode
- **Definition:** Both inputs receive the same signal (equal magnitude, same phase).
- **Operation:** An ideal differential amplifier rejects these signals, outputting zero (or near zero) if both inputs are identical.
- **Use case:** Suppression of noise or interference that appears on both lines (improves noise immunity).

## Practical Parameters

- **Differential Gain (Ad):** Amplification factor for the difference between inputs
- **Common-Mode Rejection Ratio (CMRR):** Indicates the amplifier’s ability to reject common-mode signals; higher is better

## Typical Applications

- Operational amplifiers
- Sensor signal conditioning
- Audio amplifiers
- Data acquisition systems

## Example LTspice Schematic

The basic differential amplifier consists of a matched pair of NPN BJTs with shared emitter connection and collector resistors. See `Differential amplifier.asc` or `Differential amplifier common mode.asc`  in this directory for a working simulation example.

---

For more details, see the included netlist and schematic files. You can experiment with common-mode and differential-mode signals by adjusting input voltages and sources in the LTspice file.

