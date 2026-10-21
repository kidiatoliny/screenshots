# dotsync: secret scanning before every push

## Text: X

dotsync keeps ~/.claude and ~/.codex in sync across my Macs with git. Before every push it scans the tracked files for API keys, tokens and private keys. If it finds one, the sync stops, it names the file, and I choose: ignore it or encrypt it with age.

## Text: Bluesky

dotsync keeps ~/.claude and ~/.codex in sync across my Macs with git. Before every push it scans the tracked files for API keys, tokens and private keys. If it finds one, the sync stops, it names the file, and I choose: ignore it or encrypt it with age.

#Swift #macOS

## Text: LinkedIn

I keep my AI agent setup (~/.claude and ~/.codex) in sync between my Macs with dotsync, a small menu bar app I built. Those folders keep credentials right next to the config, so most of the work went into not leaking them.

The ignore file ignores everything first and turns back on only real configuration, per tool. Before every push the tracked files are scanned for API keys, tokens and private keys, and a hit stops the sync and names the file. Credential files are either never tracked or encrypted with age, with a key pair per Mac, so adding a Mac never means copying a private key. The repositories are always private.

How do you move your dev setup to a new machine?

#macOS #Swift #DevTools
