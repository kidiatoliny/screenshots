# Unified Dev: Grok accounts

Planned: X 18/12 18:00, Bluesky 18/12 18:00, LinkedIn 23/12 08:30 (Europe/Luxembourg)

## Text: X

Grok is now a full account in Unified Dev: each profile can sign in to its own Grok account, like Claude Code and Codex. To know if it's signed in, the app asks grok models under that account's own GROK_HOME and reads the email from its auth.json.

## Text: Bluesky

Grok is now a full account in Unified Dev: each profile can sign in to its own Grok account, like Claude Code and Codex. The app checks the login under that account's own GROK_HOME.

#Swift #macOS #AIAgents

## Text: LinkedIn

Adding an agent to Unified Dev is the easy part. Knowing which account it runs as is the hard part.

Unified Dev, my macOS app for running coding agents in parallel, now lets a profile sign in to its own Grok account, the same way it already did for Claude Code and Codex. To know whether that account holds a login, the app runs grok models under the account's own GROK_HOME, and reads the email and name from that account's auth.json. Nothing comes from the environment the app happened to start with.

I tried the same for Antigravity, Cursor and OpenCode. Each one refused for a reason I could measure, and those reasons are written down in the docs instead of worked around.

Do you run more than one account per agent?

#Swift #macOS #AIAgents

## Screenshots

- `unified-dev/settings/03-grok-account.png`
