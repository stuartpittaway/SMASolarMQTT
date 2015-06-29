sudo aptitude install bluez python-bluetooth

lsusb
Bus 001 Device 004: ID 0a12:0001 Cambridge Silicon Radio, Ltd Bluetooth Dongle (HCI mode)

hcitool dev
Devices:
        hci0    00:09:DD:50:0B:A3

sudo service bluetooth start
sudo service bluetooth status

hcitool scan
Scanning ...
        00:80:25:1D:AC:53       SMA001d SN: 2120051742 SN2120051742

