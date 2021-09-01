# dmenu

My custom build of `dmenu`.

## Patches

* [alpha](https://tools.suckless.org/dmenu/patches/alpha/)
* [numbers](https://tools.suckless.org/dmenu/patches/numbers/)
* [center](https://tools.suckless.org/dmenu/patches/center/)
* [border](https://tools.suckless.org/dmenu/patches/border/)
* [fuzzymatch](https://tools.suckless.org/dmenu/patches/fuzzymatch/)
* [fuzzyhighlight](https://tools.suckless.org/dmenu/patches/fuzzyhighlight/)
* [grid](https://tools.suckless.org/dmenu/patches/grid/)
* [gridnav](https://tools.suckless.org/dmenu/patches/gridnav/)
* [bgra-glyphs](https://gitlab.freedesktop.org/mawww/libxft.git) patch for libXft
* Change Font

## Building

Since this requires having a patched version of libXft, some initial setup is
required. When first installing:

```
$ git clone --recurse-submodules https://github.com/dosisod/dmenu
$ cd dmenu/libxft
$ git checkout bgra-glyphs
$ sh autogen.sh && ./configure && make
$ cd ../freetype
$ sh autogen.sh && ./configure && make
$ cd ..
```

Tested on Ubuntu 18.04.


Original copy of `README`:

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
