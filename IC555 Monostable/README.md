# IC 555 Timer – Monostable Mode

The **555 Timer IC** in **monostable mode** generates a **single pulse** of fixed duration in response to a triggering input. It’s a one-shot pulse generator — the output stays LOW by default and goes HIGH only once per trigger.

---

## ⚙️ Working Principle

- Initially, the output is **LOW**
- When a **negative trigger** is applied to Pin 2 (voltage drops below 1/3 Vcc), output becomes **HIGH**
- The external capacitor starts charging through resistor R
- When capacitor voltage reaches **2/3 Vcc**, output returns to **LOW**
- Output duration is **independent of trigger pulse width**

---

## ⏱️ Timing Formula

- **T<sub>PULSE</sub>** = 1.1 × R × C  
  (where R = resistance in ohms, C = capacitance in farads)

---

## 📈 Output Waveform

- A **single positive pulse** of fixed width for every valid trigger
- Pulse width depends on R and C values

---

## 🧪 Applications

- Debouncing mechanical switches  
- Timer delays  
- Frequency counters  
- Missing pulse detectors

---

## 📁 Files Included

- `monostable555.asc` – LTspice schematic  
- `waveform.png` – Simulation result

