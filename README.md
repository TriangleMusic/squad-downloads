# squad-downloads

The public home of the signed releases of Triangle Tools plugins, made with
the SQUAD community (https://www.triangle-squad.com). No code lives here:
every plugin's code is private.

- **Releases**: one GitHub release per product and version
  (`throw-v0.16.0`, `flash-warp-v0.3.18`), holding what the plugins' updaters
  download. Never replaced: a signed manifest names one file for good.
- **`updates/<product>.json`**: each product's signed update manifest. The
  plugins ask the Squad gateway once a day, and it answers from here, so a
  release is live without a site deploy. Each plugin checks the RSA
  signature, the size and the SHA-256 itself before installing anything.

Written only by the release scripts (`squad-core/Tools/release/manifest.sh`).
