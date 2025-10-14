# LilyGo T-Dongle S3

⚠️ This device implementation is incubating

The device is technically implemented, but there's currently no way to control it or put apps on it without forking the firmware and changing the code. Support for remote setup via Wi-Fi will be implemented at a later stage.

⚠️ The main limitation stems from the S3 chip not having PSRAM. This leaves 0 bytes of executable RAM (even when plenty of IRAM is available) because of the way that the S3 chip works. Further investigation is needed to figure out whether executable RAM can be pre-allocated.

## Features

- ✅ SD card
- ✅ USB Storage

## Links

- [Product page](https://lilygo.cc/products/t-dongle-s3)
- [Official GitHub project](https://github.com/Xinyuan-LilyGO/T-Dongle-S3/tree/main)
