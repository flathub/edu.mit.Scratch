# Scratch Flatpak

## Re-generating the sources

- Run `update-package-info.py` to read the scratch-desktop Git tag from the manifest and generate
  the latest asset sources & download the needed package\*.json files.
- Run:

    flatpak-node-generator.py npm scratch-desktop/package-lock.json -sPR scratch-\*/package-lock.json --electron-chromedriver 7.15 --electron-non-patented-ffmpeg

  afterwards to regenerate the npm package sources.
