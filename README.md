# TeXnicalities

A collection of own utilities for beamer presentations is available here.

In order to use the tools, a possible approach is to clone somewhere the repository and then create for each file a symbolic link into `${TEXMFHOME}`.
The repository folder structure is the standard TeX one and has to be respected inside `${TEXMFHOME}`.
The `TEXHOME` location varies on different OS and the `kpsewhich -var-value TEXMFHOME` command returns the current location of your personal tree (refer to [this SO answer](https://tex.stackexchange.com/a/271545/128737) for more information).


## The `TeXnicalities` package

Since this package is for private use, I do not offer (yet) a full documentation.
Any user who landed here is probably skilled enough to open the `.sty` file and read the commands defined there.

However, it is worth mentioning that the package can and should be loaded with a `compat=X.Y` option in order to fix a version of the used package and avoid surprises in future compilations of the same document (i.e. errors due to breaking changes of the package).
If such an option is not specified, it defaults to `compat=last`, namely the last available one.

### Relevant changes between versions

* `compat=0.2`
  * The command `\FrameRemark` is now overlay-aware and its older first argument should be now specified in angular brackets.
    The old syntax e.g. `FrameRemark[1-]{A cool remark.}` becomes `FrameRemark<1->{A cool remark.}`.
* `compat=0.1` 
  * This is the first version of the package
