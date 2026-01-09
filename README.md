# LyraX Releases

![LyraX logo](./logo.svg)

LyraX Releases is the public distribution repo for the LyraX CLI. It hosts
prebuilt binaries and release notes so installs are fast, repeatable, and
platform specific.

## Quick install (recommended)

```bash
npm i -g lyrax
lyra --help
```

The npm package downloads the correct binary for your OS and CPU at install
time.

## What lives here

- GitHub Releases with prebuilt LyraX CLI binaries.
- Release notes and version history.
- No source code. This repo only contains release artifacts.

## Supported platforms

| OS    | Architecture | Asset example                     |
|-------|--------------|-----------------------------------|
| macOS | arm64        | lyra-0.1.1-darwin-arm64.zip        |
| macOS | x64          | lyra-0.1.1-darwin-x64.zip          |
| Linux | arm64        | lyra-0.1.1-linux-arm64.zip         |
| Linux | x64          | lyra-0.1.1-linux-x64.zip           |
| Windows | x64        | lyra-0.1.1-win32-x64.zip           |

Each archive contains a single binary at the root:
- macOS/Linux: `lyra`
- Windows: `lyra.exe`

## Manual download

1. Open the latest release on GitHub.
2. Download the asset that matches your OS and CPU.
3. Unzip and run the binary.

```bash
./lyra --help
```

## Asset naming

Assets follow this convention:

```
lyra-<version>-<platform>-<arch>.zip
```

Examples:
- `lyra-0.1.1-darwin-arm64.zip`
- `lyra-0.1.1-linux-x64.zip`
- `lyra-0.1.1-win32-x64.zip`

## Environment overrides (advanced)

These are read by the npm installer:

- `LYRA_RELEASE_REPO`: release repo in `owner/repo` format.
- `LYRA_DOWNLOAD_BASE`: full download base URL (overrides `LYRA_RELEASE_REPO`).
- `LYRA_BINARY_PATH`: use an existing local binary instead of downloading.

## Notes

If you hit an install issue, include your OS, CPU architecture, and the
`lyrax` version you installed.
