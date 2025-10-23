---
layout: tools-doc
title: Arkime
permalink: /doc/tools/hydrapwk-tools-arkime
comments: true
tool-icons: /assets/graphics/tools_graphics/hydrapwk-icon-arkime.svg
tool-version: blank
packages-name: arkime
tools-command: 
whoupdate: Joe
userupdate: https://github.com/me-joe
categories: A
update: 2025-09-30 06:02:00 +0700
author: Joe
editpage: https://github.com/hydrapwk/hydrapwk.github.io/blob/main/content/_tools/hydrapwk-tools-arkime.md
---

## arkime configuration

the default configuration file of Arkime on hydrapwk is in `/etc/arkime`, as default the configuration in `/etc/arkime/*` is created by hydrapwk and handle by `arkime-data` package, you could modify your own configuration in `/etc/arkime/*`.

Please see configuration bellow to starting arkime for the first time


## Starting elasticsearch

As default `arkime` on hydrapwk using [elasticsearch](/doc/tools/hydrapwk-tools-elasticsearch) as backend, you need to start [elasticsearch](/doc/tools/hydrapwk-tools-elasticsearch) for bootstraping node, every you want to using `arkime`


## Interface configuration

As default the interface is `blank`, you need to change your own interface

you could use nano or whatever text editor.

```
hydrapwk@hydrapwk:~$ sudo nano /etc/arkime/config.ini

[...]

# find the options `interface=` as example we want to use our default host interface `wlp2s0`

interface=wlp2s0

```

## Update ipv6-geo

as default we doesn't including ipv6 on arkime-data, let arkime automatically download that

```
hydrapwk@hydrapwk:~$ sudo /usr/lib/arkime/bin/arkime_update_geo.sh
```

## Init db

This section you need to INIT arkime db you can see command bellow

```
hydrapwk@hydrapwk~$ sudo /usr/lib/arkime/db/db.pl 127.0.0.1:9200 init
```

## Adding user

this is the last step before you starting arkime, you need to create `user` and `password`, you can see command bellow.

```
hydrapwk@hydrapwk~$ sudo /usr/lib/arkime/bin/arkime_add_user.sh admin "Administrator" toor --admin
```
As you can see we're making user `admin` and password is `toor` (This is the strongest password in the world) and `--admin` options telling if `admin` user is `admin`

## Starting arkime

Finally you could start arkime.

```
hydrapwk@hydrapwk:~$ sudo arkime-start
```

if you want to start arkime again when you reboot, you don't need to setup configuration again just start the [elasticsearch](/doc/tools/hydrapwk-tools-elasticsearch) service and `arkime-start` (you could use applications menu)
