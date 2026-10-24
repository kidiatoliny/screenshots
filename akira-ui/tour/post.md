# Akira UI: the tour that read the last user's progress

## Text: X

Bug from Akira UI's product tours: a child component started its tour in its own effect, which runs before the parent's. The parent's effect was the one clearing the last user's progress, so the child read it. Now progress is read per signed-in owner.

## Text: Bluesky

Bug from Akira UI's product tours: a child component started its tour in its own effect, which runs before the parent's. The parent's effect was the one clearing the last user's progress, so the child read it. Now progress is read per signed-in owner.

#React #TypeScript

## Text: LinkedIn

A React bug I enjoyed tracking down in Akira UI's product tours.

Tours remember which version of each tour a user has seen. When the signed-in user changed, an effect in the provider cleared those recorded versions. But a child component that starts a tour in its own effect runs before that parent effect, so it read the previous user's progress.

The fix wasn't another effect. The provider now takes an owner (on Inertia, the shared auth user id) and reads and writes the recorded versions for that owner, so effect order and remounts stop mattering.

A second bug lived right next to it: a page restored from Inertia's prefetch cache came back with stale props and restarted a tour the user had just closed. The provider now keeps the higher version per tour, and the prefetch cache is dropped once a tour is recorded.

Have you been bitten by child effects running before the parent's?

#React #TypeScript #Inertia
