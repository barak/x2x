# x2x

## Project status

Dormant. This project needs a new maintainer.

x2x has a long history. It was born in the times when life was hard, window
managers were simple and displays were rectangular. Now it needs an overhaul.

## Overview

x2x allows the keyboard, mouse on one X display to be used to control another X
display. It also shares X clipboards between the displays.

When built/run on Cygwin it may be run on Windows desktop to control X display.

## License

x2x is under MIT/BSD license.

Windows support includes code under GPLv2+.

## Authors

x2x was initially developed in DEC by David Chaiken.
Current maintainer is Mikhail Gusarov.


### Building on Arch

1. `git clone https://github.com/dottedmag/x2x; cd x2x`
2. `./bootstrap.sh`
3. `sudo pacman -S libxext libxtst`
4. `./configure`
5. `make && sudo make install`

If you want the simple solution, there is also a package in the [AUR](https://aur.archlinux.org/packages/x2x-git) for x2x.

###  Building on Fedora 

1. `git clone https://github.com/dottedmag/x2x; cd x2x`
2. `./bootstrap.sh`
3. `sudo dnf -y install libXext-devel libXtst-devel`
4. `./configure`
5. `make && sudo make install`

### Building on Ubuntu or Debian

1. `git clone https://github.com/dottedmag/x2x; cd x2x`
2. `git checkout debian`
3. `dpkg-checkbuilddeps` (and `sudo apt install` anything missing)
4. fakeroot debian/rules binary
5. `sudo dpkg --install ../x2x_VERSION.deb`
