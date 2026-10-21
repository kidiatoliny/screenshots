# Unified Dev: an update alert that never installs on Return

## Text: X

Unified Dev's update alert now shows what the new version changes, and you can skip a version. Every prompt opens on Later, so pressing Return never installs anything. And when a release's download is missing, the alert doesn't offer an Install button that leads nowhere.

## Text: Bluesky

Unified Dev's update alert now shows what the new version changes, and you can skip a version. Every prompt opens on Later, so pressing Return never installs anything. And when a release's download is missing, the alert doesn't offer an Install button that leads nowhere.

#Swift #macOS

## Text: LinkedIn

I don't want an update dialog to be one keypress away from installing.

In Unified Dev the update alert now shows the release notes of the version it offers, plus a button to skip that version. Every prompt opens on Later, and Return is always Later or Close, never Install. Nothing downloads until you press Install.

A review of the branch found six more things to fix. Two of them: release notes are now capped before they're parsed, because the parse runs on the main thread when the alert is built. And a skipped version whose download is missing no longer shows an Install button that leads nowhere.

What the alert says and which buttons it has is decided in the core and tested for each case: install, skipped, missing download, up to date.

What's the most annoying update prompt you've had to deal with?

#Swift #macOS
