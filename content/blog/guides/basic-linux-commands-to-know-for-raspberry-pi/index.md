---
title: Basic Linux Commands to Know when Using a Raspberry Pi
date: "2021-01-08"
description: "In this post, I am going to share some basic Linux commands that everyone should know when using a Raspberry Pi. This guide for Raspberry Pi and Linux is intended for getting people familiar with the command line."
---

## Overview

In this post, I am going to share some basic Linux commands that everyone should know when using a Raspberry Pi. This guide for Raspberry Pi and Linux is intended for getting people familiar with the command line. Using the command line is really convenient and quick once you get the hang of it.

## Basic Linux Commands

For starters, here are four different commands that will be really useful for navigating the command line on your Raspberry Pi. Just for reference, a "directory" is similar to a "folder" on Windows. A directory is simply a folder that is able to store different files.

Additionally, take note that when entering these commands you won't type the `$`. You will only type what follows the `$`. It is just a symbol to show that you would be executing this command within a terminal or command line.

### Checking the Current Directory Path

This is a really useful command if you want to determine which directory you are currently in.

```
$ pwd
```

This will print the current directory path that you are in. For example if you are in the Pi user home directory, the command would print the following.

```
$ pwd
$ /home/pi
```

### Changing Directory

If you want to navigate to a different directory on the command line, you will need to use the following command.

```
$ cd <directory_name>
```

For example if you want to change directory into the pi user's home directory.
```
$ cd /home/pi
```

Alternatively, the following command will change directory into your own user's home directory.
```
$ cd ~
```

### Looking at the Contents of a Directory

If you want to see what files are in a directory, you can use the following command.

```
$ ls
```

Additionally, if you want to see "hidden" directories and print files in a list, you can use the following command.

```
$ ls -la
```

### Make a New Directory

If you wanted to make a new directory, you would use the following command.

```
$ mkdir <directory_name>
```

For example if you wanted to make a new directory in the pi user's home folder named "Music", you would enter the following.

```
$ mkdir /home/pi/Music
```

### Becoming Root or Superuser

The last command I am going to show you in this guide is how to become the `Root` user. **Note** that you must be very careful when using the root user on Linux because it can do powerful things and potentially break the Raspberry Pi OS.

In order to become the root user on a Raspberry Pi, enter the following command.

```
$ sudo su
```

This will prompt you for a password and it will be the same password you use as the `Pi` user.

## Thanks for Reading

If you found this quick guide for basic Linux commands on Raspberry Pi useful, consider sharing it. Additionally, if you want to see more articles like this be sure to leave a comment down below!