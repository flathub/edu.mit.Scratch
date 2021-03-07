# Scratch Flatpak

## Re-generating the sources

- Run `update-package-info.py` to read the scratch-desktop Git tag from the manifest and generate
  the latest asset sources & download the needed package\*.json files.
- Run:

    flatpak-node-generator.py npm scratch-desktop/package-lock.json -PR scratch-\*/package-lock.json --node-chromedriver-from-electron 8.0.0 --electron-ffmpeg=lib --xdg-layout

  afterwards to regenerate the npm package sources.
