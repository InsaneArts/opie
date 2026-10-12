# Contributing

Opie's source code is not in this repository. What this repository takes is reports, and they are worth more than they sound: most of what Opie gets wrong is one Ring away from being obvious, and only the person holding the key knows what they meant to happen.

## The three kinds of report

**A bug.** Something does not work. [Open one](https://github.com/InsaneArts/opie/issues/new/choose) with the steps, the version, and what you expected. Logs help most of all:

```sh
log stream --predicate 'subsystem == "com.insanearts.opie"'
```

The log can name the apps and files you used. Read it before you paste it.

**An App Ring request.** An app you use every day, and the things you do in it. This has its own form, because the useful part is the list: which app, and which of its commands you reach for most. The app's own keyboard shortcuts for them help too.

**A request.** Something Opie should do and cannot. Say what you are trying to get done first, and the feature second; the task is the part that cannot be guessed. If it is still half-formed, [Discussions](https://github.com/InsaneArts/opie/discussions) is the better room.

## Before you open one

Search first; the same thing often comes up twice. Be on the latest release, or say which one you are on and why. One report per thing: two bugs in one issue means one of them gets forgotten.

## What not to post

No credentials. No filenames, screenshots, or logs that carry someone else's data, or yours. A made-up example that shows the same problem is always fine.

Security issues do not go in public at all: [SECURITY.md](SECURITY.md) says where they go.

## The code of conduct

[CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md), and it is short. Be plain, be kind, stay on the topic.
