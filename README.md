# autotools-playground

learn Autotools

> Autotools is composed of several tools: aclocal, autoconf, automake and others, belonging to two packages: Automake and Autoconf

## Prerequisites

```brew install automake```

## Build and Run

```sh
brew install automake
mkdir hello_world
cd hello_world
touch main.c
touch configure.ac
touch Makefile.am
aclocal
autoconf
automake --add-missing
./configure
make
./helloworld

# make distrubution .tar.gz
make dist

# test that the distribution tarball
make distcheck

# Use Makefile to install the program
make install
```

**Resources**

* [The magic behind configure, make, make install](https://robots.thoughtbot.com/the-magic-behind-configure-make-make-install)
* [Using Autotools](https://developer.gnome.org/anjuta-build-tutorial/stable/create-autotools.html.en)