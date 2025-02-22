# Elecrow CrowPanel Basic 3.5"

⚠️ Tactility only supports hardware revision v2.2
⚠️ The rendering performance is degraded due to hardware and software limitations. A full screen refresh takes about 1 second, but Tactility is fully usable. Rendering updates for smaller areas on the screen perform significantly better.

## Features

- ✅ SD card
- ✅ External ports (UART and I2C)
- ⏳ Power status: hasn't been tested with a battery (battery capacity is estimated from battery voltage when present)

## Rendering Performance

The panel is wired via SPI, which allows for a pixel format of either 3 bits or 18 bits in size. 18 bits is the logical choice, but LVGL doesn't support it natively.
The display driver needs to keep a separate buffer to convert from 16 bit RGB565 format (LVGL buffer) to 18 bit RGB666 format (SPI buffer). This buffer also costs extra memory,
especially considering it's 3 bytes per pixel in size.

## Links

- [Elecrow product page](https://www.elecrow.com/esp32-display-3-5-inch-hmi-display-spi-tft-lcd-touch-screen.html)
- [Elecrow documentation](https://www.elecrow.com/wiki/esp32-display-352727-intelligent-touch-screen-wi-fi26ble-320480-hmi-display.html)

