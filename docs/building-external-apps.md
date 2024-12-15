# External Apps

An example app can be found in the cmain repository in the [ExternalApps](https://github.com/ByteWelder/Tactility/tree/main/ExternalApps) folder.
The projects in this folder are standalone projects. They output an `.app.elf` file. 

## Get the SDK

There are 2 methods for getting the SDK:
1. Building it from within the Tactility project.
2. Downloading it from GitHub.

### Method 1: Build from Tactility

During Tactility OS development, we use this method.

1. Ensure the project is built for your target. (`idf.py build`)
2. Run `Buildscripts/release-sdk-current.sh`
3. Your SDK is now available at `release/TactilitySDK`

### Method 2: Downloading

Currently not actively supported. However, you can find build artifacts on GitHub (they expire after 5 days) and download them.
The provided zipfiles can be deployed anywhere.

When you compile one of the `ExternalApps` projects, make sure that `TACTILITY_SDK_PATH` environment variable is set to the SDK path.


