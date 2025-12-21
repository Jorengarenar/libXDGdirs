libXDGdirs
==========

An implementation of [XDG Base Directory Specification](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html)

_XDGBDS_ defines four categories of dotfiles and the corresponding directories
in user's home directory that should be used for those. The categories are
cache, configuration, data, state and runtime files.

All those locations have corresponding `XDG_*` environment variables.

All paths set in them must be absolute.  
If a relative path is encountered, the path is considered invalid and `NULL` is assigned.

## Build

### Download

Download the latest version from [release page](https://github.com/Jorenar/libXDGdirs/releases)
or clone Git repository for latest:
```sh
git clone https://github.com/Jorenar/libXDGdirs.git
cd libXDGdirs
```

### Build
```sh
cmake -B build/ -DCMAKE_BUILD_TYPE=Release
cmake --build build/ --config=Release
```

### Install
```sh
cmake --install build/
```

## Documentation

[Documentation](https://jorenar.github.io/libXDGdirs) generated from **latest commit** using [Doxygen](https://www.doxygen.nl)

## Usage

Refer to [topics](https://jorenar.github.io/libXDGdirs/topics.html)
and [examples](https://jorenar.github.io/libXDGdirs/examples.html)
in [documentation](https://jorenar.github.io/libXDGdirs)

## Read more

* [XDG Base Directory Specification](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html)
* [XDG Base Directory - ArchWiki](https://wiki.archlinux.org/index.php/XDG_Base_Directory)
* [XDGBaseDirectorySpecification - Debian Wiki](https://wiki.debian.org/XDGBaseDirectorySpecification)
