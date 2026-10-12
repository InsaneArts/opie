# Changelog

Every released version of Opie, newest first, with the download on the [releases page](https://github.com/InsaneArts/opie/releases). Opie checks for a new version once a day and offers to install it.

## 1.0.0 (2026-10-12)

The first public release of Opie.

- Hold a key, and a Ring of Actions opens around the pointer. Move toward a Slice and let go to run it. While you hold the key, scroll to the next Ring, or press 1 to 8 to fire a Slice directly.
- Custom Rings open anywhere. App Rings open only in their app, all on one shared key. The Media Ring plays, pauses, and skips your music.
- Ready App Rings for Xcode, Safari, Chrome, Finder, VS Code, Cursor, Slack, Linear, Zoom, Things, Obsidian, OBS, Claude, and Herdr. Each one starts off; turn it on with its switch in Settings.
- A Slice runs an Action from the System Library, opens an app, sends a Keystroke, runs an Apple Shortcut, converts the file selected in Finder, or holds a Group of more Slices.
- Your Rings take your Theme, Palette, and animations, and they live in plain TOML files in `~/.config/opie/`.
- Opie checks for updates once a day and installs them through Sparkle.
