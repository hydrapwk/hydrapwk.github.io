---
layout: blog-read
title: "HydraPWK update - (GTK themes, new tools, icons update)"
date: 2025-09-19 23:30:00 +0700
author: Joe
thumbnail: /assets/graphics/post_graphics/hydrapwk-update-theme-tools-icons/thumbnail.png
permalink: /blog/:title
description: "Today, HydraPWK Update new GTK theme (Hydra-Dark), new icons for HydraPWK tools, new tools."
---

Today, HydraPWK update GTK themes, new icons and tools.


> Once again, if you still using HydraPWK (Transition) IMAGE/ISOs `2025.01.6.5.*` please update into the latest HydraPWK IMAGE/ISOs.

# What's new?

- new themes - [Dark theme for HydraPWK](#new-themes)
- new tools - [esptool, Caringcaribou](#new-tools)
- new icons - [new icons for HydraPWK tools](#new-icons)


# New tools

- esptool - [tools for flashing and related esp from espressife](https://github.com/espressif/esptool)
- caringcaribou - [A friendly car security exploration tool for the CAN bus](https://github.com/CaringCaribou/caringcaribou)

# New themes

![HydraPWK Dark GTK theme](/assets/graphics/post_graphics/hydrapwk-update-theme-tools-icons/hydrapwk-htop.png)

In this update we're adding new GTK theme (dark theme `fork from skeuos gtk`) for HydraPWK! Previously we're only providing `light theme`.

Honestly this is not pure `dark` theme, this is combination `light` and `dark` colors but don't worry, for base themes we're using `dark` color!.

If you using latest HydraPWK (codename yellowdog) you can easily install this time, use APT!.

```
# if you using `hydrapwk-2025.02.250817233-yellowdog-T2` IMAGE/ISOs you don't need to doing this
...
hydrapwk@hydrapwk:~$ sudo apt update && sudo apt full-upgrade -y # wait until the process done
...
...
hydrapwk@hydrapwk:~$ cp -r /etc/skel/.config/xfce4 ~/.config # only if you want to using dotfiles HydraPWK!
...
```

# New icons

And we have been creating new icons for HydraPWK tools, you can see image below!.

![HydraPWK Icons](/assets/graphics/post_graphics/hydrapwk-update-theme-tools-icons/hydrapwk-new-icons.png)
