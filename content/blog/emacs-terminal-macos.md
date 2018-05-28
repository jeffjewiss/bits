---
title: "Emacs Terminal MacOS"
date: 2018-05-28T14:22:35+01:00
draft: false
tags:
- emacs
- macos
- terminal
---

For a few years now my setup for programming as been a combination of Vim + Tmux
to handle text editing and managing terminals. Recently I've been trying out
Emacs as my main editor with the [Doom](http://github.com/hlissner/doom-emacs)
config, which is a nice mix of slick UI and powerful features.

The default for Emacs on MacOS is to open as a GUI app, which meant a different
workflow than I was used to. However, if you use:

```bash
emacs -nw
```

you can open emacs in a terminal window. Not all of the apps, integrations and
UI features will be available, but this allows for running Emacs in a Tmux pane
and not disrupting my usual worflow.
