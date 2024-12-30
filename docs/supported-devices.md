# Supported Devices

Any ESP32 device with a touchscreen should be able to run Tactility,
because LVGL is set up in a platform-agnostic manner.
Implementing drivers can take some effort, so Tactility provides support for several devices.

Predefined configurations are available for:

| Device                          | Screen&Touch | SD card | Power | Other       |
|---------------------------------|--------------|---------|-------|-------------|
| [LilyGo T-Deck Plus][tdeckplus] | ✅           | ✅      | ✅    | Keyboard    | 
| [LilyGo T-Deck][tdeck] (1)      | ✅           | ✅      |       | Keyboard    | 
| [M5Stack Core2][m5stack] (2)    | ✅           | ✅      | ✅    |             |
| [M5Stack CoreS3][m5stack]       | ✅           | ✅      | ✅    |             |
| Yellow Board 2432S024C (3)      | ✅           | ✅      |       |             |

✅: Capable and implemented<br/>
⏳: Capable but not yet implemented<br/>
❌: Not capable<br/>

(1) T-Deck (regular): When a battery is not present, the device sometimes fails to initialize touch. Disconnect the USB cable, wait 5 seconds and try again.<br/>
(2) M5Stack Core2: Only the [original](https://docs.m5stack.com/en/core/Core2) version is currently supported ([v1.1](https://docs.m5stack.com/en/core/Core2%20v1.1) is not).<br/>
(3) Yellow Board: Only the capacitive version is supported. See AliExpress [here][2432s024c_1] and [here][2432s024c_2].<br/>

[tdeck]: https://www.lilygo.cc/products/t-deck
[tdeckplus]: https://lilygo.cc/products/t-deck-plus
[2432s024c_1]: https://www.aliexpress.com/item/1005005902429049.html
[2432s024c_2]: https://www.aliexpress.com/item/1005005865107357.html
[m5stack]: https://m5stack.com/
