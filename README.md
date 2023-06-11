- [Components](#components)
  - [ESP 32](#esp-32)
  - [ESP-IDF](#esp-idf)
  - [MPU-6050](#mpu-6050)
- [Quick Start](#quick-start)
  - [Connect](#connect)
  - [Configuration and Flash](#configuration-and-flash)

## Components

* [ESP 32](https://espressif.com/en/products/hardware/esp32/overview) module.
* [ESP-IDF](https://github.com/espressif/esp-idf).
* [MPU-6050](https://www.invensense.com/products/motion-tracking/6-axis/mpu-6050/) module.

### ESP 32

Any ESP 32 module should work.

### ESP-IDF

Configure your PC according to [ESP 32 Documentation](https://docs.espressif.com/projects/esp-idf/en/latest/?badge=latest?badge=latest). Windows, Linux and Mac OS are supported.

### MPU-6050

This example has been tested with a MPU-6050. 

The MPU-6000 should work aswell.

## Quick Start

If you have your components ready, follow this section to [connect](#connect) the components to the ESP 32 module, [flash](#configuration-and-flash) the application to the ESP 32 and monitor the data.

### Connect

The pins used in this project to connect the ESP 32 to the MPU-6050 and MAX30100 are shown in the table below. The pinout can be adjusted in the software.

| Interface | MPU-6050 Pin | ESP 32 PIN|
| :--- | :---: | :---: |
| I2C Serial Clock | SCL | SWCLK|
| I2C Serial Data | SDA | SWDIO|
| Power Supply| 3.3V | VCC | 3V3 |
| Ground | GND | GND | GND |

Notes:

If the sensors are not communicating with the ESP 32, consider adding 10kΩ pull-up resistors to the SCL and SDA lines.
