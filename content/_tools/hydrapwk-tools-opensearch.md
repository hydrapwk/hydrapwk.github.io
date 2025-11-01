---
layout: tools-doc
title: OpenSearch
permalink: /doc/tools/hydrapwk-tools-opensearch
comments: true
tool-icons: /assets/graphics/tools_graphics/opensearch-logo.svg
tool-version: blank
packages-name: opensearch
tools-command: 
whoupdate: Joe
userupdate: https://github.com/me-joe
categories: O
update: 2025-11-01 07:12:00 +0700
author: Joe
editpage: https://github.com/hydrapwk/hydrapwk.github.io/blob/main/content/_tools/hydrapwk-tools-opensearch.md
tools_source: https://github.com/opensearch-project/opensearch
tools_license: https://github.com/opensearch-project/OpenSearch/blob/main/licenses/APACHE-LICENSE-2.0.txt
---

> The `opensearch` packages (.deb) on HydraPWK is not official binary of `OpenSearch` the binary `.deb` is build by HydraPWK

As default `OpenSearch` used for backend tools like [Arkime](/doc/tools/hydrapwk-tools-arkime) and [OpenSearch Dashboards](/doc/tools/hydrapwk-tools-opensearch-dashboards)

in hydrapwk default configuration of `OpenSearch`
is stored in `/etc/opensearch/`

you can modify it for setting up your own configuration.

`OpenSearch` it'self is part of service handled by `_opensearch` user, Please DON'T run `OpenSearch` manually.

## starting OpenSearch

If you want to start `OpenSearch` via application menu, you just need navigate to.

`Applications menu` -> `18-Service` -> `OpenSearch` -> `opensearch-start`

for stopping OpenSearch service you can navigate to

`Applications menu` -> `18-Service` -> `OpenSearch` -> `opensearch-stop`

## starting via terminal

if you want to start `opensearch service` via terminal you can run this command

```
hydrapwk@hydrapwk:~$ sudo systemctl start opensearch.sevice
# or
hydrapwk@hydrapwk:~$ sudo opensearch-start

# Stopping opensearch

hydrapwk@hydrapwk:~$ sudo systemctl stop opensearch.sevice
# or
hydrapwk@hydrapwk:~$ sudo opensearch-stop
```
