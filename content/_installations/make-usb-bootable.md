---
layout: docs
title: Make media bootable For HydraPWK
permalink: /doc/installation/make-media-bootable-for-hydra
comments: true
desc: Guide book to creating media bootable for HydraPWK
author: Joe
update: 2025-07-11 01:22:24 +0700
---


# Creating bootable Media For HydraPWK.

> Before we start make sure you have HydraPWK .ISO image from [Official download page](/get) HydraPWK.


### Make HydraPWK bootable media using Balena Etcher.



> before we start please download balenaetcher from official [BalenaEtcher site](https://etcher.balena.io/).

After you download [BalenaEtcher](https://etcher.balena.io/) let's open it up.

![BalenaEtcher](/assets/doc_assets/installation_graphics/bootable/balena-etcher-screen.png)

Select image (.ISO/IMG) you have already download from official HydraPWK pages.

![Select image](/assets/doc_assets/installation_graphics/bootable/choose-the-image.png)

Next step you need choose media make sure you have already insert your media.

> Make sure you backup your data before continue this step

select your media

> e.g We have Kingston data traveler

![Select media](/assets/doc_assets/installation_graphics/bootable/choose-media.png)


Last step, burn image to Media

![burn media](/assets/doc_assets/installation_graphics/bootable/start-flash.png)
![burn media](/assets/doc_assets/installation_graphics/bootable/wait-until-done.png)
![burn media](/assets/doc_assets/installation_graphics/bootable/flash-done.png)

Now you can use bootable media.


### Creating bootable media for Hydra Using DD.

> As example we have USB Flash drive you can check your media partition via fdisk


```
hydrapwk@hydrapwk:~# fdisk -l

...

Disk /dev/sda: 57,62 GiB, 61872793600 bytes, 120845300 sectors
Disk model: DataTraveler 3.0
Units: sectors of 1 * 512 = 512 bytes
Sector size (logical/physical): 512 bytes / 512 bytes
I/O size (minimum/optimal): 512 bytes / 512 bytes

...
```

My USB Flash Drive on '/dev/sda' .

> This step will erase all your data

```
hydrapwk@hydrapwk:~# dd if=hydrapwk-amd64.iso of=/dev/sda bs=4M status=proggress
...
```
