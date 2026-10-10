# Swift concurrency: the Stop button and AsyncStream

Project: `unified-dev` · Status: scheduled

## Schedule

| Channel | When (Luxembourg) | Buffer post | Link |
|---|---|---|---|
| X | Thu 15 Oct, 10:00 | `6aca09b7b07d37ac9769bba9` | |
| Bluesky | Thu 15 Oct, 10:00 | `6aca09d1bba9419ccbf8c195` | |

## Images

- `01-turn-running.jpg` from `unified-dev/agent/01-turn-running.png`

## Text: X, Bluesky

Swift concurrency lesson from Unified Dev: cancelling the Task that iterates an AsyncStream ends that stream for good. Our Stop button did exactly that, so every later agent turn ran with nobody listening. The runner now multiplexes its events instead. #Swift
