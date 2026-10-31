<div align="center">

<h1>Omamori</h1>

[![release](https://img.shields.io/github/v/release/omamori-labs/Omamori?include_prereleases&style=for-the-badge&color=f7a6bf&labelColor=fff4f7&label=release)](https://github.com/omamori-labs/Omamori/releases)
[![templates](https://img.shields.io/nuget/vpre/Omamori.Templates?style=for-the-badge&color=f7a6bf&labelColor=fff4f7&label=templates)](https://www.nuget.org/packages/Omamori.Templates)
[![.NET 10](https://img.shields.io/badge/.NET-10-f7a6bf?style=for-the-badge&labelColor=fff4f7)](https://dotnet.microsoft.com/download)
[![license](https://img.shields.io/badge/license-MIT-f7a6bf?style=for-the-badge&labelColor=fff4f7)](https://github.com/omamori-labs/Omamori/blob/main/LICENSE)
[![discord](https://img.shields.io/badge/discord-come%20say%20hi-f7a6bf?style=for-the-badge&logo=discord&logoColor=d9487a&labelColor=fff4f7)](https://discord.gg/JBr3QxgDJ)
[![ko-fi](https://img.shields.io/badge/ko--fi-buy%20us%20a%20coffee-f7a6bf?style=for-the-badge&logo=kofi&logoColor=d9487a&labelColor=fff4f7)](https://ko-fi.com/catforgor)

<b>
<a href="https://github.com/omamori-labs/Omamori/releases">download</a>
&nbsp;&middot;&nbsp;
<a href="#get-started">make a mod</a>
&nbsp;&middot;&nbsp;
<a href="https://discord.gg/JBr3QxgDJ">discord</a>
&nbsp;&middot;&nbsp;
<a href="https://github.com/omamori-labs/.github/blob/main/CONTRIBUTING.md">contribute</a>
&nbsp;&middot;&nbsp;
<a href="https://ko-fi.com/catforgor">donate</a>
</b>

<br>

Omamori is a modding framework for Osu!Lazer. Mods are small C# assemblies built against a tiny API, so they keep working when lazer updates. It loads through lazer's own ruleset loading, and the game itself is never touched.

</div>

<br>

> [!NOTE]
> Omamori is an early prerelease. The API is still growing, and there are rough edges.

## What mods can do

- **Add UI** to the main menu, or an overlay above everything
- **React to the game**: screens, beatmaps, rulesets and mods, plays and scores, music, skins, the library, overlays and multiplayer rooms. Every event is read only.
- **Look at finished plays**: every judgement and the replay, for hit error graphs, cursor paths and other visualisers
- **Have settings** that players change in Omamori's mod manager

## Get started

<details>
<summary><b>I want to play with mods</b></summary>
<br>

Download the latest release from [Omamori's releases](https://github.com/omamori-labs/Omamori/releases) and extract it into osu!'s data folder.

</details>

<details>
<summary><b>I want to make a mod</b></summary>
<br>

**Starting a new mod:** install the template from NuGet, with the version from its [NuGet page](https://www.nuget.org/packages/Omamori.Templates) (it's a prerelease, so the version has to be given), then make a mod from it:

```shell
dotnet new install Omamori.Templates::<version>
dotnet new omamori-mod -n MyMod --modId yourname.mymod --modAuthor you
```

**Adding Omamori to a project you already have:** add the build package from NuGet. Your project also needs a `mod.json`, the template's is a good one to copy.

```shell
dotnet add package Omamori.ModBuildConfig --prerelease
```

</details>

<details>
<summary><b>I want to help with Omamori</b></summary>
<br>

Read [CONTRIBUTING.md](https://github.com/omamori-labs/.github/blob/main/CONTRIBUTING.md), then come say hi on [Discord](https://discord.gg/JBr3QxgDJ).

</details>

## Repositories

| Repository | |
|---|---|
| [Omamori](https://github.com/omamori-labs/Omamori) | the framework: the loader, the API mods build against, the mod manager, the build packages and the mod template |
| [.github](https://github.com/omamori-labs/.github) | The profile for our organization |

<br>

<div align="center">
<sub>made by Evie Fogarty</sub>
</div>
