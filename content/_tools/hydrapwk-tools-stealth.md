---
layout: tools-doc
title: hydrapwk-stealth
permalink: /doc/tools/hydrapwk-tools-hydrapwk-stealth
comments: true
tool-icons:
tool-version: blank
packages-name: hydrapwk-stealth
tools-command: 
whoupdate: Joe
userupdate: https://github.com/me-joe
categories: H
update: 2025-12-02 06:14:00 +0700
author: Joe
editpage: https://github.com/hydrapwk/hydrapwk.github.io/blob/main/content/_tools/hydrapwk-tools-stealth.md
---

HydraPWK Stealth is designed for reduce `IDs (Instruction detection system)`

Note: you need to install `hydrapwk` on your machine

hydrapwk-stealth is temporary user, the home of hydrapwk-stealth `/home/hydrapwk-stealth` is temp (Running on RAM)



# First init

For the first time you need to choose `interface` for `hydrapwk-stealth` as example our interface is `wlp2s0`

```
hydrapwk@hydrapwk:~# echo wlp2s0 > /opt/interface
```

After that you can Init the `hydrapwk-stealth`

```
hydrapwk@hydrapwk:~# hydrapwk-stealth-init
# Enable hydrapwk stealth
hydrapwk@hydrapwk:~# systemctl enable hydrapwk-stealth
```
And it's should success and you can reboot and you will saw `HydraPWK STEALTH` you could select it and you will boot into `hydrapwk-stealth` on the login screen you can login as user:`hydrapwk-stealth` pass:`hydrapwk`