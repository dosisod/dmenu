# dmenu

My custom build of `dmenu`.

## Patches

* [alpha](https://tools.suckless.org/dmenu/patches/alpha/)
* [bgra-glyphs](https://gitlab.freedesktop.org/mawww/libxft.git) patch for libXft
* [center](https://tools.suckless.org/dmenu/patches/center/)
* [border](https://tools.suckless.org/dmenu/patches/border/)
* [fuzzymatch](https://tools.suckless.org/dmenu/patches/fuzzymatch/)
* [fuzzyhighlight](https://tools.suckless.org/dmenu/patches/fuzzyhighlight/)
* [grid](https://tools.suckless.org/dmenu/patches/grid/)
* [gridnav](https://tools.suckless.org/dmenu/patches/gridnav/)
* [initialtext](https://tools.suckless.org/dmenu/patches/initialtext/)
* [password](https://tools.suckless.org/dmenu/patches/password/)
* Change Fonts and other settings

## Building

On Arch Linux, install the [libxft-bgra](https://aur.archlinux.org/packages/libxft-bgra/)
and [freetype2](https://archlinux.org/packages/extra/x86_64/freetype2/)
packages, then run `make && sudo make install`.

For instructions for building on Ubuntu 18.04, click
[here](https://github.com/dosisod/dmenu/tree/ubuntu1804#building) (no longer maintained).

Copy of original `README`:

```
dmenu - dynamic menu
====================
dmenu is an efficient dynamic menu for X.


Requirements
------------
In order to build dmenu you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (dmenu is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dmenu
(if necessary as root):

    make clean install


Running dmenu
-------------
See the man page for details.
```
