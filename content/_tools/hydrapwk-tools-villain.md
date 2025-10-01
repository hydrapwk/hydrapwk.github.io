---
layout: tools-doc
title: villain
permalink: /doc/tools/hydrapwk-tools-villain
comments: true
tool-icons: /assets/graphics/tools_graphics/villain-logo.svg
tool-version: blank
packages-name: villain
tools-command: villain --help
whoupdate: Joe
userupdate: https://github.com/me-joe
categories: V
update: 2025-09-30 06:02:00 +0700
author: Joe
editpage: https://github.com/hydrapwk/hydrapwk.github.io/blob/main/content/_tools/hydrapwk-tools-villain.md
tools_source: https://github.com/t3l3machus/Villain
---

```
usage: Villain.py [-h] [-p PORT] [-x HOAX_PORT] [-n REVERSE_TCP_PORT]
                  [-f FILE_SMUGGLER_PORT] [-i] [-c CERTFILE] [-k KEYFILE] [-u]
                  [-v] [-q]

options:
  -h, --help            show this help message and exit
  -p, --port PORT       Team server port (default: 6501).
  -x, --hoax-port HOAX_PORT
                        HoaxShell server port (default: 8080 via http, 443 via
                        https).
  -n, --reverse-tcp-port REVERSE_TCP_PORT
                        Reverse TCP multi-handler port (default: 4443).
  -f, --file-smuggler-port FILE_SMUGGLER_PORT
                        Http file smuggler server port (default: 8888).
  -i, --insecure        Allows any Villain client (sibling server) to connect
                        to your instance without prompting you for
                        verification.
  -c, --certfile CERTFILE
                        Path to your ssl certificate (for HoaxShell https
                        server).
  -k, --keyfile KEYFILE
                        Path to the private key for your certificate (for
                        HoaxShell https server).
  -u, --update          Try to fetch the latest commits from the main branch
                        on GitHub.
  -v, --version         Show program's version number and exit.
  -q, --quiet           Do not print the banner on startup.
```