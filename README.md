# Sami TV for TizenBrew

This is an **experimental TizenBrew application module**, not an installable WGT file.

## Contents
- `package.json`: TizenBrew app-module metadata
- `app/`: Sami TV HTML, CSS, JS, and icon (offline UI; network needed for weather and prayer data)

## Deployment
1. Install a TizenBrew build compatible with your Samsung TV. Samsung 2018 is typically Tizen 4.x; compatibility must be verified.
2. Host the contents of this folder in a GitHub repository (at the repository root) or a supported NPM module repository.
3. Inside TizenBrew's module manager, add the published module by its GitHub repository or supported package identifier, then launch Sami TV.

TizenBrew modules are hosted as application content and do not require Sami TV's own WGT signature. However, TizenBrew itself must already be successfully installed and may be rejected by the TV if its signature is incompatible.

Weather, prayer and system app launching are unverified on real device. The TizenBrew environment may not expose the same Tizen APIs to an application module, so installed-app discovery and shortcuts can be limited. This is not a firmware/home-screen replacement.

Reference: https://github.com/reisxd/TizenBrew/blob/main/docs/MODULES.md
