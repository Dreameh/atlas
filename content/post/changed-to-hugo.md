+++
title = "Changed to hugo"
author = ["Dreameh"]
lastmod = 2018-10-14T23:15:07+03:00
tags = ["Hugo", "emacs", "org-mode"]
categories = ["Linux", "Blog"]
draft = false
+++

## Hugo {#hugo}

Changing from Nikola to Hugo can a somewhat of a drag, you will have to
download the package **ox-hugo** and then set it up as what the doctor ordered.

After that little process of adding the fun stuff into your config you can essentially just
add every org file that you have as a post on Nikola to a **content-org** folder (not forced)
afterwards, add these tags in order to make it easy just to pass it to the website.

```
#+title:
#+hugo_base_dir: ../
#+hugo_section: ./posts

#+hugo_weight: auto
#+hugo_tags:
#+hugo_auto_set_lastmod: t
#+hugo_categories:

#+author: Dreameh
```

Now all that will do is pretty self-explanatory, add your content, export it through:
**C-c C-e H h** and it will become a markdown file made for Hugo's content standard.

Now for the single most important part, run the server with: **hugo server**.
