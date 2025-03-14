# Setup and Configuration

This guide will help you get started with your CYD.

## Required Software

1. Arduino IDE
2. ESP32 board support
3. Required libraries:
   - TFT_eSPI
   - XPT2046_Touchscreen
   - LVGL (optional)

## Installation Steps

1. Install Arduino IDE
2. Add ESP32 board support
3. Install required libraries
4. Configure TFT_eSPI
5. Test your setup

## Detailed Instructions

### 1. Install Arduino IDE

Download and install the latest version from [arduino.cc](https://www.arduino.cc/)

### 2. Add ESP32 Board Support

1. Open Arduino IDE
2. Go to File > Preferences
3. Add URL to Additional Board Manager URLs:
   `https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json`
4. Go to Tools > Board > Boards Manager
5. Search for ESP32
6. Install `esp32` by Espressif Systems

### 3. Install Required Libraries

1. Go to Tools > Manage Libraries
2. Install:
   - TFT_eSPI
   - XPT2046_Touchscreen
   - LVGL (if needed)

### 4. Configure TFT_eSPI

1. Locate TFT_eSPI library folder
2. Edit User_Setup.h
3. Configure for ILI9341

### 5. Test Your Setup

1. Load basic example
2. Select correct board
3. Upload and verify

## Troubleshooting

See [TROUBLESHOOTING.md](/TROUBLESHOOTING.md) for common issues and solutions.