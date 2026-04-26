# Pavlos' ZMK Config

### Setup

To flash bdn9, we need [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases)

### Flashing

- Download the latest firmware, by running:

```sh
hub api -H "Accept: application/vnd.github+json" /repos/pvinis/zmk-config-bdn9/actions/artifacts |jq ".artifacts[0].archive_download_url" | xargs hub api > firmware.zip
```

- Then just unzip, and use that file with QMK Toolbox.
- Click the reset button at the bottom of the keyboard.
- Click the "Flash" button in QMK Toolbox.
