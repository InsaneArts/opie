# Changelog

Every released version of Opie, newest first, with the download on the [releases page](https://github.com/InsaneArts/opie/releases). Opie checks for a new version once a day and offers to install it.

## 1.1.1 (2026-10-15)

- Screenshot & Recording Tools works again, and so do other Keystrokes for macOS shortcuts. Before, they did nothing while the Run reported success.
- Settings no longer stays in front of other apps' windows. It stands in front only during Getting Started.
- In a Liquid Ring, a Group's add buttons and the new moon's outline sit on the moons again.

## 1.1.0: Getting Started (2026-10-13)

- A first launch opens Getting Started. You play Pop!, a one-minute game that teaches the Ring before Opie asks for anything. Then you give Opie Accessibility, fire one Action for real, and keep fn or pick another key.
- A tour of Settings follows. A card points at each control while you make a Ring, add Actions, give the Ring its key, and use it. Optional chapters show App Rings, the Media Ring, Keystrokes and Shortcuts, Groups, and Appearance.
- Getting Started in Opie's menu bar menu opens it at any time. An update from 1.0.0 does not open it on its own.

## 1.0.0 (2026-10-12)

The first public release of Opie.

- Hold a key, and a Ring of Actions opens around the pointer. Move toward a Slice and let go to run it. While you hold the key, scroll to the next Ring, or press 1 to 8 to fire a Slice directly.
- Custom Rings open anywhere. App Rings open only in their app, all on one shared key. The Media Ring plays, pauses, and skips your music.
- Ready App Rings for Xcode, Safari, Chrome, Finder, VS Code, Cursor, Slack, Linear, Zoom, Things, Obsidian, OBS, Claude, and Herdr. Each one starts off; turn it on with its switch in Settings.
- A Slice runs an Action from the System Library, opens an app, sends a Keystroke, runs an Apple Shortcut, converts the file selected in Finder, or holds a Group of more Slices.
- Your Rings take your Theme, Palette, and animations, and they live in plain TOML files in `~/.config/opie/`.
- Opie checks for updates once a day and installs them through Sparkle.
