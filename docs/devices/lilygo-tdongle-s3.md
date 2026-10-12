# LilyGO T-Dongle S3

> [!NOTE]
> Support for this device is incubating. It runs Tactility, but there's currently no way to control it or install apps without forking the firmware and changing the code. Remote setup via Wi-Fi is planned.

## Feature support

| Feature | Status | Notes |
|-|-|-|
| SD card | ✅ | |
| USB Mass Storage | ✅ | |
| Bluetooth | ✅ | BLE |
| Backlight control | ✅ | Brightness control |
| Touch | ❌ | No touchscreen |

## Known issues

- Memory: the ESP32-S3 on this board has no PSRAM. Because of how the S3 works, this leaves 0 bytes of executable RAM, even when plenty of IRAM is free. It is still being investigated whether executable RAM can be pre-allocated.

## Links

- [Product page](https://lilygo.cc/products/t-dongle-s3)
- [GitHub](https://github.com/Xinyuan-LilyGO/T-Dongle-S3/tree/main)
