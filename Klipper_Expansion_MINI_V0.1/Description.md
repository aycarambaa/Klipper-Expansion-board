PCB having the same dimensions as the Klipper expander board designed by the user Timmit99, having more I/0 ports, and an additional SPI output. All the necessary files with a description of the outputs are available for download.

PCB designed to be relatively easy to solder, even by a beginner. The most difficult element to solder is the STM32 microcontroller, but with a little patience, everyone should be able to handle it.

The JP1 jumper should be installed when the LEDs operate with a logic level of 3.3v (most cases), then the resistors R15 and R14 and the transistor Q1 should not be installed.

The BOOT jumper should be installed when programming the microcontroller. The SWDCLK and SWDIO pins for debugging are located in the DEBUG connector. Uploading the clipper software is well presented in this video to which I refer:

https://www.youtube.com/watch?v=zDnlGL_xz0s

LEDs 3.3v and 24v indicate the presence of voltage.

when using 12v fans, you can connect 12v to the 24v input, then you need to change the resistor R17 from 1.2k to 1k

Appropriate voltage should be supplied to the Neopixel IN connector, the same as the LED supply voltage, most often it is 5V, remember about the appropriate current efficiency of the power supply.

Remember about the proper fuse selection, 3A should be more than enough for 2 fans at 12v, and 1.5A at 24v

The SPI interface, which was the reason for the creation of this board, is used to connect the ADXL345, I am aware of the existence of ready-made ADXL345 modules with a USB connector, while the cost of making my board is the same or even lower, if you use the JLCPCB promotion, STM32 can be purchased cheaply on aliexpress, just be careful of fakes. If you have a hot air station, you can desolder the smd resistors and capacitors, in this case the construction should not exceed 10-15$.

For example, air purity sensors can be connected to the I2C connector, which can be useful in the case of abs printing to monitor the level of air pollution.

Thermistor connections - this is the standard wiring copied from the creality motherboard.

Additional GPIO outputs can be used for e.g. remote control of relays, door contact or even a display like mini12864.
