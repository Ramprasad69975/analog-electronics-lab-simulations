# IC 741 Based Op-Amp Circuits – LTspice Simulations

*/
---------------------------------------------------------
📘 What is IC 741?
---------------------------------------------------------
- IC 741 is a general-purpose operational amplifier.
- It is an 8-pin dual in-line package (DIP).
- Widely used in analog electronics for:
    → Amplification
    → Filtering
    → Signal conditioning
    → Mathematical operations

🧠 Key Features:
- High gain
- Differential inputs (inverting & non-inverting)
- High input impedance
- Low output impedance

---------------------------------------------------------
🧪 CIRCUITS INCLUDED
---------------------------------------------------------
1. Inverting Amplifier
2. Non-Inverting Amplifier
3. Voltage Follower (Buffer)

---------------------------------------------------------
📁 FILE STRUCTURE (LTspice format)
---------------------------------------------------------
/inverting-amplifier
  |- inverting.asc      // LTspice schematic
  |- inverting amplifier waveform.pdf      // Simulation output

/non-inverting-amplifier
  |- non_inverting.asc
  |- non_inverting amplifier.pdf

/voltage-follower
  |- voltage follower.asc
  |- voltage follower input.pdf
  |- voltage follower output.pdf

---------------------------------------------------------
🔁 1. INVERTING AMPLIFIER
---------------------------------------------------------
→ Vin is connected to the inverting input (-) through resistor Rin
→ Non-inverting input (+) is grounded
→ Feedback resistor Rf connects output back to inverting input

🔧 Formula:
    Vo = - (Rf / Rin) * Vin

⚡ Characteristics:
    - Output is 180° out of phase with input
    - Negative gain
    - High stability and linearity

🛠 Use Case:
    - Audio signal inversion
    - Analog filters

---------------------------------------------------------
➕ 2. NON-INVERTING AMPLIFIER
---------------------------------------------------------
→ Vin is applied to the non-inverting input (+)
→ Feedback from output to inverting input (-) through resistor Rf
→ Another resistor Rin from inverting input to ground

🔧 Formula:
    Vo = (1 + Rf / Rin) * Vin

⚡ Characteristics:
    - Output is in phase with input
    - Positive gain
    - High input impedance

🛠 Use Case:
    - Signal amplification without inversion
    - Sensor signal conditioning

---------------------------------------------------------
🔁 3. VOLTAGE FOLLOWER (BUFFER)
---------------------------------------------------------
→ Vin is connected to the non-inverting input (+)
→ Output is directly connected back to inverting input (-)

🔧 Formula:
    Vo = Vin

⚡ Characteristics:
    - Unity gain (Gain = 1)
    - No phase shift
    - Very high input impedance
    - Very low output impedance

🛠 Use Case:
    - Impedance matching
    - Isolation between circuit stages

---------------------------------------------------------
📦 SIMULATION TOOLS
---------------------------------------------------------
🧰 Software: LTspice XVII or newer
    - Simulation of analog circuits
    - View waveforms (transient and AC analysis)

⚠️ Note:
    - Use opamp2 or Universal OpAmp component in LTspice
    - Configure power supply pins: V+ and V- for correct operation

---------------------------------------------------------
👨‍💻 AUTHOR
---------------------------------------------------------
Ramprasad B
Electrical and Electronics Engineering
SSN College of Engineering

GitHub: [Ramprasad69975]

---------------------------------------------------------
🔖 LICENSE
---------------------------------------------------------
MIT License – Free to use, modify, and distribute with credit.
