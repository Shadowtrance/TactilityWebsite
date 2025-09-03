# FAQ

#### What is the purpose of Tactility?

The main purpose is to create an open source platform for tinkerers/hobbyists. The secondary purpose is to build something that is usable by end-users.

Tactility wants to offer a platform that can install on a wide range of ESP32 devices.

#### How is Tactility different/similar to other platforms?

- Tactility runs native apps without flashing them to ROM. You can compile a native binary and upload it via WiFi on the fly. This allows you to use device for various purposes while developing new projects or features. The workflow compares more to mobile phone app development and less to classic microcontroller development.
- Tactility provides a hardware abstraction layer that helps people write safe code (e.g. multi-threading).
- Tactility provides various system services for easy hardware access (e.g. connecting to WiFi via service and via a user interface).

The main downside to Tactility's approach is that its background services come with a performance overhead, which is mainly a memory cost. When Wi-Fi is connect and an SD card is present, there's less than 100 kB of RAM left for running apps. Luckily there are plenty of devices that provide an extra 8MB PSRAM on top of that.

Additionally, the user interface can be completely disabled by an app at runtime. This allows an app to free up the display buffers, and drive the display (and other devices) directly via a special driver model. Once the app quits, the system can resume normally.

#### How does this relate to Flipper Zero?

Initially, the project started as a [fork](https://github.com/KenVanHoeylandt/FlipperZeroEsp32) of Flipper Zero. Flipper Zero still serves as an inspiration, but so does Android, iOS and other platforms.
