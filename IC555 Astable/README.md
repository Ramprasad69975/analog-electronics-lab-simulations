IC 555 Timer – Astable Mode
The 555 timer in astable mode functions as a free-running oscillator, generating a continuous square wave without external triggering.

Working Principle:
Capacitor charges through R1 and R2 → Output HIGH.

When voltage reaches 2/3 Vcc, output goes LOW.

Capacitor discharges through R2 → Output remains LOW.

At 1/3 Vcc, cycle repeats.

Key Formulas:
T_HIGH = 0.693 × (R1 + R2) × C

T_LOW = 0.693 × R2 × C

Frequency = 1 / (T_HIGH + T_LOW)

Applications:
LED blinkers

Clock generators

Tone generators
