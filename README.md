# Music

![Version](https://img.shields.io/github/v/tag/openblock-plugin/music?label=version)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Type](https://img.shields.io/badge/type-extension-orange.svg)
![Tags](https://img.shields.io/badge/tags-scratch-lightgrey.svg)

Play instruments and drums.

## Documentation

For detailed usage instructions, please visit:

**[OpenBlock Wiki](https://wiki.openblock.cc)**

## Asset Manifest Generation

This plugin bundles all instrument and drum MP3 files at build time. When the
contents of `assets/sounds/` change, regenerate the manifest:

```
npm run gen-manifest
```

The generation script writes a self-contained `src/manifest.js` that base64-encodes
every audio file. `npm run build` automatically runs the generator first.
