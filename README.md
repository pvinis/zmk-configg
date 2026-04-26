# Pavlos' ZMK Config

## Keyboards

- BDN9
- Aurora Corne

## Setup

To flash BDN9, we need [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases)

## Flashing

- Download the latest firmware, by running:

```sh
hub api -H "Accept: application/vnd.github+json" /repos/pvinis/zmk-config-bdn9/actions/artifacts |jq ".artifacts[0].archive_download_url" | xargs hub api > firmware.zip
```


### BDN9:

- Then just unzip, and use that file with QMK Toolbox.
- Click the reset button at the bottom of the keyboard.
- Click the "Flash" button in QMK Toolbox.

### Aurora Corne:

[![.github/workflows/build.yml](https://github.com/pvinis/zmk-config-corne/actions/workflows/build.yml/badge.svg)](https://github.com/pvinis/zmk-config-corne/actions/workflows/build.yml)

- Then just unzip.
- Connect each side of the keyboard using a cable.
- Double tap the reset button.
- Drop the correctly named firmware (left/right) to the new disc that appears to be mounted on the desktop.
