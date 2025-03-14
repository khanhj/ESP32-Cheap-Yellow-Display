# Pin Configuration

This document details the pin configuration for the ESP32 Cheap Yellow Display (CYD).

## Display Pins

| Pin | Function | Notes |
|-----|-----------|-------|
| 12 | MISO | SPI Data In |
| 13 | MOSI | SPI Data Out |
| 14 | SCK | SPI Clock |
| 15 | CS | Chip Select |
| 2 | DC | Data/Command |
| -1 | RST | Reset (not used) |
| 21 | BL | Backlight |

## Touch Screen Pins

| Pin | Function | Notes |
|-----|-----------|-------|
| 36 | IRQ | Interrupt |
| 32 | MOSI | SPI Data Out |
| 39 | MISO | SPI Data In |
| 25 | SCK | SPI Clock |
| 33 | CS | Chip Select |

## SD Card Pins

| Pin | Function | Notes |
|-----|-----------|-------|
| 18 | SCK | SPI Clock |
| 19 | MISO | SPI Data In |
| 23 | MOSI | SPI Data Out |
| 5 | CS | Chip Select |

## Available GPIO Pins

The following pins are available for general use:

| Pin | Notes |
|-----|--------|
| 0 | Boot button |
| 1 | TX |
| 3 | RX |
| 4 | Available |
| 16 | Available |
| 17 | Available |
| 22 | Available |
| 26 | Available |
| 27 | Available |
| 34 | Input only |
| 35 | Input only |

## Notes

- All pins marked as "Available" can be used as either inputs or outputs
- Pins 34 and 35 can only be used as inputs
- The boot button (GPIO0) can be used as an input, but it's recommended to leave it for programming
- TX and RX pins are used for programming and debugging, but can be used for other purposes if needed

## Configuration

The pin configuration is set in the TFT_eSPI library's User_Setup.h file. The following defines are used:

```cpp
#define TFT_MISO 12
#define TFT_MOSI 13
#define TFT_SCLK 14
#define TFT_CS   15
#define TFT_DC    2
#define TFT_RST  -1
#define TFT_BL   21
```

For the touch screen:

```cpp
#define TOUCH_CS 33
#define TOUCH_IRQ 36
```

For the SD card:

```cpp
#define SD_SCK  18
#define SD_MISO 19
#define SD_MOSI 23
#define SD_CS    5
```
