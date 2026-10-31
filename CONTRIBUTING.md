# Contributing to Omamori

Thanks for helping. This applies to every repository in omamori-labs unless a repository has its own `CONTRIBUTING.md`.

## rules

Nothing in Omamori, its API or its examples may help a player play. no aim assist, relax, auto-anything, timing or hit window changes, no reading or changing input during gameplay, and no looking at upcoming hit objects. A change that opens a way to do any of these won't be merged, however it's framed.

If you're unsure whether an idea crosses that line, open an issue and ask first.

## Before you start

- **Bugs:** open an issue with the bug form. Include the `[Omamori]` lines from osu!'s `logs/*.runtime.log`, they're usually enough to see what went wrong.
- **Features:** open an issue first, so we can agree before you spend time on it. Anything that adds to `Omamori.API` especially, once mods depend on something, it's hard to take back.
- **Small fixes** like typos or small bugs can go straight to a pull request.

## Building

Omamori needs the [.NET 10 SDK](https://dotnet.microsoft.com/download). You don't need osu!lazer installed, the build downloads the pinned lazer release and sets it up as a portable copy in `sandbox/lazer`.

```shell
./build.ps1    # Windows
./build.sh     # Linux and macOS
```

## Dependencies

Omamori is MIT licensed, and every dependency must be plainly OSI licensed with no extra terms. Check a package's license before adding it, not just its readme. A library that ships with Omamori also needs its license in `THIRD-PARTY-NOTICES.md`, and the build fails without it. Never ship a library the game already provides.

## Commits and pull requests

Commit messages follow [Conventional Commits](https://www.conventionalcommits.org): `type(scope): subject`, lowercase, no trailing period. The types are `feat`, `fix`, `refactor`, `perf`, `docs`, `style`, `test`, `build`, `ci` and `chore`. A breaking change gets a `!` and a `BREAKING CHANGE:` footer.

```
fix(core): hide the manager buttons when the mod manager breaks
```

Keep a pull request to one change. CI must pass before it's reviewed.

## Conduct

Everyone taking part follows the [code of conduct](CODE_OF_CONDUCT.md).
