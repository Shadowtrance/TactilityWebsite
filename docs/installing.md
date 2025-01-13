# Installing

You can install Tactility with the [Web Installer](https://install.tactility.one/). Installing with the _erase_ option is recommended.

Note, for **T-Deck**: You need to manually put the device in boot mode:
- Press the trackball and the reset button at the same time at the same time.
- When flashing is done, you might have to press the reset button.

Alternative methods are described below.

## Releases: Downloads

[Page with releases](https://github.com/ByteWelder/Tactility/releases)

## Releases: Manual Flashing

Make sure you have [esptool](https://docs.espressif.com/projects/esptool/en/latest/esp32/installation.html) installed.

Run the flash script:

**Linux / macOS**

Flash your serial device (often `ttyACM0` or `ttyUSB0`)

```bash
./flash.sh /dev/ttyACM0
```

**Windows**

Flash by specifying the `COM` port:

```ps
flash.ps COM3
```

## Development builds

You can find some builds in GitHub if you are logged in there, but they are only available for a few days or weeks after they were built:
- [Firmware builds](https://github.com/ByteWelder/Tactility/actions/workflows/build-firmware.yml)
- [SDK builds](https://github.com/ByteWelder/Tactility/actions/workflows/build-sdk.yml)

(scroll down to the bottom to find the zip files)

