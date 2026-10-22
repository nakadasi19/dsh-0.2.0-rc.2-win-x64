# DeepSeek Harness 0.2.0-rc.2 - win-x64 portable

Archived build of DeepSeek Harness **0.2.0-rc.2** (Electron, Windows x64), packed from a working
install directory as a portable 7z archive. Kept around because the upstream feed has moved on to
newer releases and the original setup.exe for this version is no longer obtainable.

## Download

Asset on the [releases](../../releases) page:

`
deepseek-harness-0.2.0-rc.2-win-x64-portable.7z
`

| | |
|---|---|
| version | 0.2.0-rc.2 |
| platform | Windows x64 |
| archive size | 398,743,179 bytes (380.3 MB) |
| unpacked | ~1.37 GB, 22,742 files |
| sha256 | $hash |

## Run

1. Extract the archive anywhere (7-Zip / NanaZip - Explorer cannot open .7z natively).
2. Run DeepSeek Harness.exe.
3. First launch recreates %USERPROFILE%\.dsh and %APPDATA%\@deepseek-ai; user data is *not*
   bundled, so this is a clean profile.

## Verify

`
eeb7e78ca537230b019c93e87684e412e621c209def913a850aa3bd53a35a16d  deepseek-harness-0.2.0-rc.2-win-x64-portable.7z

`

certutil -hashfile deepseek-harness-0.2.0-rc.2-win-x64-portable.7z SHA256 (Windows) or sha256sum deepseek-harness-0.2.0-rc.2-win-x64-portable.7z (Linux/macOS) must match.

## Notes

- Not the official installer: no registry uninstall entry, no Start Menu shortcut. Delete the
  folder to remove it entirely.
- Bundled runtime recorded in esources\runtime\versions.json (Node 24.18.1, pnpm 11.7.0).
- Upstream feed: https://download.deepseek.com/dsh-desk/feeds/win-x64/