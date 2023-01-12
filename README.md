# Klipper-Expansion-board MINI
![image](https://user-images.githubusercontent.com/122443228/212062985-acc01aeb-f7b0-4b58-837b-ea0c5b65688b.png)

What is this?

Additional PCB for those who use clipper software on mini computers such as thin clients. Such a minicomputer does not have any GPIO ports, on the Internet I found some projects that provide additional GPIOs, but none met my expectations. One of the main advantages of the clipper software is the ability to connect the ADXL345 sensor. For example, a PCB with ADXL345 with a USB converter is available on the Internet, the downside of this board is the lack of other GPIO outputs, and the high price, because for the same price you can do something better. Another interesting project is the Klipper Expander, designed by the user Timmit99, but it does not have an SPI output, so you can not connect ADXL to it. My MINI klipper expansion PCB has the same dimensions as Timmit99 project, so it should be compatible with mounting systems 
available on the Internet

# Klipper-Expansion-board
![image](https://user-images.githubusercontent.com/122443228/212063258-42d9a7e3-1ca9-4f17-8cd1-4b8d3855c9c6.png)

It is a PCB that fulfills the same task as the one above, except that it has even more GPIO outputs, and on board DC-DC converters to power the neopixels. PCB can be used as a second microcontroller for the klipper software, or a separate module with its own program, written e.g. in the Arduino IDE.
