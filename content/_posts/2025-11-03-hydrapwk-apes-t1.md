---
layout: blog-read
title: "HydraPWK 2025.03.T1 (Apes) - colorscheme, opensearch, opensearch-dashboard"
date: 2025-11-01 10:15:00 +0700
author: Joe
thumbnail: /assets/graphics/post_graphics/hydrapwk-2025.03.T1/thumbnail.png
permalink: /blog/:title
description: "New update HydraPWK GNU/Linux snaphost 2025.03.T1 - colorscheme, opensearch, opensearch-dashboard"
---

Today, On hydrapwk post hydrapwk dropped new snapshot and changes.

Before we start let's talk about this `Update` this update Why use the tail number `T1`? Yeah, because it's a snapshot of a previous release.

If you remember in our [major release yesterday](/blog/hydrapwk-release-apes) we included `elasticsearch` into the HydraPWK repo, however we had some issues regarding `LICENSE` (We have announced it in the official HydraPWK [issues](https://github.com/hydrapwk/hydrapwk/issues/16) and channels), And we have pulled the `elasticsearch` package from hydrapwk, And instead, we included `OpenSearch` into the HydraPWK repo.

So basically `elasticsearch` will no longer be in HydraPWK.

We apologize for that, it was our (my) fault for not checking it more deeply.

and we want to say something, we saw some posts and reviews of hydrapwk and we really respect that and are very happy, but we also don't want people to exaggerate about HydraPWK, we are really happy with people who want to review HydraPWK it means a lot to us, but please don't compare HydraPWK or make something that is `Clickbait` for example, `HydraPWK is better than this and that` we don't want that,,, we want honesty, that's what's best for this project ... and I would be happier if there was someone who criticized this project.

# Affected packages.

So yeah, because we replaced `elasticsearch` with `OpenSearch` and of course the tools that use that `Backend`.

Arkime, now arkime in hydrapwk has used `OpenSearch` as its backend as default.

...Let's jump to `What's New?`

> Note: All packages with `<packages_name>_<packages_version>_<architecture>+hydrapwk` is build by HydraPWK

# What's new?

- Xfce terminal colorscheme - Update colorscheme `hydrapwk-purplizer` for Xfce terminal.
- [OpenSearch](#opensearch-as-backend) - is an open-source, enterprise-grade search and observability suite that brings order to unstructured data at scale.
- [OpenSearch dashboard](#opensearch-dashboards) - data visualization tool designed to work with OpenSearch.

Please check our [tools documentation](/doc/tools/hydrapwk-tools) for configuration 
# Purplizer colorscheme

In this update we updated the hydrapwk-purplizer `colorscheme` (Xfce terminal), Maybe you will notice that if there is an `error message` it will not be visible (It blends in with the terminal background), So yeah once again it was our(my) fault, so we have updated it actually we don't need to announce this, but why not if you can announce it?.

# OpenSearch as backend

As we(I) said before we included `OpenSearch` into the HydraPWK repository (note that it is not an official build of `OpenSearch`, In other words it is a build of HydraPWK).

# OpenSearch Dashboards

Great news! We added `OpenSearch Dashboards` to HydraPWK, as the `OpenSearch` binary in the HydraPWK repository is not the official `OpenSearch` binary (Built by HydraPWK).

![hydrapwk screenshoot opensearch](/assets/graphics/post_graphics/hydrapwk-2025.03.T1/hydrapwk-opensearch-dashboard.png)

![hydrapwk screenshoot opensearch dashboard sample data](/assets/graphics/post_graphics/hydrapwk-2025.03.T1/hydrapwk-dashboard-visualize.png)

# Updating

So, you have two options for updating HydraPWK. Want to download a fresh image? Of course you [can!](/get)

Too lazy to download the new images? update via `apt`!

```
hydrapwk@hydrapwk:~$ sudo apt update && sudo apt full-upgrade -y
[...]
```


...So yeah, just it and we're very sorry once again about the `Problem` and Thank you for visiting this announcement...

