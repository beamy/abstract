# beamy

### Project Abstract

Beamy is a cross platform framework that allows for the sending of text, files, and other signals from one device to another using Bluetooth LE technology.

Starting by targeting iOS and macOS devices, Beamy will expand onto Android and Windows platforms at some point in the near future.

### Anticipated APIs

I anticpate implementing the following APIs in development of this project:

- **Nearby Devices**: As beamy will rely on Bluetooth, it will be relient on surrounding devices having their Bluetooth enabled. I most liekly will implement optionalities to allow developers to filter devices by distance.

- **Sending Beams**: Of course, beamy will have an API for sending various signals across Bluetooth. These methods will all have callbacks for success, failure, etc. on the sender's device.

  - **Specific Device**: Using a Bluetooth ID, beamy will be able to send beams to specific devices in the nearby area.
  - **Broadcasts**: Beamy will also be able to send beams to all devices in the surrounding area/radius as dected by a `nearbyDevices` method.

- **Accepting Beams**: Beamy will also implement methods for accepting beams that will in turn tell the sender that the beam has been accepted.

- **Rejecting Beams**: Beamy will also implement methods for rejecting beams that will in turn tell the sender that the beam has been rejected.

### Goals

- [ ] Connect to devices across Bluetooth LE using existing APIs.
- [ ] Wrap around native APIs in order to send and receive beams cross platform.
- [ ] Start with iOS and macOS, but look to develop cross platform libraries.
- [ ] Start with sending plain text, but work up to sending photos/files.
- [ ] Send native device feedback (vibrations, etc.) from one device to another.
