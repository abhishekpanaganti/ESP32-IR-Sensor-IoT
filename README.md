# ESP32-IR-Sensor-IoT
"ESP32-based IR sensor distance measurement with AWS IoT Core using MQTT"



#DESCRIPTION 

Overview
This project implements an IoT-based IR sensor system using ESP32, which measures distance and transmits the data to AWS IoT Core via MQTT. The system continuously reads data from the IR sensor, processes it, and publishes it to an AWS IoT topic for real-time monitoring. Additionally, it can receive commands from AWS to control actions remotely.



Key Features
1.ESP32-based system for wireless connectivity
2. IR Sensor integration for distance measurement
3. MQTT Protocol for efficient and secure data transmission
4. AWS IoT Core Integration for cloud-based monitoring
5. TLS Encryption for secure data exchange
6. NTP Time Synchronization to ensure timestamp accuracy



#Hardware Requirements

ESP32 Development Board
Sharp GP2Y0A21YK0F IR Distance Sensor
Jumper Wires
Breadboard
USB Cable for Programming
Software Requirements
Arduino IDE
ESP32 Board Support Package
PubSubClient (MQTT Library)
WiFiClientSecure Library
ArduinoJson Library
AWS IoT Core Account



#System Workflow

1.ESP32 connects to WiFi using predefined credentials.
2.NTP synchronization ensures accurate timestamps.
3.The IR sensor reads distance data and converts the analog values.
4.The ESP32 publishes sensor data to AWS IoT Core via MQTT.
5.AWS IoT Core can send commands back to ESP32 for remote control.
6.If ESP32 loses connection, it automatically attempts to reconnect.



#Circuit Diagram

IR Sensor VCC → ESP32 3.3V
IR Sensor GND → ESP32 GND
IR Sensor Signal → ESP32 GPIO34
