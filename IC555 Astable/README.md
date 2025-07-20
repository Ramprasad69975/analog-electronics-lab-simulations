# IC 555 Timer – Astable Mode

The **555 Timer IC** is a popular and versatile component used in timing and oscillator circuits. In **astable mode**, it operates as a free-running multivibrator, continuously switching between HIGH and LOW without external triggering.

---

## 🔧 Working Principle

- The capacitor **charges** through resistors R1 and R2 → **Output = HIGH**  
- When the capacitor voltage reaches **2/3 Vcc**, output switches to **LOW**  
- The capacitor **discharges** through R2  
- When it drops to **1/3 Vcc**, output goes HIGH again — cycle repeats

---

## 🧮 Timing Formulas

- **T<sub>HIGH</sub>** = 0.693 × (R1 + R2) × C  
- **T<sub>LOW</sub>** = 0.693 × R2 × C  
- **Frequency (f)** = 1 / (T<sub>HIGH</sub> + T<sub>LOW</sub>)

---

## 📈 Output Waveform

- A **square wave** with unequal HIGH and LOW durations  
- Duty cycle depends on values of R1, R2, and C

---

## 🧪 Applications

- LED blinkers  
- Tone generators  
- Clock pulses for digital ICs  
- Pulse Width Modulation (PWM)

---

## 📁 Files Included

- `astable555.asc` – LTspice schematic  
- `waveform.png` – Simulation result
