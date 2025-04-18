# Microcontroller-Based Fingerprint Authentication System

## Overview
This project implements a secure fingerprint authentication system using a microcontroller (Arduino/ESP32) to control door access. It integrates a fingerprint sensor for biometric verification, an LCD for status display, a servo motor for door control, and LEDs/buzzer for visual/audio feedback. Authorized users unlock the door, while unauthorized access triggers alerts.

## Features
- **Fingerprint Scanning**: R305/FPM10A sensor for biometric input.
- **Access Control**: Servo motor to open/close the door.
- **Visual Feedback**: Green LED (access granted) and Red LED (access denied).
- **Audio Alerts**: Buzzer for unauthorized access.
- **LCD Display**: Real-time status updates (e.g., "Access Granted" or "Place Finger").

## Hardware Requirements
1. **Microcontroller**: Arduino Uno/ESP32.
2. **Fingerprint Sensor**: R305/FPM10A.
3. **LCD**: 16x2 character display.
4. **Servo Motor**: SG90 (for door control).
5. **LEDs**: Green and Red LEDs.
6. **Buzzer**: 5V active/passive buzzer.
7. **Resistors**: 220Ω for LEDs.
8. **Jumper Wires and Breadboard**.

## Circuit Diagram


### Pin Connections
| Component       | Arduino Pin |
|-----------------|-------------|
| Fingerprint TX  | 2 (RX)      |
| Fingerprint RX  | 3 (TX)      |
| LCD RS          | 7           |
| LCD EN          | 8           |
| LCD D4-D7       | 10-13       |
| Servo Signal    | 9           |
| Green LED       | 4           |
| Red LED         | 5           |
| Buzzer          | 6           |

## Software Requirements
1. **Arduino IDE** (v2.0+).
2. **Libraries**:
   - `Adafruit_Fingerprint` (for sensor communication).
   - `Servo.h` (for servo control).
   - `LiquidCrystal.h` (for LCD display).
3. **Drivers**: CH340 (for Arduino Uno) or ESP32 board support.

