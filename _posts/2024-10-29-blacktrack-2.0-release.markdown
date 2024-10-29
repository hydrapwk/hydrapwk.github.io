---
layout: read
title: "BlackTrack 2.0 Release (Online repo, New tools, etc)"
date: 2024-10-29 19:20 -0500
author: joe
thumbnail: /assets/release/bt-2.0/thumbnail.png
permalink: /blog/:title
description: Today, BlackTrack 2.O has arrived with many updates!, what's new in the 2.O(vanguard) release?, there are several updates that we are trying to implement in this version! such as online trials of the official BlackTrack repo, New tools, Installer support, Desktop changes.
---
Today, BlackTrack 2.O has arrived with many updates!, what's new in the 2.O(vanguard) release?, there are several updates that we are trying to implement in this version! such as online trials of the official BlackTrack repo, New tools, Installer support, Desktop changes.

# Whats new?

- Online repo - [Official Repo](#online-repo)
- New tools - [5 tools added in this release](#new-tools)
- Desktop Changes - [Updates to GRUB themes, Missing icons, login themes](#desktop-changes)
- Installation Support - [Calamares installer](#calamares-installer)
- Page - [Updates to the index, adding blog pages, download page updates](#page-changes)


# Online repo

Finally!, we are trying to create an official repository for BlackTrack (Even though it is still in the experimental stage) and we don't know how long the repository will be running (depending on funding from my parents &#128077; ), but we are very, very happy about this!.

```bash
deb http://repo.rstrike.my.id/ vanguard main
```
Main page about this repo [rstrike.my.id](https://rstrike.my.id)


# New tools

In this release 2.0, we added approximately five new tools to the official BlackTrack repository (tools from the official Debian repository are not counted here).

- [betaflight configurator]() - Cross platform configuration tool for the Betaflight firmware.
- [satdump]() - SatDump is a general purpose satellite data processing software.
- [wall-of-flipper]() - A simple and easy way to find Flipper Zero Devices and Bluetooth Low Energy Based Attacks.
- [radare2]() -  UNIX-like reverse engineering framework and command-line toolset.
- [Fern wifi cracker]() - Wireless security auditing and attack software program written using the Python Programming Language and the Python Qt GUI library.

If you request tools to be added to the BlackTrack repository, please contact the BlackTrack developer, or send the request format in the Telegram community with the format.

NOTE!, make sure the source is still active (still being developed)

```bash
#request
Source: https://git{hub/lab}/username/repo-name
Categories: e.g Forensic
```

# Desktop changes

For this release, we updated and fixed something that was missing, such as the WIFI icon in the previous version (1.0) where the WiFi icon was missing, and we also changed several icons.
and we also updated the login screen and GRUB themes, which can be seen below.
NOTE: We also adding terminal shortcut on panel


### login screen
![BlackTrack lightdm web-greeter](/assets/release/bt-2.0/log-screen.png)

### Icons, folder, panel
![BlackTrack Mate Default Desktop](/assets/release/bt-2.0/desktop.png)

### GRUB
![BlackTrack Grub THeme](/assets/release/bt-2.0/grub-2.0.png)

# Calamares installer

Good news!, we have added calamares installation in this release!, although I'm sure no one uses this distro besides me

![BlackTrack installer calamares](/assets/release/bt-2.0/blacktrack-calamares.png)

# Page changes

In this release, we also changed the design of our official page to make it more attractive? I think, also to adapt to the BlackTrack concept
