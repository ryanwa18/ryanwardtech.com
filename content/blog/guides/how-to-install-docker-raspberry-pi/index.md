---
title: How to Install Docker on Raspberry Pi
date: "2021-01-04"
description: "A full guide on how to install and use docker community edition on any rasberry pi. Docker on raspberry pi is important for running several different services such as pihole, apache, nextcloud, etc."
---
## Video Tutorial

`youtube: https://www.youtube.com/watch?v=wJ5Ii0uT4Mk&ab_channel=RyanWard`

## Overview

[Docker](https://www.docker.com/why-docker) is an awesome application that lets you run other "micro services" on Raspberry Pi. In this guide I will show you exactly how to install Docker on Raspberry Pi in a few minutes.

## Installation

Installing Docker is similar to installing other packages on your Raspberry Pi. Simply open up "terminal" on your Raspberry Pi or you can login using SSH.

Run the following commands to install Docker.

```
curl -fsSL https://get.docker.com -o get-docker.sh
```

```
sudo sh get-docker.sh
```

## Verify Installation 

To ensure that Docker is running properly on your Raspberry Pi, run the following command.

```
docker ps
```

If Docker was installed correctly, you should see the following appear in your command line. `docker ps` shows the user which Docker containers are currently running on the Raspberry Pi.

```
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES
```