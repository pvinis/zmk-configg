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
| `settings_reset` | `settings_reset-nice_nano_v2-zmk.uf2` | Sofle only: flash to both halves if they stop pairing, then reflash the real firmware |

### BDN9:

- Use the firmware file with QMK Toolbox.
- Click the reset button at the bottom of the keyboard.
- Click the "Flash" button in QMK Toolbox.

### Aurora Corne:

- Connect each side of the keyboard using a cable.
- Double tap the reset button.
- Drop the correctly named firmware (left/right) to the new disc that appears to be mounted on the desktop.

### Sofle:

KeebMaker wireless Sofle (nice!nano v2, OLEDs, encoders, underglow). The config mirrors the vendor's
[KeebMaker/zmk-config](https://github.com/KeebMaker/zmk-config) settings; see `config/sofle.conf`.

- Connect each side of the keyboard using a cable.
- Double tap the reset button. The half mounts as a `NICENANO` drive.
- Drop the correctly named firmware (left/right) to the new disc that appears to be mounted on the desktop.
- If the halves stop pairing with each other, flash `settings_reset-nice_nano_v2-zmk.uf2` to both halves first, then the real firmware.
- If macOS won't reconnect after a reflash, forget the keyboard in Bluetooth settings and pair again.
- Live remapping: plug the left half in over USB and open [zmk.studio](https://zmk.studio/) in Chrome (Bluetooth transport doesn't work on macOS). Studio locking is disabled, so no unlock key is needed.
