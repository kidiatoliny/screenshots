# Unified Dev: rebuilding the spend screen

## Text: X

I rebuilt the spend screen in Unified Dev. It was hand-drawn cards, and in light mode those white cards sat on a white window. Now it's a grouped Form like the settings, with columns ordered by cost. The bars got square ends too: a capsule turned a short bar into a dot.

## Text: Bluesky

I rebuilt the spend screen in Unified Dev. It was hand-drawn cards, and in light mode those white cards sat on a white window. Now it's a grouped Form like the settings, with columns ordered by cost. The bars got square ends too: a capsule turned a short bar into a dot.

#SwiftUI

## Screenshots

- `01-spend-screen.png`

---

# Unified Dev: spend by account

## Text: X

Unified Dev now splits agent spend by account, next to project and provider. Each account you are signed in to gets its own line and its own cost. The app groups transcripts by the account directory they sit under.

#Swift #macOS

## Text: Bluesky

Unified Dev now splits agent spend by account, next to project and provider. Each account you are signed in to gets its own line and its own cost. The app groups transcripts by the account directory they sit under.

#Swift #macOS

## Text: LinkedIn

Unified Dev can now show agent spend by account, next to project and provider.

Each agent CLI keeps its account in its own config directory. The app groups transcripts by the directory they sit under, longest match first, so an account directory nested inside another isn't swallowed by it. A transcript under no known directory becomes historic spend for that provider.

The part I learned something from: I don't ask the CLI which account it is. In my tests, claude auth status preferred the environment over the config directory, and said loggedIn for a forged token. So the app reads email, name, organisation, plan and expiry from the account's own directory, and keeps nothing a token lives in.

Do you keep more than one agent account on the same machine?

#Swift #macOS #AI

## Screenshots

- `02-by-account.png`
