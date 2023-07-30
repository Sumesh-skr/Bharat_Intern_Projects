IoT-Based Air Pollution Monitoring System

  - Hardware Components
    - Arduino Uno (ATMega2560) board
    - ESP8266 WiFi module (ESP-01)
    - MQ135 gas sensor
    - MQ7 gas sensor
    - Buzzer
    - Fan
    - LEDs (green and red)
    - LCD (16x2)
    - Breadboard and jumper wires
  - Software Components
    - Arduino IDE
    - ThingSpeak cloud platform
    - ThingSpeak Arduino library
  - Code Structure
    - Air Pollution Monitoring System Code
      - Initializes libraries and variables
      - Sets up serial communication
      - Connects to WiFi network
      - Reads data from gas sensors
      - Displays data on LCD
      - Controls indicators based on pollution levels
      - Sends data to ThingSpeak server
    - ThingSpeak Data Upload Code
      - Imports required libraries
      - Sets up WiFi network details
      - Defines ThingSpeak channel and API key
      - Establishes WiFi connection and ThingSpeak client
      - Uploads data from serial port to ThingSpeak
      - Parses received data and displays it
      - Sets ThingSpeak fields and uploads data
      - Implements delay before next upload
  - Setup Instructions
    - Install Arduino IDE and drivers
    - Connect hardware components
    - Open and modify code for network and ThingSpeak details
    - Upload code to Arduino Uno
    - Verify serial monitor for readings and system status
    - Visit ThingSpeak website for data visualization
  - Conclusion
    - Describes the creation of an IoT-based air pollution monitoring system
    - Summarizes the hardware, software, and code structure
    - Provides setup instructions for running the system

This project implements an IoT-based air pollution monitoring system using Arduino and ESP8266 WiFi modules. The system measures the air quality using MQ135 and MQ7 gas sensors and sends the data to the ThingSpeak cloud server for visualization and analysis. It also controls various indicators like LEDs, a buzzer, and a fan based on the pollution levels.

Hardware Components
Arduino Uno (ATMega2560) board
ESP8266 WiFi module (ESP-01)
MQ135 gas sensor
MQ7 gas sensor
Buzzer
Fan
LEDs (green and red)
LCD (16x2)
Breadboard and jumper wires
Software Components
Arduino IDE
ThingSpeak cloud platform
ThingSpeak Arduino library
Code Structure
The project consists of two Arduino programs: one for the air pollution monitoring system and the other for uploading data to the ThingSpeak cloud server.

Air Pollution Monitoring System Code
The air_pollution_monitoring_system.ino code performs the following tasks:

Initializes the required libraries and defines the necessary variables and pin configurations.
Sets up the serial communication with the PC and the ESP8266 module.
Connects to a WiFi network using the ESP8266 module.
Reads data from the MQ135 and MQ7 gas sensors and calculates the pollution levels in parts per million (ppm).
Displays the pollution levels on an LCD screen.
Controls the buzzer, fan, and LEDs based on the pollution levels.
Sends the pollution level data to the ThingSpeak cloud server via the ESP8266 module.
ThingSpeak Data Upload Code
The thingSpeak_data_upload.ino code handles the data upload to the ThingSpeak cloud server. It performs the following tasks:

Imports the required libraries for WiFi communication and ThingSpeak integration.
Sets up the WiFi network details (SSID and password).
Defines the ThingSpeak channel ID, field numbers, and write API key.
Establishes the WiFi connection and initializes the ThingSpeak client.
Implements a loop that continuously uploads data from the serial port to the ThingSpeak server.
Parses the received data and shows it on the serial monitor.
Sets the ThingSpeak fields with the parsed values and uploads them to the specified channel.
Waits for a delay before making the next upload.
Setup Instructions
Install the Arduino IDE on your computer and set it up with the necessary drivers for the Arduino board.
Connect the hardware components as per the pin configurations mentioned in the code.
Open the air_pollution_monitoring_system.ino code in the Arduino IDE.
Modify the code to match your WiFi network details and ThingSpeak channel information.
Upload the code to the Arduino Uno board.
Open the serial monitor to view the pollution level readings and system status.
Open the thingSpeak_data_upload.ino code in the Arduino IDE.
Modify the code to match your WiFi network details and ThingSpeak channel information.
Upload the code to the Arduino Uno board.
Verify the serial monitor to ensure that data is being uploaded to ThingSpeak successfully.
Visit the ThingSpeak website and log in to view and analyze the air pollution data on the dashboard.
Conclusion
By following the provided instructions and running the Arduino programs, you can create an IoT-based air pollution monitoring system. The system measures the pollution levels using gas sensors, displays the readings on an LCD, and sends the data to the ThingSpeak cloud server for remote monitoring and analysis. With this system, you can gain insights into air quality and take necessary actions to improve the environment.




