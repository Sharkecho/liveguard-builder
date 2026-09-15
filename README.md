# LiveGuard Builder

Public build-only repository for the R5S OpenWrt baseline and the minimal LiveGuard package skeleton.

This repository intentionally contains no LiveGuard core algorithms, credentials, VPS settings, device configuration, or deployment logic.

Artifacts are build outputs only. The workflow never connects to or deploys to a VPS, router, or phone.

## Build modes

- `Build R5S baseline` is the infrequent full image build. Use it only when the
  OpenWrt target, kernel, device tree, or base configuration changes.
- `Build LiveGuard package` compiles only the package against a matching R5S
  SDK and uploads the package, manifest, and SHA256 file. It does not rebuild
  the firmware image and does not deploy anywhere.
