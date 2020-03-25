# BLS01

## ESP8266-01 as mini webserver
A small device that is able to switch a state (relay or LED) with a button on the device, a button on a webpage or with MQTT.
It connects to a MQTT server then:

	- on 0 switches off led (home/BLS01/Bls1in
	- on 1 switches on led
	- on 2 switches the state of the led

It will reconnect to the server if the connection is lost using a blocking
reconnect function.
The current state is stored in EEPROM and restored on bootup
	
This program is part of many different sketch examples from many different sources and is primarily just a learning case.
Nothing fancy with the simple code and Node-RED example that needs to cleaned up, made beter or even shorter.
But for now, it works.

![Diagram](https://github.com/Allday3D/BLS01/blob/master/ESP01_base_bls01sm.jpg)

## Used Hardware
The project is based on the
- ESP8266-01,

placed on a
- ESPBase01. https://www.allday-3d.com/design_espbase01.html

Side components are
- One LED. (or relay)
- One switch.
- 5 volt powersupply.

### Used Libraries
This project uses libraries and code by different authors:

For Arduino IDE:

https://github.com/knolleary/pubsubclient A client library for the Arduino Ethernet Shield that provides support for MQTT.

https://github.com/thomasfredericks/Bounce2 Debouncing library for Arduino and Wiring

https://github.com/tzapu/WiFiManager ESP8266 WiFi Connection manager with web captive portal

## To Do

Webpage!? Try to get that grid under control.

![Web view](https://github.com/Allday3D/GH03/blob/master/web_page_bls01.jpg)

Sketch uses 438100 bytes (87%) of program storage space. Maximum is 499696 bytes.
Global variables use 32648 bytes (39%) of dynamic memory, leaving 49272 bytes for local variables. Maximum is 81920 bytes.
