# NOXEL Open-Source Release Checklist

NOXEL is transitioning from a proprietary EULA to **GNU GPL v3 only (SPDX `GPL-3.0-only`)**. Do not publish an old proprietary EULA as NOXEL's application license.

## A. Prepare source repository

1. Audit every distributed library, font, runtime, and other asset for license compatibility and required notices. Validate Windows App SDK, .NET, any WebView2 or driver SDK redistributions actually bundled.
2. Verify the rights/ownership needed to GPL-license all NOXEL original code. Record contributions and imported code accurately.
3. Create the separate public `reprinted/NOXEL` source repository **only when approved**.
4. Add the verbatim official GPL v3 license text in `LICENSE`, without altering it. Use SPDX `GPL-3.0-only` in documentation and, where helpful, source headers.
5. Replace the proprietary EULA in the application, installer, About page, and docs with accurate GPL license information. Keep third-party notices and any necessary separate privacy notices.
6. Scan repository content *and commit history* for tokens, private keys, credentials, personal files, debug logs, proprietary third-party code, and unwanted binary artifacts. Ensure no secrets are in committed history. Configure `.gitignore`.
7. Add README, build prerequisites, build scripts, CONTRIBUTING.md (optional), SECURITY.md (optional), and exact source-to-binary build instructions. Confirm the code builds.

## B. Prepare each binary release

1. Choose one version; synchronize app, installer, and tag.
2. Run tests, hardware-safe checks, accessibility checks, and update tests. Preserve existing display configuration.
3. Produce `NOXEL.exe`, `NOXEL-Setup.exe`, and SHA-256 hashes.
4. Make the **complete corresponding source** for that precise binary release available under GPL v3, including build/install scripts and any required modifications or source for bundled GPL-covered components. Use a matching source tag such as `v1.0.0` in `reprinted/NOXEL` and a clear corresponding-source link in the release notes. Review GPL v3 requirements for conveying object code and whether any further source offer is needed.
5. Include the GPL v3 text, copyright notices, and all required third-party notices with distributed builds and/or installer as legally required.
6. Verify portable and installer upgrades preserve user settings and don't interrupt active display Keep/Revert operations.
7. Check whether unsigned-build Windows warnings are expected; don't claim code signing unless validated.
8. Manually approve the production release.

## C. Publish

1. Visit https://github.com/reprinted/NOXEL-Releases/releases/new
2. Create a stable tag such as `v1.0.0` for a tested build.
3. Attach binaries/checksums. Clearly label **`NOXEL-Setup.exe` as “Installer (recommended)”** and **`NOXEL.exe` as “Portable Version (no installation required)”** in the release description. Keep these exact filenames for the updater. Clearly link the matching tagged source in the public `NOXEL` repository and include license and compatibility notes.
4. Verify downloads and API endpoint: https://api.github.com/repos/reprinted/NOXEL-Releases/releases/latest
5. Test automatic update from an older controlled build without overwriting the development environment.

## Security and privacy reminders

- Do not upload signing keys, release tokens, sensitive settings, local environment information, or personal documents.
- Public repositories and public release assets are accessible to anyone, even if you distribute the URL privately.
- A SHA-256 checksum hosted in the same release provides integrity checking but not independent proof of publisher identity.
- An open-source license does not automatically grant trademark rights or permission to redistribute third-party assets outside their licenses.
