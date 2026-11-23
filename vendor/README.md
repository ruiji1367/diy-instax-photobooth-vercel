# Vendored WebBLE bridge

`webble.js` is the browser bundle from `@beacio/core@2.2.0`
(`dist/browser-auto.global.js`), MIT licensed, Copyright (c) 2025 wklm.
License text: `LICENSE.beacio.txt`.

- Source package: https://www.npmjs.com/package/@beacio/core
- Project: https://github.com/wklm/ioswebble-sdk
- App: WebBLE (ioswebble) Safari Web Extension

The bundle installs a `navigator.bluetooth` polyfill that maps to the WebBLE
Safari extension on iPadOS. The Printer Lab loads it only when the operator
turns the bridge toggle on.

The older `https://ioswebble.com/webble.js` URL returned 404 on 2026-11-12, so
the current npm browser bundle is vendored instead. Re-vendor from the package
when the extension or SDK updates, and keep `LICENSE.beacio.txt` alongside it.

The bridge requires the WebBLE extension to be installed and enabled. Whether
it works on iPad is UNVERIFIED until Phase B of
`docs/printer-testing/TEST-PLAN.md` runs.
