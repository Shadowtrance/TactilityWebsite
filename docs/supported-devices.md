# Supported Devices

Any ESP32 device with a touchscreen should be able to run Tactility,
because LVGL is set up in a platform-agnostic manner.
Implementing drivers can take some effort, so Tactility provides support for several devices.

Predefined configurations are available for:

| Device                          | Screen&Touch | SD card | Power | Other    |
|---------------------------------|--------------|---------|-------|----------|
| [LilyGo T-Deck Plus][tdeckplus] | ✅            | ✅       | ⏳ | Keyboard | 
| [LilyGo T-Deck][tdeck]          | ✅            | ✅       |   | Keyboard | 
| [M5Stack Core2][m5stack]        | ✅            | ✅       | ✅ |          |
| [M5Stack CoreS3][m5stack]       | ✅            | ✅       | ✅ |          |
| Yellow Board 2432S024C (\*)     | ✅            | ✅       |   |          |

- ✅: Capable and implemented
- ⏳: Capable but not yet implemented
- ❌: Not capable
