# arduino-climate-control-gui

MatLab App Designer + Arduino Smart Climate Control 🌡️

By: Jake Trac


## Features
- Password-protected start (4-digit code)
- Live gauges for temperature and brightness
- Servo window control (slider: open/close)
- Two modes:
  - **Manual Mode:** user controls window, LEDs, and **light intensity**
  - **Automatic Mode:** system adjusts window/lighting based on the light control slider
- Optional temperature logging to a **timestamped file**
- Load and plot saved temperature data in a separate figure

## Hardware Used
- Arduino Uno
- NTC thermistor + 10kΩ resistor
- Photoresistor (LDR) + 10kΩ resistor
- 2× yellow LEDs + 2× 200Ω resistors
- Servo motor
- Breadboard + jumper wires

## Software / Requirements
- MATLAB (App Designer)
- Arduino support package for MATLAB (and required libraries)

## How to Run
1. Wire the circuit (thermistor + LDR + LEDs + servo) to the Arduino Uno.
2. Connect the Arduino to your computer via USB.
3. Open the `.mlapp` file in MATLAB App Designer.
4. Click **Run**.
5. Enter the password, choose Manual/Automatic mode, and use the controls.
