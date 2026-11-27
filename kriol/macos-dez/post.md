# How Kriol got to the Mac (thread)

Planned: X 12/12 10:00, Bluesky 12/12 10:00 (Europe/Luxembourg)

## Text: X (thread)

1/ How Kriol, a programming language in Cabo Verdean Creole, got to the Mac. A short thread, because most of it wasn't me. 🧵

2/ First, Edilson Tavares found that the test script started with #!/usr/bin/bash, which doesn't exist on macOS. He switched it to /usr/bin/env bash and added a macOS build workflow.
   - `kriol/macos/01-check-passes.png`

3/ Then Anaxímeno Brito put macOS in the release. The workflow runs otool -L on the binary and fails if it links anything from Homebrew, so it runs on a Mac that doesn't have it.
   - `kriol/macos/02-otool-no-homebrew.png`

4/ My part: the install script now checks the archive's SHA256 against the release before extracting. Anaxímeno then taught it macOS, so one command installs Kriol on a Mac.
   - `kriol/macos/04-install-sh.png`

## Text: Bluesky

How Kriol got to the Mac: Edilson Tavares fixed the test script's shebang and added a macOS workflow, Anaxímeno Brito put macOS in the release with a check against Homebrew libraries, and I made the install script verify the SHA256.

#Kriol #macOS

## Screenshots

- `kriol/macos/01-check-passes.png`
- `kriol/macos/02-otool-no-homebrew.png`
- `kriol/macos/04-install-sh.png`
