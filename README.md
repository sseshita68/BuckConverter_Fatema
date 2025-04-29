 /BuckConverter_Fatema/ 
 
Project Overview
This project simulates a Buck Converter (DC-DC Step Down Converter) using MATLAB Simulink (R2024b).

Objective:
To design and simulate an open-loop buck converter that converts a fixed 12V input into a regulated 5V output.

This type of converter is commonly used in:
Motor drive

Mobile charger

Renewable energy systems

Electric vehicle auxiliary power supplies

Battery management systems (BMS)

Industrial automation (PLC and sensor voltage regulation)

✨ Key Features
Input Voltage: 12V DC

Output Voltage: 5V DC

Switching Frequency: 25 kHz

Voltage Ripple: ~20 mV

Current Ripple: ~0.8 A

Open-Loop Control (no feedback controller)

🛠️ Design Specifications

Parameter	Value
Input Voltage (Vin)	12V
Output Voltage (Vout)	5V
Duty Cycle (D)	41.67%
Inductor Value (L)	145.83 µH
Capacitor Value (C)	200 µF
Design Equations Used:
Duty Ratio (D) = Vout / Vin

Inductance (L) = [Vout × (Vin - Vout)] / (ΔI × Fs × Vin)

Capacitance (C) = ΔI / (8 × Fs × ΔVc)

Where:

ΔI = Peak Inductor Current Ripple (~0.8A)

ΔVc = Peak Output Voltage Ripple (~20mV)

Fs = Switching Frequency (25 kHz)

🧰 System Configuration
Components:

Ideal Switch controlled by PWM (Pulse Generator)

Diode

Inductor

Capacitor

Load Resistor

Tools:

Simulink Blocks from Simscape Electrical

Scope to monitor Output Voltage

Solver:

Fixed-Step, ode23tb

📈 Expected Results
Output voltage stabilized at ~5V DC.

Small voltage ripple within 20 mV.

Smooth current flow through the inductor.
