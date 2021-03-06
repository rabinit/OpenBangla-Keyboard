<p align="center">
<img src="https://github.com/OpenBangla/OpenBangla-Keyboard/raw/master/data/128.png">
</p>

**OpenBangla Keyboard** is an OpenSource, Unicode compliant Bengali Input Method for GNU/Linux systems. It's a full fledged Bengali input method with typing automation tools, includes many famous typing methods such as Avro Phonetic, Probhat, Munir Optima, National (Jatiya) etc.

Most of the features of [Avro Keyboard](https://www.omicronlab.com/avro-keyboard.html) are present in OpenBangla Keyboard. So Avro Keyboard users will feel at home with OpenBangla Keyboard in Linux.

[![Build Status](https://travis-ci.org/OpenBangla/OpenBangla-Keyboard.svg?branch=master)](https://travis-ci.org/OpenBangla/OpenBangla-Keyboard)
[![Downloads](https://img.shields.io/github/downloads/OpenBangla/OpenBangla-Keyboard/total.svg)](https://github.com/OpenBangla/OpenBangla-Keyboard/releases/latest)
[![Discord](https://img.shields.io/discord/436879388362014740.svg)](https://discord.gg/HXK7QnJ)

> This project is powered by github 🌟s ^ go ahead and [star it please](https://github.com/OpenBangla/OpenBangla-Keyboard/stargazers).

## Features
* Features Avro Keyboard like Top Bar for easy configuration.
* Phonetic Keyboard Layout (Avro Phonetic)
  - 100% compatibility with the current Avro Phonetic scheme.
  - Dictionary support can predict and suggest phonetically similar words with correct spelling on the fly.
  - Autocorrect support brings commonly used English words to Bangla (like, Facebook, download etc.) even with their original English spelling.
  - User can add and edit Autocorrect entries.
  - Support for preview window to see originally typed text right under the cursor.
* Fixed Keyboard Layout
  - OpenBangla Keyboard comes with Probhat, Munir Optima, Avro Easy, Bornona, National (Jatiya) keyboard layout out of the box.
  - OpenBangla Keyboard supports Avro Keyboard Layout file (version 5).
* Typing Automation tools for Fixed Keyboard layout
  - Automatic Vowel Forming.
  - Old Style “Reph”.
  - Traditional Kar Joining.
  - Automatic fixing of "Chandrabindu" position.
* Layout Viewer

## Installing
> If you had installed OpenBangla Keyboard 1.2.0 or earlier version, please uninstall it first.
### Ubuntu
OpenBangla Keyboard supports Ubuntu 16.04 LTS, 17.10 and 18.04 LTS version. Install OpenBangla Keyboard on your system by running the following commands:
```bash
$ curl -s https://packagecloud.io/install/repositories/mominul/OpenBangla/script.deb.sh | sudo bash
$ sudo apt install openbangla-keyboard
```
After the installation completes, you have to log out from your session. If your Ubuntu version is 17.04 or earlier visit [Configure on Unity DE](https://github.com/OpenBangla/OpenBangla-Keyboard/wiki/Configure-on-Unity-DE) otherwise visit [Configure on Gnome DE](https://github.com/OpenBangla/OpenBangla-Keyboard/wiki/Configure-on-Gnome-DE).
### Fedora
OpenBangla Keyboard supports Fedora 27 version. Install OpenBangla Keyboard on your system by running the following commands:
```bash
$ curl -s https://packagecloud.io/install/repositories/mominul/OpenBangla/script.rpm.sh | sudo bash
$ sudo dnf install openbangla-keyboard
```
After the installation completes, you have to log out from your session. You will need to [configure Gnome DE](https://github.com/OpenBangla/OpenBangla-Keyboard/wiki/Configure-on-Gnome-DE) for OpenBangla Keyboard to work.
### Other
Linux packages can be downloaded from [here](https://github.com/OpenBangla/OpenBangla-Keyboard/releases)

If you need help, there is a wiki [page](https://github.com/OpenBangla/OpenBangla-Keyboard/wiki/Installing-OpenBangla-Keyboard)

## Compiling on GNU/Linux
### Build & Install procedures
OpenBangla Keyboard currently needs following libraries and binaries
* GNU GCC, G++ compiler or Clang
* GNU Make or Ninja
* CMake
* Qt 5.5 or later
* iBus development library

On a Ubuntu/Debian system you can easily install them like this
```
sudo apt-get install build-essential cmake libibus-1.0-dev qt5-default
```

On a Fedora system you can easily install them like this
```
sudo dnf install @buildsys-build cmake qt5-qtdeclarative-devel ibus-devel
```
On a Arch Linux / Arch Based system you can easily install them like this
```
sudo pacman -Sy base-devel cmake qt5-base libibus
```

After you have installed required libraries and binaries. Clone this repository and change the directory to the cloned folder and issue the commands:
```
mkdir build && cd build
cmake ..
make
sudo make install
```

Use iBus UI or run `ibus-setup` to add **OpenBangla Keyboard**. To get help on configuring OpenBangla Keyboard, visit [Configure on Gnome DE](https://github.com/OpenBangla/OpenBangla-Keyboard/wiki/Configure-on-Gnome-DE) or [Configure on Unity DE](https://github.com/OpenBangla/OpenBangla-Keyboard/wiki/Configure-on-Unity-DE).

## Acknowledgements
 - Mehdi Hasan Khan for originally developing and maintaining Avro Keyboard,
 - Rifat Nabi for porting Avro Phonetic to Javascript,
 - [Sarim Khan](https://github.com/sarim) for writing ibus-avro.

## License
Licensed under [GPL 3 Licence](https://opensource.org/licenses/GPL-3.0).

Made with ❤️ by [Muhammad Mominul Huque](https://github.com/mominul).