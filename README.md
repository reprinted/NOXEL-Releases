# NOXEL — Official Releases

**NOXEL** is a Windows display-management utility for resolutions, refresh rates, supported color controls, and saved presets.

This repository is the **public binary-distribution channel**. The NOXEL source repository is planned to be published separately at `reprinted/NOXEL` after a dependency, security, and license review. **Source code has not been published here.**

## Downloads

No stable release is published yet. Verified builds will appear on the [Releases page](https://github.com/reprinted/NOXEL-Releases/releases).

Planned Windows x64 assets:

| Asset | Purpose |
| --- | --- |
| `NOXEL.exe` | Portable application |
| `NOXEL-Setup.exe` | Inno Setup installer |
| `SHA256SUMS.txt` | Asset checksums |

## Licensing

**Planned license for NOXEL's original application code: GNU GPL v3 only (`GPL-3.0-only`).**

The GPL transition is **in preparation**. NOXEL's original source has not been published under GPL yet; an old proprietary EULA should not accompany future GPL releases.

Before publishing binaries, the developer must include the applicable GPL v3 license text, corresponding source-code access for the exact build, copyright notices, and all required third-party licenses. Third-party components and assets retain their own licenses. NOXEL branding may have separate trademark considerations.

This repository's README does not itself license unpublished source code or grant rights to third-party components.

## Compatibility

Target: Windows 10/11 x64. Actual available modes and advanced color controls depend on the GPU, driver, display, and Windows configuration. Cross-vendor support must not be represented as hardware-tested without evidence.

## Updates

The updater inside the NOXEL application is being developed. Its planned stable release endpoint is [GitHub Releases API](https://api.github.com/repos/reprinted/NOXEL-Releases/releases/latest). Until the first stable release exists, this may return 404.

Only download from the official repository. GitHub hosting and SHA-256 checksums are not substitutes for publisher signing; unsigned executables may prompt Windows warnings.

## Development

See [the release checklist](docs/RELEASING.md). Do not upload private configuration files, credentials, signing keys, personal information, or unreleased artifacts.
