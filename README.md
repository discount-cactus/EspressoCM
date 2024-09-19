# EspressoCM
Espresso Rev 4 CM, or just Espresso CM, is an STM32- and ESP32-based compute module for high performance networking and automation applications. The board was designed to provide a plethora of capabilities in a small, user-friendly and cheap package. An STM32 and two (not one but two!) ESP32's were chosen for their ease-of-use, clock speed and peripherals to acommodate these requirements. For the beginner or novel hobbyist, the ESP32's can be used - both come with their own dedicated flash memory chip and CAN bus port as well as Wi-Fi and Bluetooth connectivity. For the more advanced and tech-savy, the STM32 can be programmed directly for higher-performance control.

Link to EspressoCM's complimentary library: https://github.com/discount-cactus/EspressoCM_arduinolib

<img width="946" alt="espressoCM_3drender" src="https://github.com/user-attachments/assets/b606fc82-9e2f-45a0-9720-430596f09b01">

## Board Statistics
- Dimensions: 99.9mm x 50.2mm
- Layers: 4
- Components: 140
- Mounting Hole Size: M2

## Features
- 1 x STM32H7 (dual-core, @ 480MHz/240MHz)
- 2 x ESP32-S3 (@240MHz)
- 1 x ATtiny85
- 2A capability
- JST LiPo Battery Connector
- 128Mbit Flash (one per ESP32)
- CAN bus port (one per ESP32)
- Dedicated E2B functionality (TBD)
- On-board current sensing
- Power Switch

## Applications
- Smart Homes
- Home networks
- IoT Connectivity
- Home automation
- Sensor monitoring

## Programming
### STM32

*NOTES:*
- *The STM32 is programmed on-board via the JTAG connector `J5`. The connector is shielded and keyed so there is (ideally) only one way to plug in the connector.*

### ESP32

*NOTES:*
- *The ESP32's are programmed on-board via the header pins `J3` (for Core 1) and `J4` (for Core 2). Pins are labeled on silkscreen.*

- Library for using flash chips: https://github.com/PaulStoffregen/SerialFlash
- Library for using CAN bus: https://github.com/coryjfowler/MCP_CAN_lib/tree/master

### ATtiny85

*NOTES:*
- *The ATtiny85 is programmed off-board.*
