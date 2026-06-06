# Hardware Setup

## Parts List

- Arduino Uno or compatible Arduino board
- NTC thermistor
- 10 kOhm resistor for the thermistor voltage divider
- Photoresistor
- 10 kOhm resistor for the photoresistor voltage divider
- Two LEDs
- Two current-limiting resistors appropriate for the LEDs
- Hobby servo motor
- Breadboard and jumper wires
- USB cable

## Pin Map

| Arduino pin | Connection |
| --- | --- |
| `A0` | Thermistor voltage-divider output |
| `A1` | Photoresistor voltage-divider output |
| `D5` | LED 2 PWM control |
| `D10` | Servo signal |
| `D11` | LED 1 PWM control |
| `5V` | Sensor-divider and servo supply, where appropriate |
| `GND` | Common ground |

## Wiring Notes

1. Build the thermistor and photoresistor as separate voltage dividers and connect their measured outputs to `A0` and `A1`.
2. Connect each LED through a current-limiting resistor to its PWM pin.
3. Connect the servo signal wire to `D10`.
4. Ensure every component shares a common ground.
5. Use an external regulated supply for the servo if its current draw is too high for the Arduino's 5 V rail. Connect the external supply ground to Arduino ground.

## Safety

Disconnect USB and external power before changing the circuit. Verify LED polarity, resistor values, and servo power requirements before running the app.
