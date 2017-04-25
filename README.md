# Gregorio PKGBUILDs for the AUR

This repository provides files for building Gregorio from the [Arch User Repository](https://aur.archlinux.org).

## Packages

Two Gregorio packages are available:

- `gregorio` provides the latest [stable release](https://github.com/gregorio-project/gregorio/releases).
- `gregorio-git` builds from the `develop` branch of the [Gregorio Github repository](https://github.com/gregorio-project/gregorio/tree/develop).

## Usage

The easiest way to install packages from the AUR is to use an [AUR helper](https://wiki.archlinux.org/index.php/AUR_helpers). For example,

    $ yaourt -S gregorio

To install manually from this repository using [`makepkg`](https://wiki.archlinux.org/index.php/Makepkg):

    $ git clone https://github.com/gregorio-project/gregorio-aur.git
    $ cd gregorio-aur/gregorio
    $ makepkg -si

Replace `cd gregorio-aur/gregorio` above with `cd gregorio-aur/gregorio-git` to build the development package.

## Bugs

Please report bugs with Gregorio itself to the Gregorio [bug tracker](https://github.com/gregorio-project/gregorio/issues).

Problems with these packaging files can be left on the AUR ([gregorio](https://aur.archlinux.org/packages/gregorio/), [gregorio-git](https://aur.archlinux.org/packages/gregorio-git/)) or in the Github [bug tracker](https://github.com/gregorio-project/gregorio-aur/issues).

## Authors

### Current
- Br Anthony VanBerkum
- Br Elijah Schwab

### Past
- David Gippner
- Laércio de Sousa

## License

These files are released to the public domain. See the [Gregorio project](https://github.com/gregorio-project/gregorio/tree/master#license) for its license.

## Changelog

### 2017-04-25

#### Changed
- Removed `gregorio.install` for both packages. `texlive-bin` includes a hook for Pacman that does the same work.

### 2017-04-18

#### Changed
- PKGBUILD for `gregorio-git` upgraded to v5.0.1. This will build and install all three fonts.
- PKGBUILD for `gregorio` upgraded to v5.0.1. This will download and install all three fonts.

### 2016-09-25

#### Changed
- PKGBUILD for `gregorio` upgraded to v4.2.0.

### 2016-08-09

#### Changed
- Both PKGBUILDs updated for compatibility with TeX Live 2016.
- Build docs for `gregorio-git`.

### 2016-05-30

#### Changed
- PKGBUILD for `gregorio` upgraded to v4.1.4.

### 2016-05-28

#### Changed
- PKGBUILD for `gregorio` upgraded to v4.1.3.

### 2016-03-03

#### Changed
- PKGBUILD for `gregorio` upgraded to v4.1.0.
- PKGBUILD for `gregorio-git` upgraded to v4.1.0.

### 2016-01-06

#### Changed
- PKGBUILD for `gregorio` upgraded to v4.0.1.

### 2015-12-10

#### Changed
- PKGBUILD for `gregorio` upgraded to v4.0.0.

### 2015-07-06

#### Changed
- PKGBUILD for `gregorio` upgraded to v3.0.3.

### 2015-06-01

#### Changed
- PKGBUILD for `gregorio` upgraded to v3.0.2.

### 2015-05-15

#### Changed
- PKGBUILD for `gregorio` upgraded to v3.0.0.

### 2015-04-12

#### Added
- This README.md.

### 2015-04-06

#### Added
- PKGBUILD for `gregorio-git`.

#### Changed
- PKGBUILD for `gregorio` upgraded to v2.4.3.

#### Removed
- AUR package for `gregorio-svn`.
