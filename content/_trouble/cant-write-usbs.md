---
layout: docs
title: cant write USB - issues 3
permalink: /doc/troubleshot/:title
comments: true
desc: HydraPWK Introduction
author: Joe
update: 2025-07-31 09:47:00 +0700
---

# HydraPWK can't read USB

This is issues This issue was raised from the issue [#3](https://github.com/hydrapwk/hydrapwk/issues/3) report.
first one we're very sorry because not including `important` part on build!.


### Packages problem
what we said we doesn't including important packages, thats why thats our mistake so if you have same problem you can install this packages.

- udisks2
- gvfs
- mtp-tools (recommend for Mtp transfer)
- ntfs-3g (recommend for ntfs media partition)

or you can copy this command

```
sudo apt install -y udisks2 \
	gvfs \
	mtp-tools \
	ntfs-3g
```

ThankYou `Bluewolftech` for reporting this issues! and I'm Sorry!
