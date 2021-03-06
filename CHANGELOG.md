# MTBBarcodeScanner CHANGELOG

## 1.7.1

Allow setting torchMode to On before scanner starts. (Thanks [felipowsky](https://github.com/felipowsky)!)

## 1.7.0

Added support for controlling the torch. (Thanks [felipowsky](https://github.com/felipowsky)!)

## 1.6.1

Bug Fixes:
- Removed duplicate method call

## 1.6.0

Bug Fixes:
- Further fixes for issue #25: focus issue

## 1.5.0

Bug Fixes:
- Fixed an issue with the auto focus range restriction and focus point incorrectly persisting. (Thanks [sebastianludwig](https://github.com/sebastianludwig)!). Read more [here](https://github.com/mikebuss/MTBBarcodeScanner/issues/25).

## 1.4.0

Enhancements:
- Scan codes from the front or back camera! Thanks to [lanbozhang](https://github.com/lanbozhang).

## 1.3.2

Enhancements:
- Use AVCaptureSessionPresetHigh for session preset for higher quality video. (Thanks [@rshevchuk](https://github.com/rshevchuk)!)

## 1.3.1

Bug Fixes:
- Removed CocoaPods build phases from test target to fix issue [#19](https://github.com/mikebuss/MTBBarcodeScanner/issues/19).

## 1.3.0

Enhancements:
- Added support for the following:
  - AVMetadataObjectTypeInterleaved2of5Code
  - AVMetadataObjectTypeITF14Code
  - AVMetadataObjectTypeDataMatrixCode
  
Thanks to [@hdoria](https://github.com/hdoria) for [bringing this](https://github.com/mikebuss/MTBBarcodeScanner/issues/15) to my attention!

## 1.2.0

Enhancements:
- The capture preview layer now inherits the corner radius of the previewView's layer. Thanks [@tupps](https://github.com/tupps)!

## 1.1.18

Enhancements:
- Removed `scanningIsAvailable` and `scanningIsAvailableAndAllowed` methods in favor of `requestCameraPermissionWithSuccess:`, which requests camera permission and returns the result in a block.

## 0.1.8

Enhancements:
- Added `scanningIsAvailableAndAllowed` and `scanningIsProhibited` methods. Thanks to [@MattLewin](https://github.com/MattLewin) for the fix!

## 0.1.7

Bug Fixes:
- Fixed issue with preview orientation when starting in landscape. Thanks to [@laptobbe](https://github.com/laptobbe) for the fix!

## 0.1.6

Bug Fixes:
- Updated `captureOrientationForInterfaceOrientation` to handle all cases, including the new `UIInterfaceOrientationUnknown`. Thanks to [@emilstahl](https://github.com/emilstahl) for the fix!
- Updated sample project to recommended settings for Xcode 6

## 0.1.5

Bug Fixes:
- `stopScanning` was not correctly discarding the existing session, causing a lock.
- Scanner now stops scanning on a background thread

Thanks to [@brandonschlenker](https://github.com/brandonschlenker) for the fix!

## 0.1.4

Bug Fixes:
- The logic to check for the unsupported type (`AVMetadataObjectTypeFace`) was inverted. Thanks to [@Dario848](https://github.com/Dario848) for the fix!

## 0.1.3

Bug Fixes:
- Fixed issue with setting auto range restriction and focus point of interest on older models of iPads

## 0.1.2

Version 0.1.2 adds improvements to documentation and formatting.

Demo Project Enhancements:
- Added Kiwi testing framework

## 0.1.1

Features:
- Allow calling of `stopScanning` if scanning is unavailable to the device to make everything a little cleaner

Bug Fixes:
- Fixed issue with podspec `source_files` attribute

## 0.1.0

Initial release.
