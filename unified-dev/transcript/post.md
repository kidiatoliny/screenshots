# Unified Dev: reply to a selection

Planned: 2026-11-11 18:00 Luxembourg (X + Bluesky)

## Text: X

Replying to part of an agent's answer in Unified Dev used to write > lines into your draft. Now selecting a passage opens a small card with the quote and a field for your reply. The quote waits above the composer as a card, and you can hold several.

## Text: Bluesky

Replying to part of an agent's answer in Unified Dev used to write > lines into your draft. Now selecting a passage opens a small card with the quote and a field for your reply. The quote waits above the composer as a card, and you can hold several.

#Swift #macOS

## Screenshots

- `01-reply-card.png`
- `04-held-quotes.png`

---

# Unified Dev: select across one answer

Planned: 2026-11-13 10:00 Luxembourg (X + Bluesky)

## Text: X

An answer in Unified Dev is now one text view, so a selection runs across paragraphs, lists, code blocks and tables. It copies in the shape it's drawn: list markers, code lines, table cells split by tabs. Long code lines wrap now too.

## Text: Bluesky

An answer in Unified Dev is now one text view, so a selection runs across paragraphs, lists, code blocks and tables. It copies in the shape it's drawn: list markers, code lines, table cells split by tabs. Long code lines wrap now too.

#Swift #macOS

## Screenshots

- `02-selection.png`
- `05-paste-shape.png`

---

# Unified Dev: background tasks

Planned: 2026-11-21 10:00 Luxembourg (X + Bluesky)

## Text: X

Background tasks in Unified Dev now split into Running and Finished, with a Clear button that hides what has finished. A background command opens as a sheet with its status, type, duration, the command and its output.

## Text: Bluesky

Background tasks in Unified Dev now split into Running and Finished, with a Clear button that hides what has finished. A background command opens as a sheet with its status, type, duration, the command and its output.

#Swift #macOS

## Screenshots

- `03-tasks-sheet.png`

---

# Unified Dev: confirm before running, invisible characters spelled out

Planned: LI 04/12 08:30, X 04/12 18:00, Bluesky 04/12 18:00 (Europe/Luxembourg)

## Text: X

An orchestrator in Unified Dev can put a shell command in a code block with a Run button. A command that only reads runs at once. Anything else asks first, and the confirmation spells out every invisible character, so a bidi override or a zero-width joiner can't disguise it.

## Text: Bluesky

An orchestrator in Unified Dev can put a shell command in a code block with a Run button. A read runs at once. Anything else asks first, and the alert spells out every invisible character, so a bidi override can't disguise it.

#Swift #AISecurity

## Text: LinkedIn

A command you are asked to confirm should look exactly like the command that will run.

In Unified Dev, the orchestrator agent can answer with a shell command in a code block, and there's a Run button on it. A command on the closed list of reads runs at once. Anything else opens a native alert with the whole command, its folder and a warning that it may change files, and runs only if you confirm.

The detail I care about: the alert keeps only characters that draw something and spells out the rest. Control characters, bidi overrides, zero-width spaces, combining marks, blank letters, in the command and in the folder, with a count of how many it spelled out. Text can say one thing on screen and another to the shell. The confirmation shouldn't be where that happens.

Would you have caught a zero-width character in a command?

#Swift #macOS #AISecurity

## Screenshots

- `06-confirm-invisible.png`
