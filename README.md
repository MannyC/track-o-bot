# Build Dependencies

* Qt 5.5
* (OS X) Sparkle
* (Windows) WinSparkle

## Mac OS X

```
brew install qt5
brew link qt5 --force
```

* Install [Sparkle](http://sparkle.andymatuschak.org/)
 * Move _Sparkle.framework_ to ``/Library/Frameworks``.

## Windows

* Install [Qt](http://qt-project.org/downloads)
 * I use the Qt libraries 5.5.0 for Windows VS 2012.
* Install [WinSparkle](https://github.com/vslavik/winsparkle)
 * Clone the repository and build the library, for example with VS 2012. The precompiled releases are ancient.

## GNU/Linux

* Install Qt5.5+ with your distribution package manager (apt, etc...)

You also need development packages for:

* qt5-base
* mesa
* xcb
* xcb-icccm

on Ubuntu this should install all required development packages:

```
sudo apt-get install build-essential qt5-default qtbase5-dev libxcb1-dev libxcb-icccm4-dev
```

# Build Instructions

```
qmake
make
```

The resulting binary can be found in the ``build`` subfolder.

# Install Instructions

```
sudo make install
```

Default install prefix is /usr/local. You can change it by adding PREFIX argument to qmake command eg:

```
qmake PREFIX=/usr
```

# Contributing

Feel free to submit pull requests, suggest new ideas and discuss issues. Track-o-Bot is about simplicity and usability. Only features which benefit all users will be considered.

# License

GNU Lesser General Public License (LGPL) Version 2.1.

See [LICENSE](LICENSE).

