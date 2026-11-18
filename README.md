# NOXEL Releases

Download NOXEL for Windows 10/11 x64. NOXEL lets you switch display modes, adjust supported color controls, and save settings as presets.

| Download | Choose this if |
| --- | --- |
| **[Windows installer](https://github.com/reprinted/NOXEL-Releases/releases/latest/download/NOXEL-Setup.exe)** | You want the recommended per-user installation. |
| [Portable executable](https://github.com/reprinted/NOXEL-Releases/releases/latest/download/NOXEL.exe) | You want to run NOXEL without installing it. |

[Release notes and all assets](https://github.com/reprinted/NOXEL-Releases/releases/latest) · [Source code and documentation](https://github.com/reprinted/NOXEL)

## Other release assets

| File | Purpose |
| --- | --- |
| `SHA256SUMS.txt` | Download checksums |
| `NOXEL-source.zip` | Corresponding source archive |
| `LICENSE.txt` | GNU GPL v3 license text |
| `THIRD-PARTY-NOTICES.txt` | Third-party software license notices |

## Licensing

NOXEL's original application code is licensed under the **GNU GPL v3 only (`GPL-3.0-only`)**. The corresponding source for each binary release is available at [reprinted/NOXEL](https://github.com/reprinted/NOXEL) under the same version tag.

Third-party components and assets retain their own licenses (see `THIRD-PARTY-NOTICES.txt` in each release). NOXEL branding may have separate trademark considerations.

## Compatibility

Target: Windows 10/11 x64. Actual available modes and advanced color controls depend on the GPU, driver, display, and Windows configuration. See the [compatibility notes](https://github.com/reprinted/NOXEL#compatibility) for tested hardware and driver-specific features.

## Updates

NOXEL checks the [GitHub Releases API](https://api.github.com/repos/reprinted/NOXEL-Releases/releases/latest) for new stable releases. It installs an update only after verifying its size, SHA-256 checksum and version.

Only download from the official repository. GitHub hosting and SHA-256 checksums are not substitutes for publisher signing; unsigned executables may prompt Windows warnings.

## Development

See [the release checklist](docs/RELEASING.md). Do not upload private configuration files, credentials, signing keys, personal information, or unreleased artifacts.
