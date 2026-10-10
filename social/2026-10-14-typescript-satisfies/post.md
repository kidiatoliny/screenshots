# TypeScript: satisfies

Project: `tips` · Status: scheduled

## Schedule

| Channel | When (Luxembourg) | Buffer post | Link |
|---|---|---|---|
| X | Wed 14 Oct, 18:00 | `6aca07e9ed92ed8fa5c31782` | |
| Bluesky | Wed 14 Oct, 18:00 | `6aca07f0b07d37ac97697935` | |
| LinkedIn | not scheduled yet (weekly roundup) |  | |

## Images

None.

## Text: X, Bluesky

TypeScript tip: satisfies checks a value against a type without widening it.

const routes = { home: '/', blog: '/blog' } satisfies Record<string, string>

TS still knows the exact keys, so routes.blgo is an error. #TypeScript
