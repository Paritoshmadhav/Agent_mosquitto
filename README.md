# Agent_mosquitto
# ESP32 MQTT IoT Project – Dual Sensor & Dual LED Control

## Overview
This project uses an **ESP32** and **MQTT protocol** to publish sensor data and receive commands for LED control.  
Two sensors (**LDR** and **Ultrasonic HC-SR04**) send data to the MQTT broker, while two LEDs are controlled remotely through subscribed topics.

---

## Hardware Setup
| Component | Pin | Description |
|------------|-----|-------------|
| LDR Sensor | GPIO 34 | Reads light intensity (analog) |
| Ultrasonic Sensor | TRIG → GPIO 5, ECHO → GPIO 18 | Measures distance (cm) |
| LED1 (Red) | GPIO 23 | Controlled via MQTT (`mqtt-demo/led1`) |
| LED2 (Green) | GPIO 22 | Controlled via MQTT (`mqtt-demo/led2`) |
| Power | 3.3V / 5V | Common VCC |
| GND | - | Common ground |

---

## MQTT Broker
- **Broker:** `test.mosquitto.org`  
- **Port:** `1883`  
- **Client ID:** `mqtt-demo`  
- **Authentication:** None (public test broker)  
- **Protocol:** MQTT v3.1.1  

---


