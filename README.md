# Prospect Multiplayer downloads

[**Download the latest Windows setup EXE**](https://github.com/daboisadasd/prospect-multiplayer-downloads/releases/latest/download/ProspectMultiplayerSetup.exe)

[Full installation and upgrade guide](https://prospect.playit.plus/) · [All releases](https://github.com/daboisadasd/prospect-multiplayer-downloads/releases) · [Latest SHA256 checksum](https://github.com/daboisadasd/prospect-multiplayer-downloads/releases/latest/download/SHA256SUMS.txt)

This repository distributes the Prospect Multiplayer client installer and public checksums. The full supported original Prospect game installation is required.

## Install and play

1. Close the game and keep Steam running.
2. Put `ProspectMultiplayerSetup.exe` beside `Prospect-Win64-Shipping.exe`, normally in `Prospect\Binaries\Win64`. Supported copies using `Binaries\mp` should use that folder instead.
3. Run setup once and wait for the installation confirmation.
4. Launch with the generated **Play Prospect Multiplayer** shortcut. Keep the setup EXE in its installed location; you may copy the shortcut to your desktop.

**Setup is an install/remove toggle.** After installation, running setup normally again removes multiplayer support. Use the Play shortcut to play.

## Update an older installation

Close the game. Replace the old setup EXE in the game folder with the latest one, run it once to remove the recognized old installation, then run it again to install the new version. Launch with **Play Prospect Multiplayer**.

## Included maps

PvP01, Killhouse 3, Killhouse 4, and DM Map. Bright Sands comes with the required original game installation.

## Verify a download

Each release includes `SHA256SUMS.txt`. In PowerShell, run:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\ProspectMultiplayerSetup.exe'
```

Compare the hash with the checksum from the same release. Matching hashes verify that the downloaded file matches the published installer.

The setup EXE is hosted on GitHub Releases so the large download does not pass through the game host's home upload connection. The community website and game services remain at their existing addresses.
