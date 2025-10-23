---
layout: tools-doc
title: Elasticsearch
permalink: /doc/tools/hydrapwk-tools-elasticsearch
comments: true
tool-icons: /assets/graphics/tools_graphics/elasticsearch-logo.svg
tool-version: blank
packages-name: elasticsearch
tools-command: 
whoupdate: Joe
userupdate: https://github.com/me-joe
categories: E
update: 2025-09-30 06:02:00 +0700
author: Joe
editpage: https://github.com/hydrapwk/hydrapwk.github.io/blob/main/content/_tools/hydrapwk-tools-elasticsearch.md
---

As default elasticsearch on hydrapwk disabling
xpack security for making `hydrapwk team`
easier to handle some tools which use elasticsearch
as backend, like arkime.

in hydrapwk default configuration elasticsearch (elasticsearch.yml)
is stored in `/etc/elasticsearch/elasticsearch.yml`

you can modify it for setting up your own configuration.

`elasticsearch` it'self is part of service handled by `_elasticsearch` user, Please DON'T run elasticsearch manually.

## starting elasticsearch

If you want to start elasticsearch via application menu, you just need navigate to.

`Applications menu` -> `18-Service` -> `Elasticsearch` -> `elasticsearch-start`

## starting via terminal

if you want to start `elasticsearch service` via terminal you can run this command

```
hydrapwk@hydrapwk:~$ sudo systemctl start elasticsearch.sevice
or
hydrapwk@hydrapwk:~$ sudo elasticsearch-start
```
