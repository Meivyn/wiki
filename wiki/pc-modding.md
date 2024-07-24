---
prev: false
next: false
description: Learn how to mod Beat Saber on PC!
---

# PC Modding

## Preface

::: danger DISCLAIMER
By choosing to use mods, you understand that:

- You may experience problems that don't exist in the vanilla game. Most bugs, crashes, and performance issues are due
  to mods.
- Mods are subject to being broken by updates and that's normal - be patient and respectful when this happens,
  as modders are volunteers with real lives.
- Beat Games employees aren't purposefully trying to break mods. They wish to work on the codebase and sometimes this
  breaks mods that depend on it.

Do not attack the game developers for issues related to mods, and vice versa - modders and game developers
are two separate groups. Just don't be a jerk.
:::

::: warning
This guide is for PC modding on Windows.  
If you have a Quest and play on standalone, see the [Quest Modding page](/quest-modding.md).  
If you're on Linux, check out the [Linux Modding page](./linux-modding.md)
:::

Beat Saber natively supports custom songs, so if that's all you're looking for, you don't require mods!
It's a wise idea to install `SongCore` though, as this mod expands upon the base game functionality to improve
loading times and fixes some issues.

If you run into problems at any point, please head to the [support page](./support/) and see if you can identify what
went wrong before asking in the Discord server. Chances are, your answer is on that page!

::: warning I watched a video tutorial on YouTube, but I got stuck/it didn't work. What gives?
We at BSMG **strongly** advise against using any video tutorials for modding. Often, we find that they are either
outdated or contain incomplete, erroneous, or straight up incorrect information.

