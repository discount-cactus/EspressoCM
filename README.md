# EspressoCM
Espresso Rev 4 CM, or just Espresso CM, is an STM32- and ESP32-based compute module for high performance networking and automation applications. The board was designed to provide a plethora of capabilities in a small, user-friendly and cheap package. An STM32 and two (not one but two!) ESP32's were chosen for their ease-of-use, clock speed and peripherals to acommodate these requirements. For the beginner or novel hobbyist, the ESP32's can be used - both come with their own dedicated flash memory chip as well as Wi-Fi and Bluetooth connectivity. For the more advanced and tech-savy, the STM32 can be programmed directly for higher-performance control.

Link to EspressoCM's complimentary library: https://github.com/discount-cactus/EspressoCMlib

![Screenshot 2025-04-10](https://github.com/user-attachments/assets/6fa4da34-ec05-48b8-9b83-ecbb4fbdb876)

## Board Statistics
- Dimensions: 84.9mm x 50.2mm
- Layers: 4
- Components: 83
- Mounting Hole Size: M2

## Features
- 1 x STM32F107 (@72MHz)
- 2 x ESP32-S3 (@240MHz)
- 1 x ATtiny85
- 1.5A linear regulator (VIN: 3-20V)
- Automatic power switchover from terminal block `J7` and JST battery connector `J8`
- JST LiPo Battery Connector
- 128Mbit Flash (one per ESP32)
- Dedicated E2B functionality
- On-board current sensing

## Applications
- Smart Homes
- Home networks
- IoT Connectivity
- Home automation
- Sensor monitoring

## Programming
### STM32
- The STM32 is programmed on-board via the pin connector `J5` with an ST-Link V2.
- Verify STM32CubeIDE is up-to-date
- Verify ST-Link V2 is up-to-date
1. Set BOOT0 to HIGH
2. Push reset button
3. Build code
4. Run code
5. Set BOOT0 to LOW
6. Push reset button

### ESP32
- The ESP32's are programmed on-board via the header pins `J3` (for Core 1) and `J4` (for Core 2). Pins are labeled on silkscreen.

### ATtiny85
- The ATtiny85 is programmed off-board.
