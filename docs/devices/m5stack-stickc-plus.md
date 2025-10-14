# M5Stack StickC Plus

⚠️ This device implementation is incubating

The device is technically implemented, but there's currently no way to control it or put apps on it without forking the firmware and changing the code. Support for remote setup via Wi-Fi will be implemented at a later stage.

There is an issue with the display flickering when it updates. It's unclear what the cause is, but I'm suspecting the display driver as I investigated the AXP192 a lot already.

⚠️  Must flash at one of these baud rates: 1500000, 750000, 500000, 250000, 115200 bps

## Features

- ✅ Power status

## Links

- [Official documentation](https://docs.m5stack.com/en/core/m5stickc_plus)
- [Official store](https://shop.m5stack.com/products/m5stickc-plus-esp32-pico-mini-iot-development-kit)
- [AXP192 details](https://github.com/m5stack/M5Unified/blob/5580ff6923a868cc71d5b30c962186bde2c85b67/README.md)
