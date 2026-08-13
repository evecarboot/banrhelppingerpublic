# BANR Help Pinger
Just somewhere to upload the releases for The Bannermen corp members to download. 

## Download

Choose the package for your operating system from the repository's Releases page.

- Windows x64: `BANRHelpPinger-test-windows-x64.zip`
- macOS Intel: `BANRHelpPinger-test-macos-intel.app.zip`
- macOS Apple Silicon: `BANRHelpPinger-test-macos-arm64.app.zip`
- Linux x64: `BANRHelpPinger-test-linux-x64.AppImage`

Use the `test` packages while testing. The `main` packages send alerts to the production Discord webhook and should only be distributed after testing is complete.

## Windows

1. Download `BANRHelpPinger-test-windows-x64.zip`.
2. Extract the ZIP.
3. Double-click `BANRHelpPinger.exe`.
4. Click `ESI Login` and sign in with a character in The Bannermen.
5. Select the EVE log folder. This is normally the folder containing `Gamelogs` and `Chatlogs`.
6. Click `Start Monitoring`.

The app must show `Running - watching logs` before it can send alerts.

The Windows test ZIP also contains `run-test.bat`. Double-click it to create a test log and simulate a webbed attack. Follow the prompts in that window.

## macOS

1. Download the package matching the Mac's processor.
2. Double-click the downloaded ZIP to extract the app.
3. Move `BANRHelpPinger.app` to Applications if desired.
4. Double-click the app.
5. If macOS shows an unidentified-developer warning, right-click the app, choose `Open`, then choose `Open` again.
6. Click `ESI Login`, sign in with a Bannermen character, select the EVE log folder, and click `Start Monitoring`.

Choose `macos-intel` for Intel Macs. Choose `macos-arm64` for Apple Silicon Macs.

Damaged file... 

Rename it to BANRHelpPinger and then run this in terminal `xattr -cr ~/Downloads/BANRHelpPinger.app` and then drag it to your applications folder.

## Linux

1. Download `BANRHelpPinger-test-linux-x64.AppImage`.
2. Open it with the file manager and choose `Run`.
3. If the desktop asks whether to trust or make it executable, approve that once.
4. Click `ESI Login`, sign in with a Bannermen character, select the EVE log folder, and click `Start Monitoring`.

## Requirements

- ESI login with a character in The Bannermen corporation (ID `98760719`).
- Access to the EVE log folder.
- Internet access for ESI and Discord.

The app watches new and changed `.txt` files under `Gamelogs` and `Chatlogs`. It does not replay old combat history when monitoring starts.

## Reporting a Problem

When reporting a problem, include the operating system, package name, selected log-folder path, and the messages shown in the app log panel. Do not post ESI tokens or Discord webhook URLs.


## EVE Online Game Logs

**Windows**

```text
%USERPROFILE%\Documents\EVE\logs\
```

**macOS**

```text
~/Documents/EVE/logs/
```

**Linux**

```text
~/Documents/EVE/logs/
```

**Linux (Steam/Proton)**

```text
~/.local/share/Steam/steamapps/compatdata/8500/pfx/drive_c/users/steamuser/My Documents/EVE/logs/
```
