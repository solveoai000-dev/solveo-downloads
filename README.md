# Solveo AI downloads

This repository hosts the published builds of **Solveo AI**, a desktop
assistant that reads a question on your screen and returns the answer
discreetly.

It contains no source code. Its only purpose is to serve the installers that
[solveo-ai.com](https://solveo-ai.com) links to.

## Download

Always download from [solveo-ai.com](https://solveo-ai.com). It points to the
latest build, so you do not have to pick a version yourself.

If you prefer a direct link, use the [latest release](../../releases/latest):

| File | What it is |
| --- | --- |
| `Solveo-Setup.exe` | Windows installer. Installs the app and creates shortcuts. |
| `Solveo-Portable.exe` | Windows, no installation. Runs as it is. |
| `solveo-bundle-<version>.zip` | Used by the app's own updater. Not meant to be downloaded by hand. |

Requires Windows 10 or 11. A macOS build is not published yet.

## About the Windows warning

These builds are not code-signed yet, so Windows SmartScreen shows
"Windows protected your PC" the first time you run the installer. Choose
**More info**, then **Run anyway**.

Code signing is planned. Until then, only download from
[solveo-ai.com](https://solveo-ai.com) or from this repository's releases, and
check that the publisher is `solveoai000-dev`.

## Verifying a download

Each release of the update bundle is published together with its SHA-256
checksum in the app's update manifest, and the app refuses any update whose
checksum does not match. You can verify a file yourself:

```powershell
Get-FileHash .\Solveo-Setup.exe -Algorithm SHA256
```

## Support

Questions, bugs, refunds: <support@solveo-ai.com>. Issues are disabled here
because this repository only stores files.
