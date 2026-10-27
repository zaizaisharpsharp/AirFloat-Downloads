# AirFloat test downloads

**Move anything. Between anything.**

This repository distributes compiled, experimental AirFloat installers only.
It does not contain AirFloat application source code. These are test prereleases,
not production releases. Universal compatibility is not claimed.

## Downloads

Use the assets on the [Releases page](https://github.com/zaizaisharpsharp/AirFloat-Downloads/releases).
Each prerelease includes versioned filenames, SHA-256 checksums and installation
instructions. A GitHub account is not required to download public release assets.

## Installation status

macOS distribution is being audited. The existing private development DMG has not
been uploaded: its development signing identity and build paths fail the public
artifact privacy gate. Do not interpret an absent Mac download as installation
success. A new public test candidate must disclose its actual signing and
notarization status.

No installers or release assets have been published. The Windows test package is
unsigned and is also held from publication. A normal signed MSIX installation remains
blocked until a trusted publisher signature is available. Do not install a
development certificate, enable Developer Mode or disable Windows protections to
make this package install. The framework-dependent build requires Microsoft's
.NET 8 Desktop Runtime (x64); no runtime or development credentials are bundled.

## Intended physical test

1. Download the appropriate test installer from a release.
2. Install and open AirFloat normally. Stop if the OS blocks launch; record the
   warning instead of overriding its security policy.
3. Grant normal requested OS permissions.
4. Choose **Everyone Nearby** from AirFloat's tray/menu-bar home.
5. Choose the other compatible AirFloat computer, then accept on the recipient.
6. Verify discovery and file transfers in both directions, including matching
   source and destination SHA-256 hashes.

The current test uses a shared local network and AirFloat installed on both
computers. Direct wireless, stock AirDrop receiving and compatibility with every
platform are not demonstrated. Clipboard sync requires separate explicit trust.

## Privacy and integrity

Release assets exclude source trees, debug symbols, logs, received files, device
identities, trust databases and private keys. Each download is audited before
publication. Compare its SHA-256 with the release's `SHA256SUMS.txt`.
Download checksums establish artifact integrity, not fresh-device compatibility.
