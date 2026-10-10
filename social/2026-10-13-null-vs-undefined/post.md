# JS/TS: null vs undefined

Project: `tips` · Status: scheduled

## Schedule

| Channel | When (Luxembourg) | Buffer post | Link |
|---|---|---|---|
| LinkedIn | Tue 13 Oct, 08:30 | `6ac248e2d8dbde86e1473163` | |

X and Bluesky version published Tue 6 Oct.

## Images

None.

## Text: LinkedIn

A question I see a lot from people learning JavaScript: what's the difference between null and undefined?

undefined means a variable exists, but nothing was ever assigned to it.
null means someone set it to "empty" on purpose.

The way I think about it: undefined is "nobody set this", null is "someone decided this is empty".

In TypeScript, turning on strictNullChecks makes the compiler force you to handle both cases, which catches a lot of "cannot read property of undefined" errors before they reach production.

If there's a JS or TS question you'd like explained, leave it in the comments.
