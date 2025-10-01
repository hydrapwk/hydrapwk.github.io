---
layout: tools-doc
title: cupp
permalink: /doc/tools/hydrapwk-tools-cupp
comments: true
tool-icons: /assets/graphics/tools_graphics/hydrapwk-icons-missing.svg
tool-version: blank
packages-name: cupp
tools-command: cupp --help
whoupdate: Joe
userupdate: https://github.com/me-joe
categories: C
update: 2025-09-30 06:02:00 +0700
author: Joe
editpage: https://github.com/hydrapwk/hydrapwk.github.io/blob/main/content/_tools/hydrapwk-tools-cupp.md
---

```
 ___________ 
   cupp.py!                 # Common
                            # User
           ,__,             # Passwords
           (oo)____         # Profiler
           (__)    )    
              ||--|| *      [ Muris Kurgas | j0rgan@remote-exploit.org ]
                            [ Mebus | https://github.com/Mebus/]

usage: cupp.py [-h] [-i | -w FILENAME | -l | -a | -v] [-q]

Common User Passwords Profiler

options:
  -h, --help         show this help message and exit
  -i, --interactive  Interactive questions for user password profiling
  -w FILENAME        Use this option to improve existing dictionary, or WyD.pl
                     output to make some pwnsauce
  -l                 Download huge wordlists from repository
  -a                 Parse default usernames and passwords directly from
                     Alecto DB. Project Alecto uses purified databases of
                     Phenoelit and CIRT which were merged and enhanced
  -v, --version      Show the version of this program.
  -q, --quiet        Quiet mode (don't print banner)
```