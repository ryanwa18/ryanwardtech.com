---
title: How to Connect WiFi on Raspberry Pi
date: "2021-01-03"
description: "A full guide to enable WiFi and connect to your home network on a raspberry pi. This guide shows exactly how to add a file to the SD card for a raspberry pi to connect to WiFi."
---

## Overview

In this guide I will show you how to connect your raspberry pi to a WiFi network without connecting a keyboard, mouse, or monitor. In order to connect it to WiFi you will need to add a file to the SD card with [Raspbian OS](https://www.raspbian.org/) installed on it.

## Load SD Card on Computer

First you will need to plug in your micro sd card with [Raspbian OS](https://www.raspbian.org/) installed on it. 

## Create wpa_supplicant.conf File on SD card

Next go ahead and open the SD card on your computer and create a new file in the root directory called `wpa_supplicant.conf`.

## Edit wpa_supplicant.conf with Network Credentials

Open `wpa_supplicant.conf` with a text editor of your choice to change the contents.

Add the following to the `wpa_supplicant.conf` file and change the 'ssid', 'psk' and 'country' to match your own network. If you are in the United States, the country code would be `US` for example.

```
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1
country=<Insert 2 letter ISO 3166-1 country code here>

network={
 ssid="<Name of your wireless LAN>"
 psk="<Password for your wireless LAN>"
}
```

Finally, save the file and unmount your SD card.