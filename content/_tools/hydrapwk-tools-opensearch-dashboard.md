---
layout: tools-doc
title: OpenSearch Dashboards
permalink: /doc/tools/hydrapwk-tools-opensearch-dashboard
comments: true
tool-icons: /assets/graphics/tools_graphics/opensearch-logo.svg
tool-version: blank
packages-name: opensearch-dashboard
tools-command: 
whoupdate: Joe
userupdate: https://github.com/me-joe
categories: O
update: 2025-11-01 07:13:00 +0700
author: Joe
editpage: https://github.com/hydrapwk/hydrapwk.github.io/blob/main/content/_tools/hydrapwk-tools-opensearch-dashboard.md
---

> The `opensearch-dashboard` packages (.deb) on HydraPWK is not official binary of `OpenSearch` the binary `.deb` is build by HydraPWK

in hydrapwk default configuration of `OpenSearch Dashboards`
is stored in `/etc/opensearch-dashboard/`

you can modify it for setting up your own configuration.

`OpenSearch` it'self is part of service handled by `_opensearch` user, Please DON'T run `OpenSearch` manually.

## starting OpenSearch Dashboards

If you want to start `OpenSearch Dashboards` via application menu, you just need navigate to.

`Applications menu` -> `18-Service` -> `OpenSearch` -> `opensearch-dashboard-start`

for stopping `OpenSearch Dashboards` service you can navigate to

`Applications menu` -> `18-Service` -> `OpenSearch` -> `opensearch-dashboard-stop`

## starting via terminal

if you want to start `opensearch-dashboard service` via terminal you can run this command

```
hydrapwk@hydrapwk:~$ sudo systemctl start opensearch-dashboard.sevice
# or
hydrapwk@hydrapwk:~$ sudo opensearch-dashboard-start

# Stopping opensearch

hydrapwk@hydrapwk:~$ sudo systemctl stop opensearch-dashboard.sevice
# or
hydrapwk@hydrapwk:~$ sudo opensearch-dashboard-stop
```
