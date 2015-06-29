# SMASolarMQTT

Report generation statistics from SMA photovoltaic inverter over a shared MQTT hub.  Designed for use with emonCMS and emonPi see http://openenergymonitor.org/emon/

Copyright 2013-2015 Stuart Pittaway

GNU GENERAL PUBLIC LICENSE -  Version 2, June 1991

# Installation

Install on Raspberry PI image (low write) emonCMS from https://github.com/emoncms/emoncms/blob/master/readme.md

Fire up a command prompt and install the bluetooth stack

sudo aptitude install bluez python-bluetooth

Plug in a CLASS 1 BLUETOOTH USB adapter to the PI.

Run command

lsusb

should be shown similar to this...

Bus 001 Device 004: ID 0a12:0001 Cambridge Silicon Radio, Ltd Bluetooth Dongle (HCI mode)

Start the bluetooth service

sudo service bluetooth start
sudo service bluetooth status

Run command

hcitool scan

Should find your SMA inverter...

Scanning ...
        00:80:25:1D:AC:53       SMA001d SN: 2120051742 SN2120051742
		
	