# Raspberry Pi Weather Station

The code here will generally be a modification of the
Raspberry Pi Foundation Weather Station Code, I am not using the
official Raspberry Pi Weather Station hardware, so I will be
modifying it to suit my own hardware

## wind_direction.py

First up is the wind vane, this uses a Maplin wind vane, more specifically,
this [one](http://www.maplin.co.uk/p/maplin-replacement-wind-direction-sensor-for-n96fyn96gy-n81nf).

This is an analogue sensor and thus needs an Analogue to digital convertor or ADC.
The ADC I am using is an MCP3008, and to make it easy I am using the Rasp.io
[anglogzero](http://rasp.io/analogzero/) board by Alex Eames

This code has been updated to use the MCP3008 with [gpiozero](https://www.raspberrypi.org/blog/gpio-zero-a-friendly-python-api-for-physical-computing/)