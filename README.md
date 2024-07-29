# ESP32S Soil Moisture Sensor with LED Indicator

## Description

This Arduino project creates a simple soil moisture monitoring system with visual feedback. It uses a soil moisture sensor to detect the moisture level in the soil and an LED to indicate when the soil is too dry. This setup can be particularly useful for indoor plants or small garden plots where you want an easy way to know when it's time to water your plants.

## Features

- Continuous soil moisture monitoring
- LED indicator for dry soil conditions
- Serial output for detailed moisture readings
- Adjustable moisture threshold

## Hardware Requirements

- ESP32S microcontroller
- Soil moisture sensor (analog)
- LED
- 220-ohm resistor (for the LED)
- Jumper wires
- Breadboard (optional)

## Pin Configuration

- Soil Moisture Sensor: A0
- LED: Digital Pin 13

## Installation

1. Connect the hardware components as shown in the circuit diagram.
2. Install the Arduino IDE on your computer if you haven't already.
3. Clone this repository or download the `.ino` file.
4. Open the `.ino` file in the Arduino IDE.
5. Upload the code to your Arduino board.

## Usage

1. After uploading the code, open the Serial Monitor in the Arduino IDE (Tools > Serial Monitor).
2. Set the baud rate to 115200.
3. Insert the soil moisture sensor into the soil you want to monitor.
4. The LED will light up when the soil moisture falls below the set threshold.
5. Check the Serial Monitor for continuous moisture level readings and status updates.

## Customization

You can adjust the `threshold` value in the code to change the moisture level at which the LED turns on. Lower values indicate drier soil. Experiment with this value to find the right setting for your plants and sensor.

(```cpp
const int threshold = 100; // Adjust this value based on your sensor and soil type)

## Troubleshooting

If the LED doesn't light up when the soil is dry, check your wiring and ensure the threshold value is appropriate for your sensor and soil type.
If you're getting inconsistent readings, make sure the sensor is making good contact with the soil and that there are no short circuits in your wiring.

## Contributing
Contributions to improve the project are welcome. Please feel free to fork the repository and submit pull requests.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
