## 0.1.0

### Changed
- Replaced React with preact compat, which means it's not compatible with
React anymore until they support declarative html attributes and properties

### Added
- Flow typing added
- Added automatic mirroring for webcam facing the user and cameras
that don't have info on where they are facing (mostly desktop ones)
- Added support iOS
- Added support for picking user/env facing

### Removed
- Prop types have been removed


## 0.0.20

### Changed
- height and width props now only apply to the getUserMedia constraints i.e. camera resolution. Setting the size of the video element should be done through CSS.

### Fixed
- Support Safari 11. Use video.srcObject rather than video.src

## 0.0.19

### Fixed
- Fix for firefox when requested resolution is higher than available resolution

### Removed
- Removed support for `navigator.getUserMedia`, only `navigator.mediaDevices.getUserMedia` is supported. This is due to too many inconsistencies in the `getUserMedia` api.


## 0.0.18

### Added
- Add onFailure callback for when the camera cannot be accessed.

### Changed
- Update to `mediaDevices.getUserMedia`.


## 0.0.17

### Changed
- `getUserMedia` and the video element are passed the width and height props of the component.
- `getCanvas` returns a canvas with the same size as the video element.
