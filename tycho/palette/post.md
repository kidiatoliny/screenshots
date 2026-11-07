# Tycho: the command palette

Planned: 2026-11-12 10:00 Luxembourg (X + Bluesky)

## Text: X

Command-K in Tycho opens a palette: suggestions, recent tasks, recent searches and results per scope, all from the keyboard. Single keys and G chords navigate too, and they stand down while you type in a field or a sheet is open.

## Text: Bluesky

Command-K in Tycho opens a palette: suggestions, recent tasks, recent searches and results per scope, all from the keyboard. Single keys and G chords navigate too, and they stand down while you type in a field or a sheet is open.

#SwiftUI #macOS

## Screenshots

- `01-command-k.png`
- `02-search.png`
- `03-view-all.png`

---

# Tycho: the command palette

Planned: 2026-11-12 08:30 Luxembourg (LinkedIn)

## Text: LinkedIn

Tycho, the task manager I'm building in SwiftUI, now has a command palette.

Command-K, or the toolbar button, opens an overlay with suggestions, recent tasks, recent searches and results grouped by scope. Arrow keys, Return, Tab and Escape drive it, and "View all" opens a search page with a count per scope.

The shortcuts around it were the harder part. Single keys like N and P, and G chords for navigation, have to stand down while you type in a field or a sheet is open, and they have to stay out of the way during onboarding. A good share of this phase's commits went into those guards and the UI tests that check them.

Keyboard or mouse, how do you move around your task manager?

#SwiftUI #macOS #iOS

## Screenshots

- `01-command-k.png`
- `02-search.png`
- `03-view-all.png`
