# Memlogger binaries
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/yvoinov/memlogger-binaries/blob/main/LICENSE)
## Installation

To install binary package, run over package archive:
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

## Usage

Using memlogger described [here](https://github.com/yvoinov/memlogger/blob/main/README.md).

Feel free to check [project wiki](https://github.com/yvoinov/memlogger/wiki).
