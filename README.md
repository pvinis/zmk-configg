# Pavlos' ZMK Config

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
