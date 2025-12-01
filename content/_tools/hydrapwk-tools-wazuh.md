---
layout: tools-doc
title: Wazuh
permalink: /doc/tools/hydrapwk-tools-wazuh
comments: true
tool-icons: /assets/graphics/tools_graphics/wazuh-logo.svg
tool-version: blank
packages-name: wazuh
tools-command: 
whoupdate: Joe
userupdate: https://github.com/me-joe
categories: W
update: 2025-12-02 06:15:00 +0700
author: Joe
editpage: https://github.com/hydrapwk/hydrapwk.github.io/blob/main/content/_tools/hydrapwk-tools-wazuh.md
tools_source: 
tools_license: 
---

> The `wazuh` packages (.deb) on HydraPWK is not official(Unofficial) binary of `wazuh` the binary `.deb` is build by HydraPWK

Note: You need minimal 16GB RAM, 32GB DISK, 4 CORE CPU OR `HIGHER` and you should run HydraPWK On `bare-metal` not in `Live environment` The `init` might be `fail`

Caution: The `init` might be `fail` if your `hardware(Machine) very low`.

in hydrapwk default configuration of `wazuh-indexer` is stored in `/etc/wazuh-indexer/` and `wazuh-dashboard` is stored in `/etc/wazuh-dashboard`


you can modify it for setting up your own configuration.

## starting and init Wazuh

For the first time you need to `INIT` wazuh to generate password and `SSL Certs`

you could navigate to : `Applications menu` -> `Respond` -> `Wazuh`

or via terminal type

```
hydrapwk@hydrapwk:~$ sudo wazuh-start
```

After that the terminal will show up for the first Time (INIT wazuh for the first time)

This is may take 5 Minutes (Depends on your machine)

you may will get this message

`A keystore already exists, Overwrite? [y/N]:`

you can just `y` and enter

```
[...]

Starting wazuh manager
Wazuh manager is online
Starting Filebeat giving 8sec to Up
Filebeat is online
Starting Wazuh indexer giving 60sec to UP
Filebeat is online
Init filebeat
A keystore already exists, Overwrite? [y/N]:y

[...]
```

After the `init` success fully will get message like this


```
Starting wazuh about 20sec...
Wazuh indexer...OK
Wazuh manager...OK
Filebeat...OK
Wazuh dashboards...OK
Login credentials. user: admin password: user: admin password: 7QG+wcgs6y9NkXAg # <Generated password check on /opt/wazuh-pass.$(date)>
Your pass has been stored in /opt/wazuh-pass.datenow
Wazuh starting on https://127.0.0.1:5601
```

And here we go! you can now access wazuh on you'r browser, you could check your login password (Admin) in `/opt/wazuh-pass.$(date)` or `/opt/.wazuh-pass-latest`


## Generate new pass.

Note: Only change your pass if really needed

Generate new password for wazuh on `hydrapwk` is easy you only need to open terminal and type

```
hydrapwk@hydrapwk:~$ sudo wazuh-gen-new-pass
```

And it's would automatically generate your pass and you might will get this message

`A keystore already exists, Overwrite? [y/N]:`

you can just `y` and enter

```
[...]

Starting wazuh manager
Wazuh manager is online
Starting Filebeat giving 8sec to Up
Filebeat is online
Starting Wazuh indexer giving 60sec to UP
Filebeat is online
Init filebeat
A keystore already exists, Overwrite? [y/N]:y

[...]
```

Your new password will stored in `/opt/wazuh-pass.datenow` after that you need to modify `/etc/wazuh-dashboard/opensearch_dashboards.yml`

find the line with strings `opensearch.pass: "This is your old password"` and replace the `Your old password` with the new password you just generate (admin password) you can find your latest password in `/opt/.wazuh-pass-latest`



.