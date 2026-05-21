# Pavlos' ZMK Configg

[![Build](https://github.com/pvinis/zmk-configg/actions/workflows/build.yml/badge.svg)](https://github.com/pvinis/zmk-configg/actions/workflows/build.yml)

## Keyboards

- BDN9
- Aurora Corne
- Sofle

## Setup

To flash BDN9, we need [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases)

## Flashing

- Download the latest firmware, by running:

```sh
gh run download -R pvinis/zmk-configg -n firmware -D firmware
```

or

```sh
zmk download
```

| Keyboard | Firmware artifact | Flashing method |
| --- | --- | --- |
| `bdn9_rev2` | `bdn9_rev2-zmk.bin` | Flash with QMK Toolbox |
| `splitkb_aurora_corne_left` | `splitkb_aurora_corne_left-nice_nano_v2-zmk.uf2` | Copy to the mounted bootloader drive |
| `splitkb_aurora_corne_right` | `splitkb_aurora_corne_right-nice_nano_v2-zmk.uf2` | Copy to the mounted bootloader drive |
| `sofle_left nice_oled` | `sofle_left-nice_nano_v2-zmk.uf2` | Copy to the mounted bootloader drive |
| `sofle_right nice_oled` | `sofle_right-nice_nano_v2-zmk.uf2` | Copy to the mounted bootloader drive |

### BDN9:

- Use the firmware file with QMK Toolbox.
- Click the reset button at the bottom of the keyboard.
- Click the "Flash" button in QMK Toolbox.

### Aurora Corne:

- Connect each side of the keyboard using a cable.
- Double tap the reset button.
- Drop the correctly named firmware (left/right) to the new disc that appears to be mounted on the desktop.

### Sofle:

- Connect each side of the keyboard using a cable.
- Double tap the reset button.
- Drop the correctly named firmware (left/right) to the new disc that appears to be mounted on the desktop.
