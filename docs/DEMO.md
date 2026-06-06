# Demo Guide

## Before the Demo

1. Connect the completed circuit and Arduino.
2. Open `src/ArduinoClimateControl.mlapp` in MATLAB App Designer.
3. Set MATLAB's current folder to a writable demo folder.
4. Run the app and enter the demo password `1234`.

## Suggested Walkthrough

1. Show the live temperature gauge and warm the thermistor gently to demonstrate the reading changing.
2. Switch to **Manual Mode**.
3. Toggle each light independently and adjust the intensity slider.
4. Move the window slider to demonstrate servo positioning.
5. Switch to **Automatic Mode** and cover/uncover the photoresistor to demonstrate responsive lighting.
6. Record temperature for several seconds, stop recording, then open the generated data file from the app to plot it.

## Troubleshooting

| Symptom | Check |
| --- | --- |
| MATLAB cannot connect to Arduino | Confirm the support package is installed and only one board is connected. |
| Temperature is invalid or extreme | Check the `A0` voltage divider and thermistor resistor values. |
| Automatic brightness moves in the wrong direction | Reverse the photoresistor divider orientation or adjust the mapping in the app. |
| Servo jitters or resets the board | Power the servo from a suitable external supply with a common ground. |
| No data file appears | Check MATLAB's current folder and write permissions. |
