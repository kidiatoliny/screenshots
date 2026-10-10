# Rust: the ? operator

Project: `tips` · Status: scheduled

## Schedule

| Channel | When (Luxembourg) | Buffer post | Link |
|---|---|---|---|
| X | Fri 16 Oct, 10:00 | `6aca09d8f91f772d458abb42` | |
| Bluesky | Fri 16 Oct, 10:00 | `6aca09def91f772d458abc24` | |
| LinkedIn | not scheduled yet (weekly roundup) |  | |

## Images

None.

## Text: X, Bluesky

Rust: ? returns early if a Result is Err and unwraps it if it's Ok.

let config = fs::read_to_string(path)?;

It also converts the error type through From, which is why it pairs so well with thiserror. #rustlang
