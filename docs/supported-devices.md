# Supported Devices

Any ESP32 device with a touchscreen should be able to run Tactility,
because LVGL is set up in a platform-agnostic manner.
Implementing drivers can take some effort, so Tactility provides support for several devices.

Predefined configurations are available for:

| Device                          | Screen&Touch | SD card | Power | Other       |
|---------------------------------|--------------|---------|-------|-------------|
| [LilyGo T-Deck Plus][tdeckplus] | ✅           | ✅      | ✅    | Keyboard    | 
| [LilyGo T-Deck][tdeck]          | ✅           | ✅      |       | Keyboard (1)| 
| [M5Stack Core2][m5stack]        | ✅           | ✅      | ✅    |             |
| [M5Stack CoreS3][m5stack]       | ✅           | ✅      | ✅    |             |
| Yellow Board 2432S024C (2)      | ✅           | ✅      |       |             |

- ✅: Capable and implemented
- ⏳: Capable but not yet implemented
- ❌: Not capable

(1) T-Deck (regular): When a battery is not present, the device sometimes fails to initialize touch. Disconnect the USB cable, wait 5 seconds and try again.
(2) Yellow Board: Only the capacitive version is supported. See AliExpress [here][2432s024c_1] and [here][2432s024c_2].

[tdeck]: https://www.lilygo.cc/products/t-deck
[tdeckplus]: https://lilygo.cc/products/t-deck-plus
[2432s024c_1]: https://www.aliexpress.com/item/1005005902429049.html
[2432s024c_2]: https://www.aliexpress.com/item/1005005865107357.html
[m5stack]: https://m5stack.com/
