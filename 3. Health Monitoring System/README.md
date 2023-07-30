# IoT Patient Monitor System

This Arduino code implements an IoT-based patient monitor system. It uses various sensors and modules to monitor the patient's heart rate and body temperature. The data is displayed on an LCD screen and sent to an ESP8266 module for wireless transmission to a remote server.

## Installation

- Connect the necessary hardware components according to the circuit diagram.
- Install the required libraries (LiquidCrystal, SoftwareSerial, OneWire, DallasTemperature, and PulseSensorPlayground) in your Arduino IDE.
- Upload the code to your Arduino board using the Arduino IDE.

## Components Used

- Arduino Board/Chip
- LiquidCrystal Library for LCD Display
- SoftwareSerial Library for Serial Communication
- OneWire Library for Temperature Sensor
- DallasTemperature Library for Temperature Sensor
- PulseSensorPlayground Library for Pulse Sensor



## Usage

1. Connect the Arduino board/chip to the necessary components (LCD, temperature sensor, pulse sensor, buzzer, ESP8266 module) following the wiring diagram above.
2. Upload the code to the Arduino board using the Arduino IDE or compatible software.
3. Open the serial monitor to view the heart rate and temperature readings.
4. The LCD will display the heart rate and body temperature readings.
5. The ESP8266 module will transmit the heart rate and temperature data to a remote server.

## Contributing

Contributions to this project are welcome. Feel free to open issues and submit pull requests to help improve the code.

## License

This project is licensed under the [MIT License](LICENSE).
