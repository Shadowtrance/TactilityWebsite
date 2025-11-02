# Supported Devices

Any ESP32 device should be able to run Tactility, because drivers can be implemented for any hardware.
Some hardware combinations are officially supported.

Recommendations:
- LilyGO: [LilyGo T-Deck Plus](devices/lilygo-tdeck-plus.md) is currently the best-supported device: all features are working and performance is great.
- Elecrow: [CrowPanel Advance 2.8"](devices/elecrow-crowpanel-advance-28.md): This device also has great performance. It offers an extra USB UART and several external ports.
- M5Stack: [Core2](devices/m5stack-core2.md) is recommended.

|Name|Memory|SD card|ROM|Ext|
|-|-|-|-|-|
|[CYD 2432S024C](devices/cyd-2432s024c.md)|🟧|🟩|4 MB|🟩|
|[CYD 2432S028R](devices/cyd-2432s028r.md)|🟧|🟩|4 MB|🟩|
|[CYD 2432S028R v3](devices/cyd-2432s028rv3.md)|🟧|🟩|4 MB|🟩|
|[CYD 2432S032C](devices/cyd-2432s032c.md)|🟧|🟩|4 MB|🟩|
|[CYD 4848S040C](devices/cyd-4848s040c.md)|🟩|🟥|16 MB|🟥|
|[CYD 8048S043C](devices/cyd-8048s043c.md)(\*)|🟩|🟩|16 MB|🟥|
|[CYD E32R28T](devices/cyd-e32r28t.md)(\*)|🟧|🟩|4 MB|🟩|
|[CYD E32R28T](devices/cyd-e32r32p.md)(\*)|🟧|🟩|4 MB|🟩|
|[CYD JC2432W328C](devices/cyd-jc2432w328c.md)(\*)|🟧|🟩|4 MB|🟩|
|[CYD JC8048W550C](devices/cyd-jc8048w550c.md)(\*)|🟩|🟩|16 MB|🟥|
|[Elecrow CrowPanel Advance 2.8"](devices/elecrow-crowpanel-advance-28.md)|🟩|🟩|16 MB|🟩|
|[Elecrow CrowPanel Advance 3.5"](devices/elecrow-crowpanel-advance-35.md)|🟩|🟩|16 MB|🟩|
|[Elecrow CrowPanel Advance 5.0"](devices/elecrow-crowpanel-advance-50.md)|🟩|🟩|16 MB|🟥|
|[Elecrow CrowPanel Basic 2.8"](devices/elecrow-crowpanel-basic-28.md)|🟧|🟩|4 MB|🟩|
|[Elecrow CrowPanel Basic 3.5"](devices/elecrow-crowpanel-basic-35.md)|🟧|🟩|4 MB|🟩|
|[Elecrow CrowPanel Basic 5.0"](devices/elecrow-crowpanel-basic-50.md)|🟩|🟩|4 MB|🟥|
|[LilyGo T-Deck](devices/lilygo-tdeck.md)|🟩|🟩|16 MB|🟩|
|[LilyGo T-Deck Plus](devices/lilygo-tdeck-plus.md)|🟩|🟩|16 MB|🟩|
|[LilyGo T-Lora Pager](devices/lilygo-tlora-pager.md)|🟩|🟩|16 MB|🟩|
|[M5Stack Cardputer](devices/m5stack-cardputer.md)|🟧|🟩|8 MB|🟩|
|[M5Stack Cardputer Adv](devices/m5stack-cardputer-adv.md)|🟧|🟩|8 MB|🟩|
|[M5Stack Core2](devices/m5stack-core2.md)|🟩|🟩|16 MB|🟩|
|[M5Stack CoreS3](devices/m5stack-cores3.md)|🟩|🟥|16 MB|🟩|
|[unPhone](devices/unphone.md)|🟩|🟩|8 MB|🟩|
|[Waveshare ESP32 S3 Touch LCD 4.3"](devices/waveshare-s3-touch-lcd-43.md)|🟩|🟥|4 MB|🟥|
|[BigTreeTech Panda Touch K Touch](devices/btt-panda-touch.md)(\*)|🟩|🟥|16 MB|🟥|

Incubating:

|Name|Memory|SD card|ROM|Ext|
|-|-|-|-|-|
|[LilyGo T-Display S3](devices/lilygo-tdisplay-s3.md)|🟩|🟩|16 MB|🟩|
|[LilyGo T-Dongle S3](devices/lilygo-tdongle-s3.md)|🟧|🟩|16 MB|🟩|
|[LilyGo T-Display](devices/lilygo-tdisplay.md))(\*)|🟧|🟧|16 MB|🟩|
|[M5Stack StickC Plus](devices/m5stack-stickc-plus.md)|🟧|🟥|4 MB|🟩|
|[M5Stack StickC Plus2](devices/m5stack-stickc-plus2.md)|🟩|🟥|8 MB|🟩|
|[Waveshare ESP32 S3 LCD 1.3"](devices/waveshare-s3-lcd-13.md)|🟩|🟩|16 MB|🟥|
|[Waveshare ESP32 S3 Touch LCD 1.28"](devices/waveshare-s3-touch-lcd-128.md)|🟩|🟩|16 MB|🟥|
|[Waveshare ESP32 S3 Touch LCD 1.47"](devices/waveshare-s3-touch-lcd-147.md)|🟩|🟩|16 MB|🟥|


Memory: 🟧 = no external RAM, 🟩 = external RAM present

SD card: 🟩 = working, 🟥 = unavailable/broken/not implemented

ROM: System storage size. This allows for a larger `/data` partition which stores configuration and other mutable data.

Ext: This stands for "extended features". If available, it allows apps to directly control display and touch devices. Currently unavailable for RGB/i80 displays.

 (\*) These boards are not owned by the developer, so quality control is limited to community efforts.
