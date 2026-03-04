# NeuroLock – Smart Door Security System

HackArena 2026 Project

## Overview

NeuroLock is a multi-factor authentication smart door system using:

• Face Recognition (ESP32-CAM)
• Bluetooth Low Energy (BLE) phone authentication
• Cryptographic challenge-response verification
• Relay-controlled solenoid lock

The system ensures secure access by verifying both biometric and device-based authentication.

## System Components

Hardware:
- ESP32
- ESP32-CAM
- Relay Module
- Solenoid Lock
- LEDs
- Buzzer

Software:
- Flutter Mobile App
- ESP32 Firmware
- BLE Communication
- HMAC-based Authentication

## Authentication Flow

1. ESP32-CAM detects face
2. ESP32 detects authorized phone via BLE
3. ESP32 sends random challenge
4. Flutter app generates secure response
5. ESP32 verifies response
6. Relay activates and door unlocks