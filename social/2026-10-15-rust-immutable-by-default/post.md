# Rust: immutable by default

Project: `tips` · Status: scheduled

## Schedule

| Channel | When (Luxembourg) | Buffer post | Link |
|---|---|---|---|
| LinkedIn | Thu 15 Oct, 08:30 | `6ac248e9d8dbde86e147328f` | |

X and Bluesky version published Fri 9 Oct.

## Images

None.

## Text: LinkedIn

Why are variables immutable by default in Rust?

let count = 0; can't be changed later. If you need that, you have to write let mut count = 0;

It feels strict at first, but most values in a program never change after they're set. Making mutation opt-in means that when you see mut, you know to pay attention to that variable.

Coming from TypeScript, it's a bit like const being the default and let being the exception.

Did this take you a while to get used to?
