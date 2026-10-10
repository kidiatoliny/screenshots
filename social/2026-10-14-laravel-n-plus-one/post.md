# Laravel: o problema N+1

Project: `tips` · Status: scheduled

## Schedule

| Channel | When (Luxembourg) | Buffer post | Link |
|---|---|---|---|
| X | Wed 14 Oct, 10:00 | `6aca07d3b07d37ac976974d1` | |
| Bluesky | Wed 14 Oct, 10:00 | `6aca07e6c4de2d2b1220a055` | |
| LinkedIn | not scheduled yet (weekly roundup) |  | |

Language: Portuguese (Cabo Verde).

## Images

None.

## Text: X, Bluesky

Dica de Laravel: se fazes um foreach nos posts e usas ->author dentro do loop, o Eloquent faz uma query por cada post. Com Post::with('author')->get() passam a ser 2 queries no total. É o famoso problema N+1. #Laravel
