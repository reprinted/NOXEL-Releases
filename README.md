# NOXEL — Official Releases

**NOXEL** is a Windows display-management utility for resolutions, refresh rates, supported color controls, and saved presets.

This repository is the **public binary-distribution channel**. The source code is published at [reprinted/NOXEL](https://github.com/reprinted/NOXEL); every release here links to the matching source tag (for example `v1.0.0`).

## Downloads

Get the latest version from the [Releases page](https://github.com/reprinted/NOXEL-Releases/releases/latest).

Windows x64 assets:

| Asset | Purpose |
| --- | --- |
| `NOXEL.exe` | Portable application |
| `NOXEL-Setup.exe` | Inno Setup installer |
| `SHA256SUMS.txt` | Asset checksums |
| `LICENSE.txt` | GNU GPL v3 license text |
| `THIRD-PARTY-NOTICES.txt` | Licenses of bundled third-party components |

## Licensing

NOXEL's original application code is licensed under the **GNU GPL v3 only (`GPL-3.0-only`)**. The corresponding source for each binary release is available at [reprinted/NOXEL](https://github.com/reprinted/NOXEL) under the same version tag.

Third-party components and assets retain their own licenses (see `THIRD-PARTY-NOTICES.txt` in each release). NOXEL branding may have separate trademark considerations.

## Compatibility

Target: Windows 10/11 x64. Actual available modes and advanced color controls depend on the GPU, driver, display, and Windows configuration. Cross-vendor support must not be represented as hardware-tested without evidence.

## Updates

NOXEL checks the [GitHub Releases API](https://api.github.com/repos/reprinted/NOXEL-Releases/releases/latest) for new stable releases. It installs an update only after verifying its size, SHA-256 checksum and version.

Only download from the official repository. GitHub hosting and SHA-256 checksums are not substitutes for publisher signing; unsigned executables may prompt Windows warnings.

## Development

See [the release checklist](docs/RELEASING.md). Do not upload private configuration files, credentials, signing keys, personal information, or unreleased artifacts.
