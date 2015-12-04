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
