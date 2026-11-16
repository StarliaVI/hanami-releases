# Hanami Store

Finished recomp builds for the **Hanami** launcher, plus the little `store.json` file Hanami reads to know what's available.

**No game files are ever stored here.** Every recomp needs your own copy of the original game — Hanami tells you exactly which version (for example *USA region ISO*), checks your copy, and sets everything up for you.

## How it works

- `store.json` lists each recomp: its name, which game copy it needs, and the release tag prefix.
- Each build is a GitHub **Release** (for example `wfc-v1.0.0`) with one ZIP attached.
- Every ZIP contains a `hanami.json` describing the required game copy and how to launch it.

Hanami checks this page by itself — you don't need to download anything from here manually.
