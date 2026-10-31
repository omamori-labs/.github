# Security

## Reporting a vulnerability

**Don't open a public issue.** Report it privately through GitHub instead, open the repository's **Security** tab and choose **Report a vulnerability**. Only the maintainers see it.

Include what you found, how to reproduce it, and which Omamori release and lazer version you used. You'll get a reply within a week. Once a fix is out, we're happy to credit you in the release notes if you'd like.

## What's in scope

- **Omamori itself:** the loader, the core, the API, the mod manager, and the `Omamori.ModBuildConfig` and `Omamori.Templates` packages.
- **The build and release pipeline:** anything that could get unintended code into a release, a package or a player's osu! folder.
- **Anything that lets a mod get past Omamori's rules,** like reading input during gameplay, or affecting gameplay in a way the API doesn't allow.

## What isn't

- **Mods made by other people.** C# mods run with the same access as osu! itself, so only install mods you trust. If you find a malicious one, report it to us anyway, so we can warn people.
- **osu! and osu!framework.** Report those to [ppy](https://github.com/ppy/osu/security).

## Supported versions

Only the latest release gets fixes, so update to it before reporting.
