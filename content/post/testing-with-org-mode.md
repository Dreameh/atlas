+++
title = "Testing with org-mode"
author = ["Dreameh"]
lastmod = 2018-10-14T20:47:50+03:00
tags = ["emacs", "Nikola", "org-mode"]
draft = false
+++

## Nikola {#nikola}

Using org-mode with nikola is a blast, writing everything down in org-mode
then just building it afterwards couldn't really be easier.


## Code blocks {#code-blocks}

using code-blocks is easy as well...

```python
def f(x):
    """ because docstrings is pissing me off """
    return x * x

print("Test" + str(f(5)))
```


## Note taking {#note-taking}

Using org-mode is such a blast, that even note-taking can be easy and fun.
Just open up a org-file, call it something like... "notes.org"
then in your org config file, you can add this:

```
(custom-set-variables
 '(org-directory "Where your default org-directory is...")
 '(org-default-notes-file (concat org-directory "/notes.org")))
```
