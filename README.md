# practice

Svalboard typing practice at https://practice.svalboard.com.

This repository owns the independent GitHub Pages deployment. Application source is currently maintained on the `feat/svalbr-standalone` branch of [morganvenable/keybard](https://github.com/morganvenable/keybard/tree/feat/svalbr-standalone).

To release, dispatch `deploy.yml` with `ref` set to a full, published source commit SHA. The workflow tests and builds the standalone trainer, then publishes only `dist-svalbr`. It does not deploy Keybard or Overlay. Releasing a previous SHA rolls back the site. `/release.json` identifies the deployed source.

GitHub Pages uses Actions, the custom domain `practice.svalboard.com`, and enforced HTTPS. DNS is a CNAME to `svalboard.github.io`.
