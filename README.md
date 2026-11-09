# NOXEL — Official Releases

**NOXEL** is a Windows display-management utility for resolutions, refresh rates, supported color controls, and saved presets.

This repository is the **public binary-distribution channel**. The source code is published at [reprinted/NOXEL](https://github.com/reprinted/NOXEL); every release here links to the matching source tag (for example `v1.0.0`).

## Downloads

**Official recommended download: [NOXEL-Setup.exe — Installer](https://github.com/reprinted/NOXEL-Releases/releases/latest).** Open the latest release and choose `NOXEL-Setup.exe` under **Assets** to install NOXEL normally.

**Alternative: [NOXEL.exe — Portable Version](https://github.com/reprinted/NOXEL-Releases/releases/latest).** The portable version runs directly without installing NOXEL. It is intended for people who prefer a standalone executable or want to test NOXEL without the normal installation process.

| File | What it is |
| --- | --- |
| **`NOXEL-Setup.exe`** | **Installer (recommended)** — installs NOXEL like a normal Windows application |
| **`NOXEL.exe`** | **Portable Version (optional)** — runs without installation |
| `SHA256SUMS.txt` | Download checksums |
| `LICENSE.txt` | GNU GPL v3 license text |
| `THIRD-PARTY-NOTICES.txt` | Third-party software license notices |

Both application versions offer NOXEL's display-management features. **The portable EXE is not the installer.**

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
