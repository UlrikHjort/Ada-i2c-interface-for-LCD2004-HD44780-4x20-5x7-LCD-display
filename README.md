# Ada i2c interface for LCD2004 HD44780 4x20 5x7 LCD display

Ada i2c interface for PCF8574 Remote 8-bit I/O I2C expander to drive a LCD2004 HD44780 4x20 5x7 LCD display
Adaption of the C device I/O system call functions: **open**, **close**, **read**, **write**, **ioctl** and **perror**.
Due to the variadic nature of **ioctl** it have been adapted specific for the i2c interface purpose. 
See **io.ads** and **io.adb** for details.

## Hardware:
* PCF8574 Remote 8-bit I/O I2C expander
* LCD2004 (4 lines) HD44780 4x20 5x7 LCD display
* Raspberry Pi 3 Model B+

## Wiring:
I2c device 1 is used.

| PCFF8574 "Backpack" PIN  |  Raspberry Pi PIN |
| --- | --- |
|GND | GND |
|VCC | +5V |
|SDA | GPIO2 (SDA1) |
|SCL | GPIO3 (SCL1) |


