---
layout: read
title: "BlackTrack 3.0 Batik Release (Tools, WM support, Update cycle)"
date: 2025-01-21 05:17:00 +0700
author: joe
thumbnail: /assets/release/bt-3.0/thumbnail.png
permalink: /blog/:title
description: Today, BlackTrack released the latest version (3.0) with the codename 'BATIK' (Batik is a pictorial cloth made by dyeing cloth using wax. Batik is an Indonesian cultural heritage that has been recognized worldwide.)
---

Today, BlackTrack released the latest version (3.0) with the codename 'BATIK' (Batik is a pictorial cloth made by dyeing cloth using wax. Batik is an Indonesian cultural heritage that has been recognized worldwide.)


```
# default user is 'blacktrack' and password is 'live' (remove quote)
```

# Whats New?

- New tools - [2 tools added in this release](#new-tools)
- Wm support - [blacktrack adding dwm support](#dwm)
- Update cycle - [BlackTrack update cycle anouncment](#update)

# New tools

In this release 3.0 We didn't add a lot of new tools but we hope this will usefull

- [PE-bear](https://github.com/hasherezade/pe-bear) - Portable Executable reversing tool with a friendly GUI
- [linpeas/PEASS-ng](https://github.com/peass-ng/PEASS-ng/) -  PEASS - Privilege Escalation Awesome Scripts SUITE (with colors)


# DWM

in this release we're using DWM as default GUI, Why? that's because WM like DWM doesnt need a big resource also by using WM(in this case DWM) we can save more space.
However some people may need to adapt to WM

BlackTrack DWM keyboard

| Key | Exec    | Mode    |
| :---:   | :---: | :---: |
| Win+f | Float Layout   | - |
| Win+t | Tile Layout   | - |
| Win+m | Monocle layout   | - |
| Win+Shift+Enter | Spawn terminal   | Float/Title/Monocle |
| Win+j | previous window   | Float/Tile/Monocle |
| Win+k | Next window   | Float/Tile/Monocle |
| Win+-/+ | Increase(+)/Decrease(-) gaps | Tile |
| Win+left/right/up/down | Move window | Float |
| Win+Shift+down | Increase window height | Float |
| Win+Shift+up | Decrease window height | Float |
| Win+Shift+right | Increase window width | Float |
| Win+Shift+left | Decrease window width | Float |
| Win+space | Menu   | Float/tile/monocle |

Maybe some time WM will bug, so you need restart display manager with

```
sudo service lxdm restart # This because were using lxdm as display manager
```

and may if you installing blacktrack WM on VM (Virtual Machine), maybe you need set screen resolution using xrandr

```
# Win+Shift+enter to spawn terminal

# inside terminal you need type

blacktrack@blacktrack:~$ xrandr -s 1920x1080 # This will Make WM change screensize to 1920x1080
```



# Update

Maybe someone is asking questions about the BlackTrack update cycle, including us.
However, at this time we are not sure how long the BlackTrack cycle will be, but in the near future we will try to release BlackTrack with an LTS edition (which means the update cycle follows Debian, which of course we will also try to update the repository)


# install

For this time we doesn't recommend install BlackTrack on real hardware, but, we will respect to people who install BlackTrack in hes real machine

```
# how to install
# Make sure you already connect to internet before/during installation, this only make sure some packages # installed perfectly because some packages maybe not installed normally

# Open terminal using Winkey+Shift+Enter
# inside terminal type

blacktrack@blacktrack00:~$ sudo install-debian
```

Sayonara!, Sampai berjumpa pula!


```
# BlackTrack Application pre-installed 3.0
# We apologize that we haven't been able to create an 
# application menu for the blacktrack tool list
# but we are determined to make it in the LTS edition

├── cracking
│   ├── cewl
│   ├── cowpatty
│   ├── hydra
│   ├── john
│   ├── medusa
│   ├── onesixtyone
│   └── ophcrack
├── forensic
│   ├── aircrack-ng
│   ├── audacity
│   ├── hydra
│   ├── imagemagick
│   ├── john
│   └── steghide
├── information-gathering
│   ├── btscanner
│   ├── masscan
│   ├── netdiscover
│   ├── nmap
│   ├── p0f
│   ├── reaver
│   └── wireshark
├── reverse-enginering
│   ├── apktool
│   ├── binwalk
│   ├── pe-bear
│   └── radare2
├── vulnerability-analysis
│   ├── nmap
│   └── slowhttptest
└── wireless
    ├── aircrack-ng
    ├── bettercap
    ├── bt-scanner
    ├── fern-wifi-cracker
    ├── macchanger
    ├── mitmproxy
    ├── nmap
    ├── pixiewps
    ├── reaver
    ├── responder
    ├── routersploit
    ├── wifite
    └── wireshark

```


