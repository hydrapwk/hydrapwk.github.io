---
layout: tools-doc
title: NetExec
permalink: /doc/tools/hydrapwk-tools-netexec
comments: true
tool-icons: /assets/graphics/tools_graphics/netexec-logo.svg
tool-version: blank
packages-name: netexec
tools-command: nxc -h
whoupdate: Joe
userupdate: https://github.com/me-joe
categories: N
update: 2025-09-30 06:02:00 +0700
author: Joe
editpage: https://github.com/hydrapwk/hydrapwk.github.io/blob/main/content/_tools/hydrapwk-tools-netexec.md
---

NetExec (a.k.a nxc) is a network service exploitation tool that helps automate assessing the security of large networks.

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

## $ nxc smb