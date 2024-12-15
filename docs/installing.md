# Installing

### Downloading

An official release is pending.

For now you can find some builds in GitHub, but they are only available for a few days or weeks after they were built:
- [Firmware builds](https://github.com/ByteWelder/Tactility/actions/workflows/build-firmware.yml)
- [SDK builds](https://github.com/ByteWelder/Tactility/actions/workflows/build-sdk.yml)

(scroll down to the bottom to find the zip files)

### Flashing

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

