# M5Stack CoreS3

## Features

- ✅ Power status
- ⚠️ SD card
- ⚠️ USB Storage

## Issues

(\*) SD card is currently not working once the display is in use. See [this](https://github.com/espressif/esp-bsp/blob/63b99593b7ead04336c0f22e7bc880167d9bfdb6/bsp/m5stack_core_s3/README.md)
and [this message](https://community.m5stack.com/post/21397). [According to a post online]((https://community.m5stack.com/topic/5415/core-s3-sd-tf-card-issues/2)),
this appears to be a hardware design error:

> (...) it looks like the TFT (which also uses SPI) uses MISO as DC. From an ESP32 perspective MISO is an input but DC needs to be an output. So the TFT driver configures the MISO GPIO to an output. This conflicts with the SD card, which is on the same SPI bus and requires MISO to be an input. Not sure how to resolve that so that TFT and SD card can coexist.

External I2C is currently not working because it's not getting power to the connector.

## Links

- [Official documentation](https://docs.m5stack.com/en/core/CoreS3)


