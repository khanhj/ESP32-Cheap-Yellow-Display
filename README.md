# ESP32-Cheap-Yellow-Display

There is an ESP32 with a built in 320 x 240 2.8" LCD display with a touch screen called the "ESP32-2432S028R", since this doesn't roll of the tongue, I propose it should be renamed the "Cheap Yellow Display" or CYD for short. This display is only about $15 delivered so I think it's really good value.

![image](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display/assets/1562562/76c3d481-2523-4b6f-881c-2e29f9368cd0)

## Features

The CYD has the following features:

- ESP32 (With Wifi and Bluetooth)
- 320 x 240 LCD Display (2.8")
- Touch Screen (Resistive)
- USB for powering and programming
- SD Card Slot, LED and some additional pins broken out

## Code Examples

### The Basics

A collection of examples demonstrating how to use the different features of the CYD, this is a good place to get started. [Check them out here.](/Examples/Basics)

### LVGL Examples

The LVGL example in `/Examples/LVGL9/LVGL_Arduino/LVGL_Arduino.ino` demonstrates a working implementation of LVGL 9.2.2 on the CYD. It includes a demo interface with buttons, toggles, and a slider, all with touch input support.

### Alternative Display Libraries

The basics examples are based on the TFT_eSPI display library, but the CYD also works with other display libraries too. Here is some example code if you prefer to use an alternative Arduino library. [Check them out here.](/Examples/AlternativeLibraries)

## License Info

This project is licensed as MIT as per the [license file](/LICENSE)