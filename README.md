2-Bit Flash ADC Using Subthreshold Technique
📌 Project Overview

This project presents the design, simulation, and analysis of a 2-bit Flash Analog-to-Digital Converter (ADC) implemented using CMOS technology, with a special focus on subthreshold operation to achieve ultra-low power consumption. Flash ADCs are known for their high-speed performance due to parallel comparison, making them suitable for high-frequency and real-time applications.

The complete design is simulated using LTSpice and Microwind, and performance is evaluated across different technology nodes.

🎯 Objectives

Design a 2-bit Flash ADC using CMOS technology

Implement a novel low-power comparator

Reduce power consumption using subthreshold technique

Design and integrate a priority encoder

Compare power and delay across 180 nm, 45 nm, and subthreshold operation

⚙️ Working Principle

A 2-bit Flash ADC uses:

Resistor ladder network to generate reference voltages

Three comparators to compare the analog input against reference levels

Priority encoder to convert comparator (thermometer) outputs into binary form

The conversion occurs in one step, resulting in very low latency.

🧩 System Architecture

The ADC consists of:

Voltage Divider (Resistor Ladder)

Comparator Array (3 Comparators)

Priority Encoder

Digital Output (2-bit)

Input voltage ranges are divided as:

Input Voltage Range	Comparator Output (C1 C2 C3)	Digital Output
0 ≤ Vi ≤ V/4	000	00
V/4 < Vi ≤ V/2	100	01
V/2 < Vi ≤ 3V/4	110	10
3V/4 < Vi ≤ V	111	11
🧪 Tools & Technologies Used

LTSpice – Circuit simulation & waveform analysis

Microwind – CMOS layout and power analysis

CMOS Technology – 180 nm & 45 nm

Subthreshold Design Technique – Ultra-low power operation

🔬 Key Features

Novel low-power CMOS comparator

Priority encoder implemented using CMOS logic

Full ADC realization in Microwind

Power-efficient design using subthreshold operation

Verified using sine and triangular wave inputs

📊 Performance Comparison
Technology	Power Consumption	Delay
180 nm	0.935 mW	1865 ps
45 nm	0.961 µW	3095 ps
Subthreshold	0.950 µW	6070 ps

✔ Significant power reduction is achieved using subthreshold operation, at the cost of increased delay.
