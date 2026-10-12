# Anchor: iCloud Keychain sync in the iOS Simulator

## Text: X, Bluesky

I'm building Anchor, which syncs my AI coding sessions' context to my iPhone, encrypted with a key in iCloud Keychain. In the Simulator the app never found the key: its keychain sync switch won't stay on. A real iPhone did. Is that a Simulator limitation, or a setting I missed?

## Text: LinkedIn

I'm building Anchor, an app that keeps the context of my AI coding sessions (decisions, sessions, what each project already knows) in sync between my Mac and my iPhone. The Mac already publishes that context to iCloud, encrypted with a key it stores as a synchronizable keychain item, and iCloud Keychain carries the key to my other devices.

The next step is the iPhone reading that context. Before writing any receive code, I checked whether the iPhone could see the key the Mac created. I built a throwaway probe: one screen that calls the key store's existingKey() and prints "found" or "not found".

In the iOS Simulator it said "not found", before and after I signed in to my Apple Account. Settings showed Passwords as Off, and the "Sync this iPhone" switch under Passwords & Keychain went back to off each time I turned it on.

I installed the same build on my iPhone and it said "found" on the first launch.

For now I test anything that depends on iCloud Keychain sync on a real device. The Simulator still works for the states around it, like "waiting for the key".

Is this a known limitation of the Simulator, or is there a setting I missed?
