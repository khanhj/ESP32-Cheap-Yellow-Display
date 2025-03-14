# Setup Guide

## Hardware Setup

1. Connect your ESP32 Cheap Yellow Display to your computer via USB
2. Install any required USB drivers for your operating system

## Software Setup

### Arduino IDE

1. Install the Arduino IDE from [arduino.cc](https://www.arduino.cc/en/software)
2. Add ESP32 board support:
   - Open Preferences
   - Add `https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json` to Additional Board URLs
   - Install ESP32 boards from Board Manager
3. Install required libraries:
   - TFT_eSPI
   - XPT2046_Touchscreen

### PlatformIO

1. Install Visual Studio Code
2. Install PlatformIO extension
3. Create a new project:
   - Select ESP32 Dev Module as the board
   - Select Arduino as the framework
4. Add required libraries to `platformio.ini`:
```ini
lib_deps =
    bodmer/TFT_eSPI
    PaulStoffregen/XPT2046_Touchscreen
```

## Display Configuration

1. Configure TFT_eSPI library:
   - Copy `User_Setup.h` from this repository to the TFT_eSPI library folder
   - Or add these defines to your `platformio.ini`:
```ini
build_flags =
    -DUSER_SETUP_LOADED
    -DILI9341_2_DRIVER
    -DTFT_MISO=12
    -DTFT_MOSI=13
    -DTFT_SCLK=14
    -DTFT_CS=15
    -DTFT_DC=2
    -DTFT_RST=-1
    -DTFT_BL=21
```

## Testing

1. Upload the basic example sketch
2. Verify the display shows the test pattern
3. Test touch input functionality

## Troubleshooting

See [TROUBLESHOOTING.md](TROUBLESHOOTING.md) for common issues and solutions.
