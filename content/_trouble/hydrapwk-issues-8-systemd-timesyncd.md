---
layout: docs
title: Clock not sync with ntp (sqv error on apt)
permalink: /doc/troubleshot/:title
comments: true
author: Joe
update: 2025-10-02 22:16:00 +0700
---

# Problem with repo sqv (clock is not sync) Fixed with systemd-timesyncd packages

This issue was raised from the issue [#8](https://github.com/hydrapwk/hydrapwk/issues/8) report.

do

```
sudo ntpdate-debian # this is will automatically sync the clock to ntp server before you using APT
sudo apt update && sudo apt full-upgrade -y # Upgrade all packages containt hydrapwk metapackages (hydrapwk-utilities) metapackages
```

we(me) apologize for this problem because we're always forgot important things