# Tycho: the macOS UI made native

Planned: LI 23/11 08:30, X 23/11 10:00, Bluesky 23/11 10:00 (Europe/Luxembourg)

## Text: X

Tycho's Projects screen was a grid of web-style cards. Now it's grouped rows like the Health summary: favourites first, then one section per status, each with a progress bar, "4 of 18 tasks", the lead and the last update. Sorting lives in the toolbar.

## Text: Bluesky

Tycho's Projects screen was a grid of web-style cards. Now it's grouped rows like the Health summary: favourites first, then one section per status, with a progress bar, "4 of 18 tasks" and the last update.

#SwiftUI #macOS

## Text: LinkedIn

I took the web out of Tycho's Mac UI.

Tycho is the task manager I'm building in SwiftUI for macOS and iOS. Its Projects screen used to be a grid of cards that looked like a web page. Now it's a grouped list in the style of the Health summary: favourites first, then one section per status, each project with a system label for its status, a progress bar in the project colour, "4 of 18 tasks", the lead and the last update. Sorting moved to a Sort By menu in the toolbar.

The date fields went the same way. The hand-drawn month calendar is gone: a date is the system date picker, and an optional date is a toggle plus a picker, like in Reminders. Dependencies are picked with system checkboxes.

The less I draw myself, the more it feels like it belongs on the Mac.

What's the first thing that tells you an app isn't native?

#SwiftUI #macOS #Tycho

## Screenshots

- `01-projects-summary.png`

---

# Tycho: system date pickers

Planned: X 25/11 18:00, Bluesky 25/11 18:00 (Europe/Luxembourg)

## Text: X

In Tycho, browsing to next month to pick a date used to write a date and close the popover. Now the date pill edits a draft in the system date picker, with Today and Clear Date, and only your pick is saved. An optional date is a toggle plus a picker, like Reminders.

## Text: Bluesky

In Tycho, browsing to next month to pick a date used to write a date and close the popover. Now the pill edits a draft in the system date picker, with Today and Clear Date. An optional date is a toggle plus a picker, like Reminders.

#SwiftUI #macOS

## Screenshots

- `02-date-picker.png`
