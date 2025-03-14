# Pin Information

This page contains information about what pins are used where on the CYD, and what ones are free to use.

## Display Pins

The display uses the following pins:

- MOSI: GPIO 13
- MISO: GPIO 12 (not used)
- CLK: GPIO 14
- CS: GPIO 15
- DC: GPIO 2
- RST: GPIO 4
- BL: GPIO 21

## Touch Screen Pins

The touch screen uses the following pins:

- MOSI: GPIO 32
- MISO: GPIO 39
- CLK: GPIO 25
- CS: GPIO 33
- IRQ: GPIO 36

## SD Card Pins

The SD card uses the following pins:

- MOSI: GPIO 13 (shared with display)
- MISO: GPIO 12
- CLK: GPIO 14 (shared with display)
- CS: GPIO 5

## Free Pins

The following pins are free to use:

- GPIO 16
- GPIO 17
- GPIO 18
- GPIO 19
- GPIO 22
- GPIO 23
- GPIO 26
- GPIO 27
- GPIO 34
- GPIO 35

Note: Some pins have special functions or limitations:

- GPIO 34-39 are input only
- GPIO 6-11 are used by the internal flash and are not available
- Some pins may have pull-up or pull-down resistors

## Power Pins

- 5V: Available on expansion header
- 3.3V: Available on expansion header
- GND: Available on expansion header

## Special Function Pins

- BOOT: GPIO 0
- EN/RST: Connected to reset circuit

## Notes

1. Always verify pin functionality in your specific use case
2. Some pins may have different behavior during boot
3. Check the ESP32 datasheet for detailed pin information
4. Some pins may affect the boot process if pulled high or low

## Example Usage

Check the [Basic GPIO](/Examples/Basics/GPIO) example for how to use the free pins.