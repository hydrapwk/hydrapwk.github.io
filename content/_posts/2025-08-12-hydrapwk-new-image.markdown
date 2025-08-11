---
layout: blog-read
title: "HydraPWK 2025.01.6.5.250806258"
date: 2025-08-12 05:24:00 +0700
author: Joe
thumbnail: /assets/graphics/post_graphics/hydrapwk-2025-01.6.5.250806258/hydrawpk-2025-update-image.png
permalink: /blog/:title
description: Today HydraPWk GNU/Linux update new IMAGES/ISOS, TvBox Alpha, semi-rolling, new tools, discontinued packages, etc.
---
Today HydraPWk GNU/Linux releases new Images and TvBox alpha.
like we said before, we will release HydraPWK Image and TvBox alpha, also this time we're will trying `semi-rolling` release, previously in BlackTrack we're using fixed release.

- new tools - [2 tools adding into our repo!](#new-tools).
- new IMAGE/ISO - [Update HydraPWK standard ISO/IMAGE](#new-image)
- new Metapackages - [Utilities metapackages](#metapackages)
- release plan - [HydraPWK planning for semi-rolling release](#release)
- TvBox Alpha - [Alpha Image HydraPWK TvBox](#tvbox)
- user review - [Blog, article, content reviewing HydraPWK](#review)

# New tools

- hackrf - [hackrf-host](https://github.com/greatscottgadgets/hackrf/tree/master/host)
- seclists - [seclists wordlist collections](https://github.com/danielmiessler/SecLists)

not only new tools, we're also drop somepackages. here is the list discontinued packages.

- burpsuite
- fern-wifi-cracker
- qrljacking

Why we do this? Off course because our main Purpose, and for efficiency for our repo, we don't have much resource that's why!

# IMAGE/ISO

IMAGE update fixing [issues](https://github.com/hydrapwk/hydrapwk/issues) in the last week.

# Metapackages

for handle our mistake like we forgot including utility tools while building IMAGE, we've been made metapackages containt Utility tools.

```
sudo apt update && sudo apt install -y hydrapwk-utilities
```

# Release

For the first time we will trying to use `semi-rolling`, so in this update you don't need to download new IMAGE/ISO (But still recommend to download new IMAGE).

> If you using new IMAGE (hydrapwk-2025.01.6.5.250806258-amd64) you don't need to do this, but still recommended

```
...
hydrapwk@hydrapwk:~$ sudo apt update && sudo apt full-upgrade -y
...

verify HydraPWK version make sure the version same as 2025.01.6.5.250806258

...
hydrapwk@hydrapwk:~$ cat /etc/hydrapwk_version

2025.01.6.5.250806258 #make sure the version same like this

....
```

# TvBox

Yup! in our last post this week we're said still developing HydraPWK for TvBox! and now Alpha IMAGE is OUT! You can try and send feedback to us!

# Review

I'm very happy, i just seen some content / article reviewing HydraPWK! here is!

- [iguru.gr](https://iguru.gr/hydrapwk-scan-stress-test-exploitation-cracking-reversing-forensics/)
- [gladilov.org](https://gladilov.org.ru/blog/all/new-virtual-os-22-07-2025/)
- [Nano11XDEV](https://www.bilibili.com/video/BV14pbXzJE5J/)

Thankyou for all reviewer! it's surprising me!
