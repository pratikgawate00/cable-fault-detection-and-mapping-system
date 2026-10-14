# Smart Underground Cable Fault Detection System: Digital Twin

An interactive browser simulation of our Arduino Uno based underground cable fault detector.
Selected in the **top 50 of the AIoT Challenge 2026**.

**Live demo:** https://YOUR-USERNAME.github.io/cable-fault-twin/

## What you can do

- Close a fault switch at 2, 4, 6 or 8 km on the Red, Yellow or Blue line
- Watch the relays scan each line, the Arduino read A0 and the 16×2 LCD update
- See the IoT dashboard and alerts (online and offline bridge)
- Run the **insulation ageing** demo: the AI layer warns before the cable fully shorts, while fixed thresholds react late

## How the hardware works

| Part | Role |
|---|---|
| Arduino Uno | Scans the lines and reads the voltage on A0 |
| ULN2003 + 3 relays | Connect one line at a time (pins 8, 9, 10) |
| 100 Ω resistors | Cable model, one resistor = 2 km |
| R17 (1 kΩ) | Voltage divider with the cable: V(A0) = 5 V × R / (1 kΩ + R) |
| 16×2 LCD, LEDs, buzzer | Show the fault distance, the line under test, and alarm |

## Team: Group 02, Dept. of ECE, MIT-ADT University, Pune

Aadi Gargote · Pratik Gawate · Atharv Dhaygude · Harshal Kolpkar
