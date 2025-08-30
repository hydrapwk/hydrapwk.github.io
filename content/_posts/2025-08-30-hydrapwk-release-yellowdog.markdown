---
layout: blog-read
title: "HydraPWK 2025.02.250817233 yellowdog release (new tools, netexec, hydrapwk-menu, Debian forky/sid base)"
date: 2025-08-30 06:37:00 +0700
author: Joe
thumbnail: /assets/graphics/post_graphics/hydrapwk-2025.02-yellowdog/thumbnail.png
permalink: /blog/:title
description: Release beta HydraPWK yellowdog 2025.02.250817233 - (netexec, exploitdb, modpoll, 6.16 kernel, Debian Forky/sid base)
---

Today, in HydraPWK Post HydraPWK released new version of HydraPWK (yellowdog 2025.02.250817233) like we said in previous announcement [here](https://hydrapwk.github.io/blog/hydrawpk-migrate)
we will migrate from "Debian Trixie base" into "Debian Forky/sid" and we've been announcement in our community group (reddit, telegram and mastodon)
we just freeze HydraPWK version 2025.01.6.5.* so we can focus on "Debian Forky/sid base" maybe you confused about our release "semi-rolling".

What's actually "semi-rolling" means(in HydraPWK)? Actually it's very, very different from "rolling" release, if we release new version HydraPWK with same
"branch or same base" we can still handle that's, but if release with new branch (base) so we will cut-off or Freeze (previous release which used older base) but
don't worry we will still give you update like fixed bug for 1-2 weeks? We can't make sure that's and If we feel the new base is "sufficient",
we will migrate completely to the new base.


# What's new?

- menu refresh - [Hybrid MITRE ATT&CK Tactics](#menu-refresh)
- new tools - [netexec, modpoll, exploitdb](#new-tools)
- kernel - [updating kernel to version 6.16](#kernel-update)
- can-j19399 - [new pre-built can-j19399 module](#kernel-update)
- separate metapackages - [Remove hydrapwk-default-tools from hydrapwk-defaults](#separate-metapackages)
- expanding impacket library - [Expanding impacket library (impacket-*)[#impacket library]

# Menu refresh
- 01-Reconnaise
- 02-Resource development
- 03-Initial Access
- 04-Execution
- 05-Persistence
- ...
- Until 17-Forensic :)

![HydraPWK Applications menus MITRE ATT&CK Hybird](/assets/graphics/post_graphics/hydrapwk-2025.02-yellowdog/hydrapwk-menu.png)

As you can seen we've been "Update menu" for HydraPWK, Which this menu folllowing "Mitre ATT&CK" tactics (Hybird Enterpise and Industry).

# New tools
new tools Added on This release!

- netexec

```
usage: netexec [-h] [--version] [-t THREADS] [--timeout TIMEOUT]
               [--jitter INTERVAL] [--verbose] [--debug] [--no-progress]
               [--log LOG] [-6] [--dns-server DNS_SERVER] [--dns-tcp]
               [--dns-timeout DNS_TIMEOUT]
               {vnc,rdp,smb,ftp,nfs,mssql,wmi,ssh,winrm,ldap} ...

     .   .
    .|   |.     _   _          _     _____
    ||   ||    | \ | |   ___  | |_  | ____| __  __   ___    ___
    \\( )//    |  \| |  / _ \ | __| |  _|   \ \/ /  / _ \  / __|
    .=[ ]=.    | |\  | |  __/ | |_  | |___   >  <  |  __/ | (__
  / /Ë™-Ë™\ \  |_| \_|  \___|  \__| |_____| /_/\_\  \___|  \___|
  Ë™ \   / Ë™
    Ë™   Ë™

    The network execution tool
    Maintained as an open source project by @NeffIsBack, @MJHallenbeck, @_zblurx

    For documentation and usage examples, visit: https://www.netexec.wiki/

    Version : 1.4.0+hydrapwk1
    Codename: SmoothOperator
    Commit  :

options:
  -h, --help            show this help message and exit

Generic:
  Generic options for nxc across protocols

  --version             Display nxc version
  -t, --threads THREADS
                        set how many concurrent threads to use
  --timeout TIMEOUT     max timeout in seconds of each thread
  --jitter INTERVAL     sets a random delay between each authentication

Output:
  Options to set verbosity levels and control output

  --verbose             enable verbose output
  --debug               enable debug level information
  --no-progress         do not displaying progress bar during scan
  --log LOG             export result into a custom file

DNS:
  -6                    Enable force IPv6
  --dns-server DNS_SERVER
                        Specify DNS server (default: Use hosts file & System DNS)
  --dns-tcp             Use TCP instead of UDP for DNS queries
  --dns-timeout DNS_TIMEOUT
                        DNS query timeout in seconds

Available Protocols:
  {vnc,rdp,smb,ftp,nfs,mssql,wmi,ssh,winrm,ldap}
    vnc                 own stuff using VNC
    rdp                 own stuff using RDP
    smb                 own stuff using SMB
    ftp                 own stuff using FTP
    nfs                 own stuff using NFS
    mssql               own stuff using MSSQL
    wmi                 own stuff using WMI
    ssh                 own stuff using SSH
    winrm               own stuff using WINRM
    ldap                own stuff using LDAP

```
- exploitdb(searchsploit)
- modpoll

# Impacket library

So, yeah for make easier we're decide to expand some impacket library, so you don't need to enter /usr/share/doc/python3-impacket/examples/ directory

```
/usr/bin/impacket-atexec	/usr/bin/impacket-registry-read
/usr/bin/impacket-changepasswd	/usr/bin/impacket-regsecrets
/usr/bin/impacket-dcomexec	/usr/bin/impacket-rpcdump
/usr/bin/impacket-exchange	/usr/bin/impacket-rpcmap
/usr/bin/impacket-samrdump      /usr/bin/impacket-mimikatz
/usr/bin/impacket-mqtt_check	/usr/bin/impacket-smbclient
/usr/bin/impacket-mssqlclient	/usr/bin/impacket-smbexec
/usr/bin/impacket-netview	/usr/bin/impacket-smbserver
/usr/bin/impacket-ping		/usr/bin/impacket-sniff
/usr/bin/impacket-ping6		/usr/bin/impacket-sniffer
/usr/bin/impacket-psexec	/usr/bin/impacket-ticketConverter
/usr/bin/impacket-rdp_check	/usr/bin/impacket-ticketer
/usr/bin/impacket-reg		/usr/bin/impacket-wmiexec
/usr/bin/impacket-secretsdump
```

# Kernel Update

So we have update HydraPWK kernel to latest stable Linux kernel 6.16 and Enabling "can-j1939" modules


# Seperate metapackages

As you know in our HydraPWK version 2025.01.6.5.* we combine packages hydrapwk-default-tools inside hydrapwk-defaults as dependencies.

and we relize it's not a good things, so we decide to remove hydrapwk-default-tools from hydrapwk-defaults (as dependencies), and not including in ISO/IMAGE
that's because as you know, if you delete, just one tools, your environment will broke, were very sorry about thats.

don't worry you're free now to remove tools.

# Upgrading

So like we said before, this release we're using Debian Forky/sid as base, so you need to download `beta iso for updating`, but don't worry if you doesn't want to update to 'This release (beta) with codename yellowdog' you can still using stable base, but ofc it's will got freeze, but don't worry we will maintenance the repo for stable base for maybe 1 week
