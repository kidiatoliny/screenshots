# Swift concurrency: the Stop button and AsyncStream

## Text: X, Bluesky

Swift concurrency lesson from Unified Dev: cancelling the Task that iterates an AsyncStream ends that stream for good. Our Stop button did exactly that, so every later agent turn ran with nobody listening. The runner now multiplexes its events instead. #Swift
