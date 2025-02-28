# Memlogger binaries
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/yvoinov/memlogger-binaries/blob/main/LICENSE)
## Installation and removal

### Installation from binary tarball

To install from binary tarball, run over archive:
```sh
gzcat memlogger*.gz|tar xvf - -C /
```
or (some Linux)
```sh
zcat memlogger*.gz|tar xvf - -C /
```

Library will be installed under /usr/local/lib. Runtime libraries will installed same path.

Usually package contains both 32 and 64 bit version library:

/usr/local/lib/libmemlogger.so

and

/usr/local/lib/64/libmemlogger.so

**Note**: On Solaris 11, the shipped tar does not allow unpacking to a specified directory. To unpack, you need to extract the files to the current directory and then move them with the mvdir command:

```sh
gunzip memlogger*.gz && tar -xvf *.tar
mvdir usr/local /usr/local
```

To remove, run the commands:

find /usr/local -name libmemlogger* -exec sudo rm -Rf {} \;

### Installation from packages

*Arch Linux*

Installation :
```sh
pacman -U memlogger-*.pkg.tar.zst
```

Removal (example; bit depth may vary):
```sh
pacman -Rs memlogger-x86_64
```

*Deb packages*

Installation:
```sh
dpkg -i memlogger-*.deb
```

Removal (example; name is the package file name):
```sh
apt remove memlogger-2.2.0-Linux-Debian11-amd64.deb
```

*Rpm packages*

Installation (syntax is the same for dnf/yum):
```sh
dnf install memlogger-*.rpm
```

Removal:
```sh
dnf remove memlogger
```

*Solaris SVR4 Packages*

Installation:
```sh
unzip TCW*.zip && pkgadd -d TCW*.pkg
```

Removal:
```sh
pkgrm TCWmemlogger
```

*FreeBSD*

Installation:
```sh
pkg install memlogger-*.pkg
```

Removal:
```sh
pkg remove memlogger
```

## Usage

Using memlogger described [here](https://github.com/yvoinov/memlogger/blob/main/README.md).

Feel free to check [project wiki](https://github.com/yvoinov/memlogger/wiki).
