---
layout: docs
title: Hydra Installation standard 
permalink: /doc/installation/installation-standard
comments: true
desc: Guide book standard installation for Hydra
author: Joe
update: 2025-07-11 01:22:24 +0700
---


# Hydra Installation - Book Guide.



## Single boot installations
> Before we start please make sure you have ready to backup your data, This process will <b>Wipe</b> your data on the <b>Disk</b>


### 1.1 Preparation

I'm sure you have already know how to Installing "OS" using calamares, but don't worries we will give you guide if you doesnt know.
make sure you have ISO image from [Official Hydra site](/) (if you don't know how to download [clickme](/doc/introductions/downloading-image-from-hydra-site)).
second step you need burn ISO image to your Media such <b>FLASHDRIVE</b> or <b>CD</b> doesn't know how to burn? [clickme](/doc/introduction/make-hydra-bootable-media).
<br>

### 1.2 Boot into Hydra system using LIVE media.

next step you need to boot into Hydra Live environment, but before thats you need to <b>disable secure boot</b> first.
second step after you <b>disable secure boot</b> time to boot Hydra environment! you need to plugin your Hydra media like flashdrive into your computer, then reboot your computer for entering boot chooser select <n>media/drive</n> you already burned.
GRUB will show up, just press enter ("Try/Install").

![boot into hydrapwk](/assets/doc_assets/installation_graphics/calamares/boot-into-hydra.png)



### 1.3 Hydra Environment

in some version release Hydra you may should login and you can enter user <b>hydrapwk</b> and password <b>hydrapwk</b>.
after you success login you will seen Desktop icon with label "Install Hydra" just double click thats icon.

> In some case you need launch manually, just open terminal and type <b>"sudo debian-install"</b> may you need entering password <b>hydra</b>

Or not you can click applications launcher and type "Install HydraPWK"

![boot into hydrapwk](/assets/doc_assets/installation_graphics/calamares/whisker-menu.png)


### 2.1 Hydra calamares - Welcome

In this step you must have Installation welcome screen may will like this.
> PS: Different Hydra Version Different UI.

![Hydra calamares](/assets/doc_assets/installation_graphics/calamares/01-calamares.png)

> You can choise your language (default is American english).

you can click <n>next</n> if you sure what are you choise.


### 2.2 Hydra calamares - Location and Date.

In this step you may will see like this.

> You can set your default <b>region</b> and <b>timezone</b>

![Hydra calamares](/assets/doc_assets/installation_graphics/calamares/02-calamares.png)


### 2.3 Hydra calamares - Keyboard.

In this step you may will see like this. just choose your keyboard setup configuration.

![Hydra calamares](/assets/doc_assets/installation_graphics/calamares/03-calamares.png)

### 2.4 Hydra calamares - Partitions.

> Pls read carefully this tutorial for <b>SINGLE BOOT</b> so all data on your computer will <b>Wipe/formated</b>.

![Hydra calamares](/assets/doc_assets/installation_graphics/calamares/04-calamares.png)


### 2.5 Hydra calamares - User setup.

in this setup you will seen <b>user setup</b> screen.

> eg:<b>
username: hydra
login name: hydra
yourcomputername: hydracomputer
password: toor</b>

![Hydra calamares](/assets/doc_assets/installation_graphics/calamares/05_user_setup_bt.png)

### 2.6 Hydra calamares - Confirmation.

This is the last step, you may will seen.

> <b>This is confirmation screen, after you click next all data in your computer will wiped, and you can comeback.</b>

after you sure what are you choise just click <b>install</b>.

![Hydra calamares](/assets/doc_assets/installation_graphics/calamares/06-calamares.png)

### 2.7 Hydra calamares - Installation proccess.

> Wait until installation done, after that you can click finish and your computer automatically reboot, when your computer reboot you can unplug installation media!.

![Hydra calamares](/assets/doc_assets/installation_graphics/calamares/07-calamares.png)
![Hydra calamares](/assets/doc_assets/installation_graphics/calamares/08-calamares.png)


### End

You can reboot and dont forgot to unplug your Bootable Media

![Hydra calamares](/assets/doc_assets/installation_graphics/calamares/grub-done.png)
