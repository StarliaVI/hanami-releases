# Hanami Store

Finished recomp builds for the **Hanami** launcher, plus the little `store.json` file Hanami reads to know what's available.

**No game files are ever stored here.** Every recomp needs your own copy of the original game — Hanami tells you exactly which version (for example *USA region ISO*), checks your copy, and sets everything up for you.

## How it works

- `store.json` lists each recomp: its name, which game copy it needs, and its builds.
- Builds live in `builds/<recomp>/` as ZIPs. Every ZIP contains a `hanami.json` describing the required game copy and how to launch it.
- `art/` holds original store artwork (never game box art).
- `hanami/` is how Hanami updates itself (3.2.2 and newer): `update.json` lists the app's files and their SHA-256, and `hanami/files/<sha256>` holds each file. Hanami only downloads the files that changed, checks every one, and installs the update inside its own data folder. (`latest.json` is retired.)

Hanami checks this page by itself — you don't need to download anything from here manually.
