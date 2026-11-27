# Tycho: Home

Planned: 2026-11-13 18:00 Luxembourg (X + Bluesky)

## Text: X

Tycho opens on Home: today's tasks, and cards for what's open, done and overdue. A card takes you to Tasks with that filter already applied.

## Text: Bluesky

Tycho opens on Home: today's tasks, and cards for what's open, done and overdue. A card takes you to Tasks with that filter already applied.

#SwiftUI #iOS #macOS

## Screenshots

- `01-home.png`
- `02-overdue-filter.png`
- `03-ios-home.png`

---

# Tycho: Home counts that mean something

Planned: LI 10/12 08:30, Bluesky 11/12 18:00, X 11/12 18:00 (Europe/Luxembourg)

## Text: X

Lesson from Tycho: a card's number has to match the list it opens. Home's Completed card counted tasks done in the last 7 days, but its list filtered by last update, so editing an old task put it in the list and not in the count. Now both read the completion date.

## Text: Bluesky

Lesson from Tycho: a card's number has to match the list it opens. Home's Completed card counted tasks done in the last 7 days, but its list filtered by last update. Now both read the completion date.

#SwiftUI #macOS

## Text: LinkedIn

A small lesson from Tycho, the task manager I'm building in SwiftUI: a card's number has to match the list it opens.

Tycho opens on Home, with cards for open, completed and overdue tasks. The Completed card counted tasks done in the last 7 days, but the list it opens filtered done tasks by their last update. So editing an old completed task put it in the list and not in the count. Now the card and the list share one filter on the completion date, and the card says "last 7 days".

The same week I found the counts included tasks without a project, which the lists never showed. Now both only look at live projects, and a test checks every card against the list it opens.

Project progress is drawn as the system's capacity gauge instead of a bar I drew myself.

#SwiftUI #macOS #Tycho

## Screenshots

- `04-counts-gauge.png`
