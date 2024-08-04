# Surveillance Robot Project

## Overview

This project involves creating a surveillance robot using Arduino and ESP32 modules. The robot is designed to navigate autonomously, detect obstacles, and continuously roam while monitoring for emergencies. It features live video streaming and can send emergency notifications if it detects fire or gas leaks.

## Components Used

- **Arduino Uno**: Manages navigation and sensor data.
- **ESP32-CAM**: Provides live video streaming over WiFi.
- **ESP32/ESP8266**: Handles WiFi communication and sends emergency notifications.
- **Ultrasonic Sensors**: Detect obstacles in the front, back, left, and right.
- **DHT11 Temperature Sensor**: Monitors temperature to detect fire.
- **Gas Sensor**: Detects gas leaks.
- **L298N Motor Driver**: Controls the robot's motors.
- **Buzzer/Alarm**: Alerts for emergency situations.

## How It Works

1. **Navigation**:
   - The robot uses ultrasonic sensors to measure distances to obstacles in various directions.
   - Based on these measurements, it navigates around obstacles and continuously roams.

2. **Emergency Detection**:
   - The temperature sensor and gas sensor monitor for potential emergencies.
   - If the temperature exceeds a threshold or gas is detected, the robot sends notifications.

3. **Live Video Streaming**:
   - The ESP32-CAM module streams live video over the internet.
   - Users can access the video feed through a web browser using the provided IP address.

4. **Emergency Notifications**:
   - In case of an emergency (fire or gas leak), the ESP32/ESP8266 module sends a notification message and a photo.
   - Notifications are sent via the IFTTT service to your phone.

## Setup Instructions

1. **Connect the Components**:
   - Connect the ultrasonic sensors, temperature sensor, gas sensor, and motors to the Arduino.
   - Connect the ESP32-CAM and ESP32/ESP8266 modules according to the wiring diagrams.

2. **Upload the Code**:
   - Upload the Arduino code for navigation and sensor handling.
   - Upload the ESP32-CAM code for video streaming.
   - Upload the ESP32/ESP8266 code for sending notifications.

3. **Configure WiFi and IFTTT**:
   - Update the WiFi credentials in the ESP32/ESP8266 code.
   - Set up IFTTT applets for sending notifications and configure the Webhooks.

## Code Files

- `Arduino_Code.ino`: Handles navigation and sensor data.
- `ESP32_CAM_Code.ino`: Manages video streaming.
- `ESP32_Code.ino`: Sends notifications via WiFi.

## Contributions

Feel free to fork this repository, make improvements, and create pull requests. Contributions are welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any questions or suggestions, please reach out to [Chaitanya](chaitanyanagasai143@gmail.com).

