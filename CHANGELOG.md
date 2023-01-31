# Changelog

**Attention**
The project is now completely stable and matches the real hardware. If you have any problems, you are probably doing something wrong!<br>
The [documentation](README.md) is very useful for troubleshooting in case of failures!<br>


## 2.9.0 - Jan 31, 2023

### Added

- First Wifi Pineapple Cloner v4 release
- Add config.php for config panel after flash
- Other minor changes in panel

### Fixed

- Fix wifi card detection
- Fix duplicate requests
- Fix airmon-ng card detection


## 2.8.5 - Oct 28, 2022

### Added

- Update panel vendor dependencies 
- Add complete-setup service for control dependencies and other problems
- Added busybox custom build to improve firmware size
- A workaround has been added for routers that do not have a reset button but have a wps button
- Other minor changes in panel views
- Other minor changes in build and logic

### Fixed

- Fix board detection logic for auto updater
- Fix Network missing request
- Fix logic in onDeviceIdentified fault logic


## 2.8.4 - Oct 18, 2022

### Fixed

- Fix angular bug in updater view


## 2.8.3 - Oct 17, 2022

### Fixed

- Fix setup after reflash


## 2.8.2 - Oct 17, 2022

### Fixed

- Fix ModuleManager installer


## 2.8.1 - Oct 17, 2022

### Fixed

- Fix logic in updater view
- Other minor changes


## 2.8.0 - Oct 17, 2022

### Added

- First Wifi Pineapple Cloner v3 release
- Add MIPSEL support
- Identified 211 supported devices (real list could exceed 300)
- Unified all updatable material in a single repository (modules, packages, oui data, etc)
- Support for automatic updates
- Initial changes for reflash support
- Other minor changes

### Fixed

- Fix switch support broken in WPC v2

