# diy_arduino

[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/prussiap/diy_arduino?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

DIY Arduinos Atmega328p:
1. Existing most recent is the V4. I added spacing. I have been considering making the voltage regulator a shield but did not implement.
1a. I would like to replace the LED to be a neopixel: https://github.com/prussiap/fritzing_projects/blob/master/ws812_circuits.fzz but use normal resisotr and caps instead of SMT
1b neopixel DI should be wired to D4
DIY Arduinos ATMEGA 84/85
1. I would like to keep the same form factor but "cut" the bottom pins to be able to create sensor nodes with the attiny 84/85s.

Voltage Regulators:
I'm using 7805 or LD1117V33 (3.3V) 
* 3.3V https://www.sparkfun.com/products/526
* 5V https://www.sparkfun.com/products/107
These usuall take a 33uF or 10uF electrolytic cap between gnd/in and gnd/out

Shields:
Notes: Using V4 of the diy Arduino and any future Attiny framworks I'd like to add shields:
1. L293D shield. There is a sample in the shields folder. I have not confirmed or validated.
- diy_arduino shield_v1_l293d
1a. Reference 
-- http://www.instructables.com/id/GOduino-II-Arduino-L293D-Variable-Speed-Motor-/
-- https://goddess-gate.com/projects/en/arduino/tinyrover (L293D)

2. NRF24l01. Very important shields. I added a 3.3V regulator to account for the 3v on the NRF24 vs the 5v on the arduino. BUT I think we can use an LED or diode
for voltage drops to 3.3V. needs investigation and added documentation.
2a: articles for reference:
-- http://www.madebymarket.com/blog/dev/getting-started-with-nrf24L01-and-arduino.html
-- 
3. IR and proximity sensors:
3a reference: 
-- https://goddess-gate.com/projects/en/arduino/tinyrover (interesting attiny)
-- https://github.com/davidk/TinyMotion (attiny but has connectors).
4. I suggest a shield on top of the other ones for all the connections we are making. 

Connectors I use:
JST-2,3,4 right angled or normal
female/male 2.54 headers 
Anything that is in my V4 schematic I have 50x samples of for the class already.


