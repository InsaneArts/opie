# Security

## Reporting a vulnerability

Report it privately, through [GitHub's private vulnerability reporting](https://github.com/InsaneArts/opie/security/advisories/new). Never in a public issue or discussion.

Please include what an attacker gains, the steps to reproduce it, the version of Opie and of macOS, and anything that narrows down where it lives. A proof of concept helps.

Reports are read by the maintainers of Opie. If one holds, you will be told when a fix ships, and credited in the release notes unless you would rather not be.

## Supported versions

Only the latest release. Opie updates itself and checks for updates once a day, so the latest release is where a fix lands.

## What is in scope

The released Opie app: the input tap that listens for your Binding, the keys it sends for a Keystroke, the Actions it runs and the apps it controls for them, what it reads through the Accessibility API, its configuration files, what it sends for usage counts and crash reports, and the update mechanism.

Some things that would be interesting:

- Making a Ring fire an Action the user did not choose, or an Action run with a value it should have refused.
- Getting another app on the Mac to make Opie send keys, run an Action, or control an app without the user's hold and release.
- Making Opie read or send the contents of what a user made, such as their Keystrokes, scripts, or files, in a way "What leaves your Mac" in the README says should not happen.
- Getting an update installed that was not signed with Opie's EdDSA key, or otherwise subverting Sparkle.
- Anything a crafted configuration file can make Opie do beyond the Actions it names.

## What is not in scope

- Reports produced only by a scanner, with no working attack behind them.
- Missing hardening that leads nowhere on its own.
- Attacks that need an already-compromised Mac, physical access with the screen unlocked, or admin rights you already have.
- An Action doing what the user set it up to do, such as a script they wrote.
- Bugs in macOS itself, or in Apple's APIs, that Opie only passes through.

Do not test against other people's Macs. Test against your own installation.
