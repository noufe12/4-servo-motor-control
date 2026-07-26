

# 4-Servo Motor Control – Arduino Project
<img width="1100" height="611" alt="Screenshot 1448-02-12 at 6 59 44 PM" src="https://github.com/user-attachments/assets/ba5b1c05-5e62-486b-a240-9115c85d4df6" />


https://www.tinkercad.com/things/0Te0Y6URPXv-grand-sango/editel?returnTo=https%3A%2F%2Fwww.tinkercad.com%2Fdashboard%2Fdesigns%2Fcircuits&sharecode=kzuCTSb8koepBGnge4wuNo0Rov2-tfdRpGk_52xWLi4


## Overview
This project programs 4 servo motors using an Arduino UNO to perform two sequential actions:

1. **Sweep Motion** – All 4 servos rotate back and forth (0°–180°) for exactly **2 seconds**.
2. **Hold Position** – After the 2 seconds, all servos stop and hold steady at **90 degrees**.

## Components Used
- Arduino UNO
- 4 x Servo Motors (e.g., SG90)
- Jumper wires
- Simulated on **Tinkercad Circuits**

## Circuit Connections

| Servo   | Signal Pin | VCC | GND |
|---------|-----------|-----|-----|
| Servo 1 | Pin 3     | 5V  | GND |
| Servo 2 | Pin 5     | 5V  | GND |
| Servo 3 | Pin 6     | 5V  | GND |
| Servo 4 | Pin 9     | 5V  | GND |

## How It Works
The code uses the `millis()` function instead of `delay()` to track elapsed time accurately:
- While elapsed time is **less than 2000 ms**, the servos perform a sweep motion (0° → 180° → 0°).
- Once **2000 ms** have passed, all servos are set to hold at **90°** continuously.



## Simulation
The circuit and code were built and tested using **Tinkercad Circuits**.
