# Tracknote

Releases of **Tracknote**, a music recording app for Windows 10/11. Record guitar and vocals with your laptop or USB
microphone, import backing tracks (WAV, MP3, FLAC, OGG, M4A), and edit them into a finished song on a multi-track
timeline: move, split, trim and fade clips, set volume, pan, mute and solo, loop a section, and export the mix as WAV.
Recording is built for a guitar in front of a simple mic: one-bar count-in, input meter with level guidance, a live
low-end boom check, voice-call processing turned off, a noise gate with room-noise measurement, background noise
reduction, and *Recording polish*, which finds and tames the soundhole resonance and evens out the level. All
processing is non-destructive: originals are kept and you can compare before/after at any time. Korean user interface,
dark theme.

## Download
Open the [latest release](../../releases/latest) and download `Tracknote-windows-<version>-setup.exe`.

## Updates
The app includes an automatic update system.

A few seconds after Tracknote starts it checks this repository for a new version. If there is one, it shows what
changed and asks you; nothing is downloaded until you choose **Install**. The installer is verified against the
app's signing key before it runs, and if anything fails the current version keeps working. Your projects,
recordings and settings are kept. You can turn the check off in **Settings**.

`latest.json` and the `.sig` file are used by the automatic updater. You don't need to download them.

## Installation
1. Download `Tracknote-windows-<version>-setup.exe`
2. Run it. It installs for the current user (no administrator rights) to `%LOCALAPPDATA%\Tracknote` and adds a Start menu entry
3. Start **Tracknote**, create a project, set the tempo, and press the record button on a track

> Windows may show "Windows protected your PC" because the installer isn't code-signed. Choose **More info** → **Run anyway**.

> Tracknote uses Microsoft Edge WebView2, which is part of Windows 11 and current Windows 10. If it is missing, the installer downloads it.

## Notes
- Use headphones or earphones while recording over a backing track, otherwise the speakers leak into the mic. Bluetooth earphones add a lot of delay; wired ones are better for recording.
- If Windows blocks the microphone, turn on *Settings → Privacy & security → Microphone → Let desktop apps access your microphone*.
- Recording latency is compensated automatically; if takes still land early or late, adjust the timing offset in Settings or nudge the clip.
- Everything runs on your PC. Tracknote doesn't upload audio and has no account or telemetry. The only network access is the update check against this repository.
- Projects and recordings are kept in `%LOCALAPPDATA%\com.smallestdev.tracknote`. Uninstalling keeps them unless you tick "delete app data".
- Planned: virtual piano and computer-keyboard input, piano roll, drum patterns, EQ/reverb/delay, pitch and time stretching, MIDI devices.
- `.sha256` files contain the SHA-256 checksum of each download.
