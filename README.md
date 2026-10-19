# Prospect Multiplayer downloads

[**Download the latest Windows launcher**](https://github.com/daboisadasd/prospect-multiplayer-downloads/releases/latest/download/ProspectMultiplayerLauncher.exe)

[Full installation and upgrade guide](https://prospect.playit.plus/) · [All releases](https://github.com/daboisadasd/prospect-multiplayer-downloads/releases) · [Latest SHA256 checksum](https://github.com/daboisadasd/prospect-multiplayer-downloads/releases/latest/download/SHA256SUMS.txt)

This repository distributes the Prospect Multiplayer small client launcher, separate content files, and public checksums. The full supported original Prospect game installation is required.

## Install, update and play

1. Close this game copy and keep Steam running.
2. Download `ProspectMultiplayerLauncher.exe` and run it as your normal Windows user.
3. Choose the supported ReCycle or Steam depot installation from its numbered list. It reads ReCycle's saved game directory; the game does not need to be inside the launcher folder. Putting it directly in `Prospect/Binaries/Win64` also selects that copy.
4. **Enter** installs/updates; **P** updates and plays. Only changed components download. Our paks stay as separate normally named files in `Content/Paks`.
5. To return to ReCycle or Singleplayer Cycle, close the game, run this launcher and choose **U**. It restores the original DLLs/settings and parked ReCycle paks/mods. Uninstall needs no internet.

The launcher is about 0.6 MB. A fresh install downloads approximately 1.63 GiB once. Existing v86 assets are reused; this release adds Reyna's approximately 20 MB pak. Downloads resume after interruption.

Known singleplayer mod files are parked in `.ProspectUpdater` while our overlay is installed. **Keep that folder: it holds your originals.** Do not run another launcher against the same game copy until uninstalling multiplayer. Unknown external changes are preserved and stop the operation for review.

Options: `--play`, `--list`, `--check`, `--uninstall`, `--game-dir PATH`, `--help`.

The old large setup EXE used an install/remove toggle. Stop using it while the new overlay is installed. Older setup backups remain untouched; uninstall restores the installation state captured when this launcher was first used. Game progress and saved recordings outside the install directory are not rolled back.

## Included maps

PvP01, Killhouse 3, Killhouse 4, and DM Map. Bright Sands comes with the required original game installation.

## Included client tools

The current launcher includes native replay recording and a separate replay
viewer, the end-of-raid skip control, an Insurance **Claim All** button, and
**Recent Purchases / Rebuy** at each trader. Rebuy remembers the purchased stack
quantity. Its history is saved on the server separately for each account and
trader, so switching computers does not reset it.

### Cosmetics and weapon inspect

Choose **Karambit** through normal melee cosmetic customization. Updated players
can see its equip/resting pose and swings and hear its sounds. Press **K** to
inspect a gun or knife, or change **Inspect Weapon** in Settings → Keybinds.
Firing, reloading or switching weapons cancels the first-person inspect.

### Loadout presets

At Station, open **Tab → Inventory**. Use **Save as Preset** to save a kit into
Preset A, B or C, then select its tab to preview or equip it. The game uses your
stash first. **Purchase & Equip** lists missing trader items and their actual
K-Mark total before confirmation; preset slots are free. Exact pieces that are
not available from the traders are skipped. Presets are stored on your account
on the server.

Free loadouts have been removed. Deployment uses the original insurance screen
without an added kit-selector overlay. This release retains the Station UI
optimizations; remaining Station hitches are still being evaluated in real play.

### Record and watch a replay

- **Ctrl+Shift+R:** start recording while in a multiplayer raid.
- **Ctrl+Shift+S:** stop recording.
- **Ctrl+Shift+P:** select a recording and open it in a separate viewer window.
- In the viewer, **F5** plays/pauses and **F6** switches normal/slow motion.
- **WASD + mouse** moves the viewer's free camera.

Recordings are saved in `%LOCALAPPDATA%\Prospect\Saved\Demos` for a normal
installation. The viewer currently has no rewind/seek control; reopen the take
to start it again.

### Console and debug camera

The native local cheat manager and console are available for each player.
Press **F10**, type `toggledebugcamera`, and press Enter. F10 closes the console;
repeat the command to return to your player. Commands that require server
authority still depend on the game's own permissions.

## Verify a download

Each release includes `SHA256SUMS.txt`. In PowerShell, run:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\ProspectMultiplayerLauncher.exe'
```

Compare the hash with the checksum from the same release. Matching hashes verify that the downloaded file matches the published launcher.

The launcher and individual components are hosted on GitHub Releases. Signed update metadata and SHA256 protect component integrity; normal HTTPS checks remain enabled. No administrator access, custom certificate, antivirus exclusion or downloaded script is required. The initial EXE is not Authenticode signed; use the official download and checksum. No software can promise zero security issues. The community website and game services remain at their existing addresses.
