---
layout: blog-read
title: "HydraPWK new snapshot - (snapshot, metapackages, tools, drop support HydraPWK Transition)"
date: 2025-09-13 05:49:00 +0700
author: Joe
thumbnail: /assets/graphics/post_graphics/hydrapwk-new-snapshot-t1/thumbnail.png
permalink: /blog/:title
description: Today, in HydraPWK post new snapshot, metapackages linux-image-xhydra, Kismet, drop support for HydraPWK Transition release.
---

Today, in HydraPWK post new snapshot, metapackages, tools, drop support for HydraPWK Transition release.

# What's new?

- New tools added - [kismet](#kismet)
- New metapackages - [linux-image-xhydra metapackages](#linux-image-xhydra)
- Drop support - [Discontinued HydraPWK (2025.01.6.5.*)support and repo](#drop-support)

# Kismet

Now kismet added in HydraPWK repo!

What is kismet?

Kismet is an open source sniffer, WIDS, wardriver, and packet capture tool for Wi-Fi, Bluetooth, BTLE, wireless thermometers, airplanes, power meters, Zigbee.

# Drop packages support

Here is, In the near future, this tool will no longer be included in the HydraPWK repository.

- squarephish
- ufonet

You can also, check this pages for information (status) tools in HydraPWK.

[HydraPWK tools status](https://hydrapwk.github.io/doc/tools-tracker)

# Linux image xhydra

We've been made new metapackages for HydraPWK.

What Is this for?

If you know about metapackages like `linux-image-amd64` on Debian, linux-image-xhydra Acting same (do same job) as a metapckages for kernel update, and it will make easier for us (me) for giving an update.

With hope, making it easier when updating, so you don't need to manually choosing kernel version, just use `apt` for upgrading kernel for HydraPWK.

If you using new IMAGE/ISOs (hydrapwk-2025.02.250817233-yellowdog-T1) you could skip this step.

Installing linux-image-xhydra on your HydraPWK machine

```
...
sudo apt update
sudo apt install -y linux-image-xhydra
...
```

# Drop support.

With this we drop support (discontinued) for the release of Hydrapwk with the release of the code `'Transition' (2025.01.6.5.*) Debian Trixie base`, and we could fully working for `HydraPWK yellowdog release`!.

And with that's, good bye transition!.


# Support and resources

GitHub issues - [Have problem or critique? Open issues now!](https://github.com/hydrapwk/hydrapwk/issues/)

Troubleshoot pages - [HydraPWK Official Troubleshoot page](https://hydrapwk.github.io/doc/troubleshot)

Reddit community - [HydraPWK Official subredit](http://reddit.com/r/hydrapwk)

Telegram community - [HydraPWK Official Telegram Community](https://t.me/blacktracksec)

Mastodon - [infosec.exchange](https://infosec.exchange/@hydrapwk)

Distrowatch - [HydraPWK distrowatch page](https://distrowatch.com/table.php?distribution=hydrapwk)

# latest independent review about HydraPWK 

> Newest review

connectwww - [How to Install HydraPWK Linux on VirtualBox](https://youtu.be/adWY0YY8j4Q?si=RerYTmPIObhMOhX4)

iguru.gr - [HydraPWK (Αύγουστος) Stress Test, Cracking, Reversing, Forensics](https://iguru.gr/hydrapwk-avgoustos-stress-test-cracking-reversing-forensics/)

..

> Older review

Penguinreviewlinux.org - [HydraPWK GNU/Linux 2025.01.6.5.250806258: Distribuția open-source pentru hacking și pentesting, cu nucleu Real-Time și unelte avansate](https://penguinreviewslinux.blogspot.com/2025/08/hydrapwk-gnulinux-20250165250806258.html?m=1)

Desdelinux - [Top nuevas Distros Linux / BSD a ser reconocidas en 2025: Parte 08](https://blog.desdelinux.net/top-nuevas-distros-gnu-linux-2025-08/)
[Penguin reviews](https://penguinreviewslinux.blogspot.com/2025/08/hydrapwk-gnulinux-20250165250806258.html?m=1)

Gladilov.org.ru - [Новая виртуальная ОСь — 22.07.2025](https://www.gladilov.org.ru/blog/all/new-virtual-os-22-07-2025/)

NX11Dev [HydraPWK GNU/Linux：Debian系渗透测试利器，以开源之力筑牢网络安全防线](https://m.bilibili.com/video/BV14pbXzJE5J)

[Iguru.gr](https://iguru.gr/hydrapwk-scan-stress-test-exploitation-cracking-reversing-forensics/)
