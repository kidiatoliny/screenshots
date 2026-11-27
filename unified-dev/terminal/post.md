# Unified Dev: terminal colours

Planned: X 14/12 10:00, Bluesky 14/12 10:00, LinkedIn 14/12 08:30 (Europe/Luxembourg)

## Text: X

Unified Dev's terminal could keep the light colour palette in a dark window: the colours followed the app, not the terminal's own appearance. Now they follow the terminal, blue is actually blue, and every colour clears 4.5:1 contrast on its background.

## Text: Bluesky

Unified Dev's terminal could keep the light palette in a dark window: the colours followed the app, not the terminal. Now they follow the terminal's own appearance, and every colour clears 4.5:1 contrast on its background.

#Swift #macOS

## Text: LinkedIn

A terminal in a dark window was drawing with the light palette.

In Unified Dev, my macOS app for running coding agents in parallel, the terminal's ANSI colours were resolved outside the terminal's appearance, so they followed the app's current appearance instead of the terminal's own. Put a terminal in a dark window at the wrong moment and it kept the light colours.

Now the palette is picked from the terminal's effective appearance and reinstalled when the view moves to a window. While I was there: blue is a real blue, every colour clears 4.5:1 contrast on the measured background of its mode, and the bright colours differ from the normal ones.

One more detail: installing the palette resets any colour a running program set for itself, so it's only reinstalled when the choice actually changes.

#Swift #macOS #Accessibility

## Screenshots

- `unified-dev/terminal/01-ansi-dark.png`
- `unified-dev/terminal/02-ansi-light.png`
