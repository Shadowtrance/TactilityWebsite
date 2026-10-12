# Device page template

Copy the block below into `docs/devices/<vendor>-<model>.md` and remove the sections that don't apply.

## Conventions

- Status legend (also shown on `supported-devices.md`):
  - ✅ Supported
  - ⚠️ Partially supported or buggy (explain in Notes)
  - 🚧 Hardware is capable, but not yet implemented
  - ❌ Not supported (hardware limitation or no driver planned)
- Feature table rows are sorted by status: ✅, ⚠️, 🚧, ❌.
- Spelling: `LilyGO`, `M5Stack`, `Elecrow`, `Guition`, `Waveshare`, `Seeed Studio`, `Wi-Fi`, `USB Mass Storage`, `SD card`.
- Chip names in code formatting: `SX1262`, `ES8311`.
- Headings in sentence case: "Known issues", not "Known Issues".
- Warnings use Docsify alerts (`> [!WARNING]`, `> [!NOTE]`), not loose ⚠️ lines.
- Link labels: "Product page", "Official documentation", "Store", "GitHub", "Wiki". Add the variant name when there are multiple, e.g. "Store (Keyboard)".
- Known issues: one or two sentences on what is affected and what to do about it, then a link to the source.

## Template

```markdown
# <Vendor> <Model>

<One sentence describing the device.>

> [!WARNING]
> <Hardware caveats that affect everyone, e.g. unsupported revisions.>

## Hardware variants

- v1: <how to recognize it>
- v2: <how to recognize it>

## Feature support

| Feature | Status | Notes |
|-|-|-|
| SD card | ✅ | |
| Power status | 🚧 | |

## Usage notes

<Button mappings, keyboard shortcuts, flashing quirks.>

## Known issues

- <Issue>: <impact and workaround>. ([source](https://...))

## Links

- [Product page](https://...)
- [Official documentation](https://...)
```
