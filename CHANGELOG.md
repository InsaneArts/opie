# Changelog

Every released version of Opie, newest first, with the download on the [releases page](https://github.com/InsaneArts/opie/releases). Opie checks for a new version once a day and offers to install it.

## 1.4.0: Files and AirDrop (2026-10-22)

### New

- Four new Actions in Files & research work on everything you select in Finder. Copy Files puts the items on the clipboard, ready to paste in Finder. AirDrop opens the AirDrop picker with them. Move to Folder and Copy to Folder ask for a folder each time. If a name is already in that folder, they move or copy nothing.
- You can set the dead zone. In Settings, open Ring and pick a Dead zone: Small (8 px), Standard (16 px), Large (22 px), or Extra large (28 px). A release inside the dead zone cancels. Standard stays the default. The setting shows when "Fire a Slice" is "On release".
- Ring size goes up to 200%. On a larger Ring, child Slices fire where the Ring draws them.
- The Media Ring stays open after a click or a digit fires a Slice, so you can pause and skip in one hold. Let go to close it.

### Changes

- Copy full file path copies the path of every selected item, one per line.
- The Ring in the Settings preview stays at 100%, whatever Ring size says. The live Ring, Try it, and Practice show your Ring size.

### Fixes

- Keystrokes work right after you allow Accessibility. Before, they failed until Opie restarted.
- A Binding made with Hyperkey opens the Ring. Opie now reads each key after other apps change it.
- When you record a Binding or a Keystroke, Opie hears system shortcuts such as ⇧⌘Tab and ⌃Space.
- The tour no longer stops at "Now scroll between Rings." It shows that step only when another Ring shares the new Ring's Binding.

## 1.3.0: Fire on Click (2026-10-19)

### New

- A Slice can fire on a click. In Settings, open Ring and set "Fire a Slice" to "On click". Hold your key to open the Ring, point at a Slice, and click it. A click on the Center cancels. "On release" stays the default.

### Changes

- Liquid is the default Theme. A Theme you picked in Settings stays.

### Fixes

- The Slack App Ring works again. Search, Quick Switcher, Unread, Threads, and DMs open in Slack. Before, they did nothing while the Run reported success.

## 1.2.0: Statistics (2026-10-15)

### New

- Statistics, a new seat in Settings, shows how you use Opie: your flicks, streaks, a calendar of active days, your favorite Actions and Rings, and milestones. The numbers stay on your Mac and are never part of the usage counts. You can pause or reset them on the page.
- The Folder card opens a folder in Finder from a Slice: Downloads, Applications, Desktop, Documents, Home, or any folder you choose.
- Rings can share a key. Hold it and scroll to switch between them, and the Ring you used last opens next time. On the App Ring key, the App Ring of the app in front opens first.

### Changes

- A scroll while you hold a key reaches only the Rings on that key. On the App Ring key, other apps' App Rings no longer join.
- Each Slice name on the Ring sits on a small mat, so it reads on any wallpaper, in light and dark.
- Every App Ring in Settings shows its app's icon. When the app is not installed, the icon shows faded with a download badge.
- The installer window shows where to drag Opie.

### Fixes

- Xcode Actions work again after Xcode relaunches. Before, they said Xcode was no longer in front.
- Lock Screen works on macOS 27.
- Eject All Disks works. It ejects the disks and disk images in Finder's sidebar, and one disk in use does not keep the others mounted. It no longer asks for Finder Automation.
- Getting Started notices the Accessibility grant without a relaunch. When Opie is missing from the Accessibility list, a panel beside System Settings lets you drag Opie into it.

### Usage counts

- Opie's anonymous usage counts now say which kind of Ring a flick comes from: one of your own Rings, an App Ring, or the Media Ring. For an App Ring, only the name of an app Opie ships Actions for is sent, such as Slack or Xcode. Any other app is counted as "other".
- Once a day, Opie sends how many Rings, Saved Actions, Scripts, and mouse Bindings you have. Only the numbers leave your Mac. Names, keys, and contents stay on it.
- Getting Started reports which steps it shows and where it ends, so we can see where it is too long.
- To turn usage counts off, quit Opie and run `defaults write com.insanearts.opie OpieTelemetryEnabled -bool false`.

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
