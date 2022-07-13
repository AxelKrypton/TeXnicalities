# TeXnicalities

A collection of own utilities for beamer presentations is available here.

In order to use the tools, a possible approach is to clone somewhere the repository and then create for each file a symbolic link into `${TEXMFHOME}`.
The repository folder structure is the standard TeX one and has to be respected inside `${TEXMFHOME}`.
The `TEXHOME` location varies on different OS and the `kpsewhich -var-value TEXMFHOME` command returns the current location of your personal tree (refer to [this SO answer](https://tex.stackexchange.com/a/271545/128737) for more information).

