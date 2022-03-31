# MEMS(Material Electronic Management System) is an extension of a previous project: [Microcomputers Project](https://github.com/levkonikitin/microcomputersproject).
The device is still based on the ATmega328p featured in the Arduino Uno development board.
This version features a few code simplifications and is built using PlatformIO's development platform.
The most major features added are the PID control scheme for the heating element and a reduction in size for the OLED library by
removing unnecessary character definitions. 

## Current Features:

- NTC 100k temperature sensor.
- Mosfet controlled Fan and Heating element.
- 128x64 Monochrome OLED over I2C.
- Simple Button Based Interface:
	- Start Heating
	- Stop Heating
	- Temp up
	- Temp down

## Current Issues:
- Temperature Sensor Readings Become inaccurate at >60c.
 	The most likely causes are either temperature sensor quality impacting an improper variance in the resistance 
	or too much resistance on the voltage devider caused by either heat changing the resistance on the 10k Ohm resistor
	or parasitic resistance caused by the breadboard and the wiring itself.
	
## Imporatant:
This project is provided as is under no warranty 
