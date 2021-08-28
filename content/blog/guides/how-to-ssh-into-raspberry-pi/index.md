---
title: How to SSH into Raspberry Pi
date: "2021-01-02"
description: "A full guide to SSH into any raspberry pi during the initial configuration. Enabling SSH on a raspberry pi allows you to connect to it remotely from any device."
thumbnail: ./ssh.jpg
---

## Overview

Learn how to enable ssh on any raspberry pi on a mac with this quick and easy tutorial.

### Benefits to Enabling SSH on Raspberry Pi

* Enabling ssh on a raspberry allows the user to connect without needing a mouse, keyboard or monitor connected.
* Editing and accessing files through ssh is usually quicker on the raspberry pi than the graphical user interface.
* Lastly, ssh access can allow multiple users at once to login to the raspberry pi if needed.

## Load SD Card on Mac

Make sure you already have Raspbian OS installed on the micro SD card you are using. If you need to install Raspbian OS, I have written a full guide for that.

Plug SD card into the Mac that you are using. You should see it visible in "Finder" once its plugged in.

## Open Terminal Application on Mac

Navigate to `Applications` on your Mac. Next open up the `Terminal` application which can usually be found in `Applications > Other > Terminal`

Once the application is open, it should look like this:

## Create SSH File

Enter the following commands into terminal to create the `ssh` file on the SD card.

```
$ cd /Volumes/boot
$ touch ssh
```

## Load SD Card on Raspberry Pi

Lastly go ahead and plugin the SD card into your Raspberry Pi and turn it on.

You should now be able to ssh into the raspberry pi from your Mac with the following command.

```
$ ssh pi@raspberrypi.local
```

You will be prompted for a password, enter the following as the default.
```
raspberry
```