Instead, you should follow the written guides here on the wiki or seek out help in the [BSMG Discord](https://discord.gg/beatsabermods).
:::

:::tip NOTE
The latest version of Beat Saber might not be compatible with mods.

Visit the [Downgrading](#downgrading) section on this page for more information.
:::

## Installers

### BSManager

> **THIS IS CURRENTLY THE RECOMMENDED MOD INSTALLER.**

An all-in-one tool that lets you easily manage Beat Saber versions, maps, mods, and even more. Get it on its [website](https://www.bsmanager.io/).

![BSManager](/.assets/images/beginners-guide/bsmanager.jpg)

### BeatSaberModManager

Yet another mod installer for Beat Saber, heavily inspired by Mod Assistant.
It strives to look more visually appealing and support both Windows and Linux, while still being as feature-rich as Mod Assistant.
Get it on [affederaffe's GitHub](https://github.com/affederaffe/BeatSaberModManager/releases/latest).

![BeatSaberModManager](/.assets/images/beginners-guide/beatsabermodmanager.png)

### Mod Assistant

::: danger DEPRECATION NOTICE
Mod Assistant reached its end of life, as it has bugs and is no longer maintained.
We recommend switching to [BSManager](#bsmanager)
which has the same modding capabilities as Mod Assistant.
:::

A simple and lightweight Beat Saber mod installer. Get it on [BSMG's GitHub](https://github.com/bsmg/ModAssistant/releases/latest).

![Mod Assistant](/.assets/images/beginners-guide/modassistant.png)

## How to get more songs

::: tip
Most maps in the "Top All", "Rating", "Downloads" or "Plays" sort filters were created before
good mapping practices were established. Try downloading songs released between late 2019 and now to get the best
custom levels experience.
:::

::: warning
It is a good idea to back up your `CustomLevels` folder periodically!

This folder is located in your game install: `Beat Saber/Beat Saber_Data/CustomLevels`
:::

### In-game Downloader

The [BeatSaverDownloader](https://github.com/Top-Cat/BeatSaverDownloader) mod allows you to download maps using the
`MORE SONGS` menu button on the `Mods` menu screen. This pulls maps directly from [BeatSaver](https://beatsaver.com).

A similar and more in-depth alternative is [BetterSongSearch](https://github.com/kinsi55/BeatSaber_BetterSongSearch).

### BeatSaver

[BeatSaver](https://beatsaver.com) is the master repository of custom songs made by the community.
Many other tools and sites enhance the experience of downloading custom songs, but this site is where they are stored.
To install songs downloaded from the site, unzip them into a folder and place it into `Beat Saber/Beat Saber_Data/CustomLevels`.
You can also use in-game downloaders, the OneClick™ Install feature, or in the "Maps"
tab of BSManager.

To enable and use BSManager's OneClick™ Install see the picture below:

![BSManager](/.assets/images/beginners-guide/bsmanager-oneclick.png)

To enable and use Mod Assistant's OneClick™ Install see the picture below:

![Mod Assistant](/.assets/images/beginners-guide/modassistant-oneclick.png)

To install songs on BeatSaver with the OneClick™ Install, press this button:

![BeatSaver](/.assets/images/beginners-guide/beatsaver-oneclick.png)

### Beast Saber

[BeastSaber](https://www.bsaber.com) is a site that tries to help make finding fantastic maps to play easier.
The most used feature is the "Recently Curated Maps" feed where a team of curators plays through most songs released
each day and recommends the ones that meet a minimum quality standard and have that subjective "fun factor" for them.
BeastSaber also features the most recent maps from verified mappers, a collection of Maps of the Week, and
featured/curated map packs/playlists.

### Song Management Apps

Currently, the only known working application to manage custom levels is [BSManager](#bsmanager).

### Playlists

You need to install the [PlaylistManager](https://github.com/rithik-b/PlaylistManager/releases/latest) mod.

Then you can either:

- Install the playlist through your mod manager.
- Place the playlist file into `Beat Saber/Playlists`, select it in-game, then hit the `DOWNLOAD` button to download all
  songs.

You should see the playlist next to the Custom Levels pack in-game. The mod also supports managing playlists.

## Install Folder

_Where is Beat Saber installed?_

### Default Location

|        |                                                                              |
| ------ | ---------------------------------------------------------------------------- |
| Steam  | `C:\Program Files (x86)\Steam\steamapps\common\Beat Saber\`                  |
| Oculus | `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

### Other Locations

**If you have moved your install folder to a different drive, it might be in the location below.**
Replace the drive letter `F` with the drive your game is installed on.
| | |
| --- | --- |
| Steam | `F:\SteamLibrary\steamapps\common\Beat Saber\` |
| Oculus | `F:\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

## Manual Installation

::: warning STAY SAFE WHEN INSTALLING MODS
Modding your game with unverified mods such as mods found in the `#pc-mods` channel comes with risks, including the
possibility for malicious software that acts like a regular mod. Security suites aren't infallible,
and a malware doesn't need administrator privileges to be harmful.

However, Beat Saber will **NEVER** ask you to run it as administrator.

If you've downloaded and installed a mod and you get the
User Account Control prompt, **DO NOT** click accept, and please report this. If you're unsure if something you installed
is malware or not, **_please ask someone in our discord_**.
:::

A mod manager is the recommended way to install mods. See the section [above](#installers).
If you already have a modded installation and just need to install mods that are not available in the installer,
skip to step 4.

1. Download [BSIPA](https://github.com/bsmg/BeatSaber-IPA-Reloaded/releases). If your game version is `1.29.1` or below,
   get [this version](https://beatmods.com/uploads/64264fed368d841027494b36/universal/BSIPA-4.2.2.zip) instead.
2. Navigate to your [install folder](#install-folder) and extract the contents of BSIPA into it.

   ![Directory Clean](/.assets/images/beginners-guide/directory-clean.png 'Directory Clean')
   ![Directory Ipa](/.assets/images/beginners-guide/directory-ipa.png 'Directory Ipa')

3. Double click `IPA.exe` to install BSIPA. Any mods in the `Plugins` folder will now be loaded when starting the game.
   If there are errors, it's possible that you didn't follow step 2 correctly.

   ![Directory Patched](/.assets/images/beginners-guide/directory-patched.png 'Directory Patched')

4. Download the mod(s) you wish to install, whether it be from GitHub, the [BSMG Discord](https://discord.com/invite/beatsabermods)
   `#pc-mods` channel, [BeatMods](https://beatmods.com/#/mods) or other sources.
   **Make sure to download any dependencies required by the mod.**

   ![Directory Plugins](/.assets/images/beginners-guide/directory-plugins.png 'Directory Plugins')

5. Some mods have installation instructions, some don't. Generally you can just drag and drop the zip contents into your
   Beat Saber install directory, and the files should go into the corresponding folders.

## Downgrading

Check `#modding-announcements` in [BSMG](https://www.discord.gg/beatsabermods) to see if the latest version is moddable.
If it is not, you can follow these tutorials to downgrade to a moddable version. We recommend using BSManager.

### Downgrading Tools

For Steam you can use [BSManager](https://www.bsmanager.io/).

For Oculus Store (on Rift and Rift S) you can use either:

- [BSManager](https://www.bsmanager.io/)
- [OculusDowngrader](https://computerelite.github.io/tools/Oculus/OculusDowngraderGuide.html)

### Legacy Branch

You can use the legacy branch method as an alternative if you want to downgrade to version `1.34.2` or `1.29.1`.
You do not need to use the legacy branch if you use one of the above downgrading tools instead.

::: warning
If you wish to downgrade to version `1.29.1`, make sure you **first** uninstall BSIPA through your mod manager!
:::

#### Steam Users

1. Right click Beat Saber in the game library
2. Select Properties
3. Select Betas in the window
4. Select either the `1.34.2_legacy` or the
   `legacy1.29.1_unity_ver2019.4.28f1` branch
5. Let the download complete then run the game once
6. Follow the regular modding process

![Steam Branch Setting](/.assets/images/beginners-guide/1291_steambranch.jpg 'Steam Branch Setting')

#### Oculus Store Users

1. Go to the Beat Saber store page
2. Scroll down to `Versions + Release Notes`
3. Click on the word `(LIVE)` next to the current version number
4. Select either the `1.34.2_legacy` or the
   `legacy1.29.1_unity_ver2019.4.28f1` branch
5. Let the download complete and run the game once
6. Follow the regular modding process

![Oculus Branch Setting](/.assets/images/beginners-guide/1291_oculusbranch.jpg 'Oculus Branch Setting')

## How to uninstall mods

It is recommended to uninstall mods with your mod manager. You can also remove `.dll` files from your `Plugins` folder.

## Where to go from here

- [Grips and Tricks](./grips-and-tricks.md)
- [Making Beatmaps](/mapping/)
- [Custom Sabers](/models/custom-sabers.md)
- [Custom Avatars](/models/custom-avatars.md)
- [Custom Platforms](/models/custom-platforms.md)
- [Play Customs in Multiplayer](https://discord.com/invite/gezGrFG4tz)
- [Making Mods](/modding/)

## Have questions?

Visit the support channels in the [BSMG Discord](https://discord.gg/beatsabermods)!
