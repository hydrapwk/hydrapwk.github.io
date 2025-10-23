---
layout: blog-read
title: "HydraPWK 2025.03 (Apes) - arkime, elasticsearch, purplizer, desktop-changes, tools page"
date: 2025-10-23 11:37:00 +0700
author: Joe
thumbnail: /assets/graphics/post_graphics/hydrapwk-2025.03-apes/thumbnail.png
permalink: /blog/:title
description: "New release HydraPWK GNU/Linux 2025.03 (Apes) - hydrapwk purplizer, arkime, elasticsearch, tools documentation page"
---

Today in HydraPWK blog post HydraPWK released new version of HydraPWK, say hello to HydraPWK 2025.03 (Apes).


and the best things is, now hydrapwk is defensive too!
another word, not just focus on pentesting and hydrapwk will be `security auditing toolkit` instead `Pentesting toolkit`.


> Don't worry about bloatware, hydrapwk still same `One task one tool` all the tools on hydrapwk is curated tools. All the tools we choice is based on real-world case.


# What's new?

- [HydraPWK Logo 2.0](#hydrapwk-logo-2.0) - hydrapwk updated logo (2.0)!
- [New tools](#new-tools) - arkime, elasticsearch
- [Polkit rules](#polkit-rules) - new hydrapwk Polkitd rules
- [Desktop changes](#desktop-changes) - HydraPWK purplizer, menu
- [Hardware reuqirements](#hardware-requirements) - Update recommended (Minimal hardware requirements)
- [Tools documentation](#tools-doc) - tools-documentation page
- [Updating hydrapwk](#Updating-hydrapwk) - Update hydrapwk using fresh image or APT.

# HydraPWK Logo 2.0

so! say hy! to hydrapwk logo 2.0! This is updated logo from HydraPWK 1.0
what's the different?

as you can see the different between HydraPWK Logo 1.0
and new logo (2.0), we made some changes as you can see bellow, like wings, and hydrapwk body...

![HydraPWK Logo 2.0](/assets/graphics/post_graphics/hydrapwk-2025.03-apes/hydrapwk-logo-2.0.png)

[Check more details](/doc/hydrapwk-policy-trademark)

# New tools

- [elasticsearch](/doc/tools/hydrapwk-tools-elasticsearch) - Elasticsearch is a distributed search and analytics engine, scalable data store and vector database optimized for speed and relevance on production-scale workloads.
- [Arkime](/doc/tools/hydrapwk-tools-arkime) - scalable packet capture

# Arkime And elasticsearch

Please read the tool documentation for [Arkime](/doc/tools/hydrapwk-tools-arkime) and [Elasticsearch/elasticsearch service](/doc/tools/hydrapwk-tools-elasticsearch)

As default hydrapwk using `elasticsearch as backend of arkime`
and vice versa `elasticsearch` would be backend for several tools like `arkime` on the future.(I hope)

![Arkime](/assets/graphics/post_graphics/hydrapwk-2025.03-apes/hydrapwk-arkime.png)

# Polkit rules

Here is we made polkit rules for hydrapwk menu

![HydraPWK Pkexec window](/assets/graphics/post_graphics/hydrapwk-2025.03-apes/hydrapwk-polkit.png)

# Desktop changes

Here is! the one of the good part `hydrapwk-purplizer` and

like we say before hydrapwk now is not just for pentesting
 and we've been made new category `defensive` category! based on NIST CSF 2.0 Framework!

> HydraPWK Menu

![HydraPWK Menu Defense](/assets/graphics/post_graphics/hydrapwk-2025.03-apes/hydrapwk-menu-defense.png)


> HydraPWK Desktop

![HydraPWK Menu Defense](/assets/graphics/post_graphics/hydrapwk-2025.03-apes/hydrapwk-desktop.png)

# Tools doc

so yeah we've been made [Tools documentation page](/doc/tools) hydrapwk several weeks ago i guess, but yeah we still need to improvement to the Documentation...
but ofc! You could contribute.
how? The hydrapwk page is hosted by GitHub and Jekyll so you could easily edit the markdown, on the tools doc on the bottom left corner you will see `Edit this page` button, and you can click it!

![HydraPWK tools page](/assets/graphics/post_graphics/hydrapwk-2025.03-apes/hydrapwk-tools-doc.png)


# Hardware requirements

here is, this is our recommandation (Minimal) hardware to run hydrapwk.

| RAM | DISK | CPU |
|:-----:|:---:|:-----:|
| 8-16GB | 16GB+ | intel i3 |

# Updating hydrapwk

> Update hydrapwk using fresh image? Yes you can [Get hydrapwk image now](/get)

so yeah don't worry, if you have already hydrapwk yellowdog you can update you're hydrapwk to the latest version (Apes) easily.


we've been made `hydrapwk-helper` it will automatically
change the `yellowdog repo to apes` but how?

its enough that's because the `hydrapwk-helper` has part of `hydrapwk-utilities` metapackages


```
hydrapwk@hydrapwk:~$ sudo apt update && sudo apt full-upgrade -y # this is will pull `hydrapwk-helper`
[...] # After thats you need to initialize hydrapwk apes
hydrapwk@hydrapwk:~$ sudo apt update && sudo apt full-upgrade
```

And boom! now you could check your hydrapwk version

```
hydrapwk@hydrapwk:~$ grep VERSION /usr/lib/os-release
# Now the output should be `apes`
```

