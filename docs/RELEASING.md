# NOXEL Release Checklist

This is the public **distribution** repository. Do not upload application source code, tokens, private keys, signing credentials, or test data.

## Before publishing

1. Complete the proprietary end-user license draft and audit required third-party notices.
2. Select one version, for example `1.0.0`, and use it consistently in NOXEL's About page, executable, installer, and GitHub tag.
3. Run the existing automated tests and validate display safety, presets, and updater behavior.
4. Build the Windows x64 `NOXEL.exe` and `NOXEL-Setup.exe`.
5. Test upgrade and uninstall behavior; confirm user settings and presets are preserved.
6. Calculate SHA-256 for exact release files with `Get-FileHash <path> -Algorithm SHA256`, and optionally publish `SHA256SUMS.txt`.
7. Prepare clear release notes, known limitations, and installation instructions.

## Publish manually

1. Open https://github.com/reprinted/NOXEL-Releases/releases/new
2. Create a tag such as `v1.0.0` only for a verified finished build.
3. Use title `NOXEL v1.0.0`, write release notes, and attach only distribution files.
4. Publish as a stable release (not draft/prerelease) and verify the downloads.
5. Confirm `https://api.github.com/repos/reprinted/NOXEL-Releases/releases/latest` reports that version.

## Updater requirements

NOXEL's installed app must implement update checks, version comparison, downloads, integrity checks, user-approved installation, and safe behavior while a Keep/Revert display-mode confirmation is active. A GitHub repository by itself is **not** an auto-update implementation.

SHA-256 from the same release protects against mismatches but does not independently authenticate a publisher if the GitHub release is compromised. Consider code signing or independently signed manifests before enabling unattended automatic installation.

Test with controlled versions (e.g. `1.0.0` to `1.0.1`) without overwriting the working development installation.

Public releases are downloadable by anyone; use access-controlled distribution if NOXEL is intended to be truly invite-only.
