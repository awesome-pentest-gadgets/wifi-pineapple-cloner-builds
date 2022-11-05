# Changelog

**Attention**
The documentation is very useful for troubleshooting in case of failures!<br>
The project is already completely stable so it's the same as the real hardware, so if you have a problem you're probably doing something wrong!


## 2.8.5 - Oct 28, 2022

### Added

- Update panel vendor dependencies 
- Add complete-setup service for control dependencies and other problems
- Added busybox custom build to improve firmware size
- Added workaround for routers that don't have a reset button but wps
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

- Add MIPSEL support
- Identified 211 supported devices (real list could exceed 300)
- Unified all updatable material in a single repository (modules, packages, oui data, etc)
- Support for automatic updates
- Initial support for reflash support
- Other minor changes

### Fixed

- Fix switch support broken in WPC v2

