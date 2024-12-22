# libretro-pcsx2-launcher

A fork of [PCSX2 Launcher](https://github.com/eduardomozart/libretro-pcsx2-launcher) (which itself is a fork of [Dolphin Launcher](https://github.com/robloach/libretro-dolphin-launcher)) that contains some modifications to enhance functionality on *nix (linux, really).

Current changes:

- respects more canonical binary strings
- easier to extend
- doesn't use special cases for launching flatpak simplifying the logic.
- corrected source code comments to correctly refer to PCSX2 and added some additional info in some cases
- corrected file names to refer to PCSX2

Future changes:
- see todo.md


Launch Sony PlayStation 2 games through [PCSX2](https://pcsx2.net/), directly from [RetroArch](http://www.libretro.com/).

![PCSX2 launcher screenshot](screenshot.png)

## Installation

1. Compile the core
  ``` bash
  git clone https://github.com/coldscientist/libretro-pcsx2-launcher.git
  cd libretro-pcsx2-launcher
  make
  ```

2. Copy the core file to the RetroArch cores directory
  ``` bash
  cp dolphin_launcher_libretro.so /usr/lib/libretro/pcsx2_launcher_libretro.so
  cp dolphin_launcher_libretro.info /usr/share/libretro/info/pcsx2_launcher_libretro.info
  ```

3. Make sure [PCSX2](https://pcsx2.net/) [is installed](https://pcsx2.net/download.html). You should be able to run at least one of the following commands:
  ``` bash
  pcsx2
  flatpak run net.pcsx2.PCSX2
  ```

## Usage

1. Scan Sony PlayStation 2 games in RetroArch

2. Launch the games directly from the RetroArch menu

3. Alternatively, you can run games through the command line
  ``` bash
  retroarch -L pcsx2_launcher_libretro.so Crash.iso
  ```

## Contributors

- [Rob Loach](http://github.com/robloach)
- [Alcaro](https://github.com/Alcaro)
- [Eduardo Mozart de Oliveira](https://github.com/coldscientist)
- [Andreas Björkman](https://github.com/TheBeardOfTruth)
