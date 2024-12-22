# Change Log
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

## 1.2.0 - 2024-12-23
### Fixed
    - Canonical pcsx2 command (*nix systems are CASE SENSITIVE and most systems install pcsx2 as pcsx2 and not PCSX2)
    - inconsistent file naming
    - inconsistent comments
    - changed buffer from 512 to 4096 bytes to accomodate longer content paths
### Added
    - Added more canonical strings (e.g pcsx2-qt)
    - Added todo.md for tracking future additions
    - Ability to load PCSX2 without a game from retroarch

## 1.1.1 - 2017-06-18
### Fixed
    - Version number in .nfo file

## 1.1.0 - 2017-06-18
### Added
    - Dolphin 5 support of `dolphin-emu-nogui`
    - Update libretro.h
