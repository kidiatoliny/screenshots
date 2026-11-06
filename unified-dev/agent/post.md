# Swift concurrency: the Stop button and AsyncStream

## Text: X, Bluesky

Swift concurrency lesson from Unified Dev: cancelling the Task that iterates an AsyncStream ends that stream for good. Our Stop button did exactly that, so every later agent turn ran with nobody listening. The runner now multiplexes its events instead. #Swift

## Text: LinkedIn

A Swift concurrency lesson from building Unified Dev.

Unified Dev streams each agent's events through an AsyncStream, and the Stop button cancelled the Task that was iterating it.

What I didn't know: cancelling the Task that iterates an AsyncStream ends that stream for good. So Stop worked once, and every later agent turn ran with nobody listening.

The fix was to stop tying the events to one consumer. The runner now multiplexes its events, so stopping a turn doesn't kill the stream the next turn needs.

If you use AsyncStream for events that outlive a single task, check what your cancel path actually ends.

Has Swift concurrency cancellation ever surprised you like this?

---

# Unified Dev: switch provider in the same chat

Planned: 2026-11-10 18:00 Luxembourg (X + Bluesky)

## Text: X

A chat in Unified Dev can now switch provider or account where it stands. Pick a Codex model in a Claude chat and the history and draft stay. The agent coming in is told what it missed. Switch back and the first one resumes its own session.

## Text: Bluesky

A chat in Unified Dev can now switch provider or account where it stands. Pick a Codex model in a Claude chat and the history and draft stay. The agent coming in is told what it missed. Switch back and the first one resumes its own session.

#Swift #macOS

## Screenshots

- `03-provider-switch.png`

---

# Unified Dev: switch provider in the same chat

Planned: 2026-11-11 08:30 Luxembourg (LinkedIn)

## Text: LinkedIn

In Unified Dev, a chat can now change provider or account where it stands.

Behind one chat there are now several native sessions, one per agent and account. Pick a model from another provider and the chat keeps its history and its draft. A running turn stops, queued messages stay. The agent coming in is told what it missed, as text it treats as untrusted. All you see is a divider.

Go back, and the first agent resumes its own session and gets only what happened since it left.

The case I wanted most: when a Claude turn is cut by the usage limit, it resumes on its own after a provider switch, once per cut and never after a Stop. The agent is told to check the repository before repeating anything.

Do you switch between coding agents in the middle of a task?

#Swift #macOS #AI

## Screenshots

- `03-provider-switch.png`
