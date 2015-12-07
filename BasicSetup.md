Basic Setup
===========

WiFi
----

https://www.raspberrypi.org/documentation/configuration/wireless/wireless-cli.md

sudo vi /etc/wpa_supplicant/wpa_supplicant.conf

  network={
    ssid="The_ESSID"
    psk="Your_wifi_password"
  }

sudo ifdown wlan0
sudo ifup wlan


Enable SSH
----------

http://www.instructables.com/id/Use-ssh-to-talk-with-your-Raspberry-Pi/
sudo raspi-config
advanced options
enable ssh

Update
------

https://www.raspberrypi.org/documentation/raspbian/updating.md
sudo apt-get update
sudo apt-get upgrade
sudo apt-get clean # Free space

Add User
--------

https://www.raspberrypi.org/forums/viewtopic.php?f=91&t=37324

sudo adduser user
sudo adduser user group
# note - dont break sudo file, it is not fun.
sudo usermod -a -G sudo hduser


Breakout board Setup
--------------------

http://thepihut.com/blogs/raspberry-pi-tutorials/27968772-turning-on-an-led-with-your-raspberry-pis-gpio-pins

use 330 Ohm resistor on 3.3v track to orientate the breakout board connector.
