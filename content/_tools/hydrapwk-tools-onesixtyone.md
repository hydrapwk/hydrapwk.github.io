---
layout: tools-doc
title: onesixtyone
permalink: /doc/tools/hydrapwk-tools-onesixtyone
comments: true
tool-icons: /assets/graphics/tools_graphics/onesixtyone-logo.svg
tool-version: blank
packages-name: onesixtyone
tools-command: onesixtyone --help
whoupdate: Joe
userupdate: https://github.com/me-joe
categories: O
update: 2025-09-30 06:02:00 +0700
author: Joe
editpage: https://github.com/hydrapwk/hydrapwk.github.io/blob/main/content/_tools/hydrapwk-tools-onesixtyone.md
---

```
onesixtyone 0.3.3 [options] <host> <community>
  -c <communityfile> file with community names to try
  -i <inputfile>     file with target hosts
  -o <outputfile>    output log
  -p                 specify an alternate destination SNMP port
  -d                 debug mode, use twice for more information

  -s                 short mode, only print IP addresses

  -w n               wait n milliseconds (1/1000 of a second) between sending packets (default 10)
  -q                 quiet mode, do not print log to stdout, use with -o
host is either an IPv4 address or an IPv4 address and a netmask
default community names are: public private

Max number of hosts :     65536
Max community length:     32
Max number of communities:  16384


examples: onesixtyone 192.168.4.0/24 public
          onesixtyone -c dict.txt -i hosts -o my.log -w 100

```