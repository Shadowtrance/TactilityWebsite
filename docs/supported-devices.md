# Supported Devices

Any ESP32 device with a touchscreen should be able to run Tactility,
because drivers can be implemented for any hardware.
Implementing drivers can take some effort, so Tactility provides support for several devices.

The currently recommended hardware are the `LilyGo T-Deck` variants due to their keyboard and larger display.

Predefined configurations are available for:

| Device                          | SD card | Power | USB storage | Other     |
|---------------------------------|---------|-------|-------------|-----------|
| [LilyGo T-Deck Plus][tdeckplus] | ✅      | ✅    | ✅          | Keyboard  | 
| [LilyGo T-Deck][tdeck] (1)      | ✅      | ✅    | ✅          | Keyboard  | 
| [M5Stack Core2][m5stack] (2)    | ✅      | ✅    | ❌          |           |
| [M5Stack CoreS3][m5stack]       | ✅ (4)  | ✅    | ✅ (4)      |           |
| Yellow Board<br/>2432S024C (3)  | ✅      | ⏳    | ❌          |           |

✅: Capable and implemented<br/>
⏳: Capable but not yet implemented<br/>
❌: Not capable<br/>

(1) T-Deck (regular): When a battery is not present, the device sometimes fails to initialize touch. Disconnect the USB cable, wait 5 seconds and try again.<br/>
(2) M5Stack Core2: Only the [original](https://docs.m5stack.com/en/core/Core2) version is currently supported ([v1.1](https://docs.m5stack.com/en/core/Core2%20v1.1) is not).<br/>
(3) Yellow Board: Only the capacitive version is supported. See AliExpress [here][2432s024c_1] and [here][2432s024c_2].<br/>
(4) Currently not working. See [this message](https://github.com/espressif/esp-bsp/blob/63b99593b7ead04336c0f22e7bc880167d9bfdb6/bsp/m5stack_core_s3/README.md).

[tdeck]: https://www.lilygo.cc/products/t-deck
[tdeckplus]: https://lilygo.cc/products/t-deck-plus
[2432s024c_1]: https://www.aliexpress.com/item/1005005902429049.html
[2432s024c_2]: https://www.aliexpress.com/item/1005005865107357.html
[m5stack]: https://m5stack.com/
