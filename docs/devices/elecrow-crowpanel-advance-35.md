# Elecrow CrowPanel Advance 3.5"

⚠️ The rendering performance is degraded due to hardware and software limitations. A full screen refresh takes a bit less than half a second. Rendering updates for smaller areas on the screen perform significantly better.

## Features

- ✅ SD card
- ✅ External ports (UART and I2C)
- ⚠️ USB Mass Storage: capable, but TinyUSB crashes upon disconnect. It might work when using a battery and disconnecting the USB port after the reboot, but this is untested.

## Rendering Performance

The panel is wired via SPI, which allows for a pixel format of either 3 bits or 18 bits in size. 18 bits is the logical choice, but LVGL doesn't support it natively.
The display driver needs to keep a separate buffer to convert from 16 bit RGB565 format (LVGL buffer) to 18 bit RGB666 format (SPI buffer). This buffer also costs extra memory,
especially considering it's 3 bytes per pixel in size.

## Links

- [Elecrow product page](https://www.elecrow.com/crowpanel-advance-3-5-hmi-esp32-ai-display-480x320-artificial-intelligent-ips-touch-screen.html)
- [Elecrow documentation](https://www.elecrow.com/pub/wiki/CrowPanel_Advance_3.5-HMI_ESP32_AI_Display.html)
- [Elecrow GitHub project](https://github.com/Elecrow-RD/CrowPanel-Advance-HMI-ESP32-AI-Display)

