# Building Tactility

## Cloning from git

Ensure you clone the repository including the submodules! For example:

```bash
git clone --recurse-submodules -j8 https://github.com/ByteWelder/Tactility.git
```

## Build environment setup

Ensure you have [esp-idf 5.3](https://docs.espressif.com/projects/esp-idf/en/release-v5.3/esp32/get-started/index.html) installed.

## Build an ESP32 variant

Run this:

```bash
Buildscripts/build.sh <board-name>
```

`<board_name>` is the the last part of the names of the boards in `./sdkconfig.board.<board-name>`.

For example:

```bash
Buildscripts/build.sh lilygo-tdeck
```

## Build the simulator

Ensure you do **not** have esp-idf on your path and run:

```bash
idf.py build
```

## Building ESP32 manually

Copy the `sdkconfig.board.YOUR_BOARD` into `sdkconfig`. Use `sdkconfig.defaults` if you are setting up a custom board.

```bash
cp sdkconfig.board.<board-name>
idf.py build
```

Flashing ESP32:

```bash
idf.py flash monitor
```

