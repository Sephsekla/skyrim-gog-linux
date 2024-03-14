# Skyrim GOG Linux Setup

> Setup and configuration for the GOG version of Skyrim on Linux, with MO2 support.

## Requirements

- **[Bottles](https://usebottles.com/)** - A Wine-based solution to run Windows applications in a sandbox
- **[GOG Galaxy](https://www.gog.com/galaxy) (optional)** - If you're going to use Galaxy, I'd recommend using [Bottles' own installer script](https://usebottles.com/app/#gog)
- **Skyrim offline installers** (optional, use if you're not using Galaxy)
- **[Mod Organizer 2 v2.4.4](https://github.com/ModOrganizer2/modorganizer/releases/tag/v2.4.4)** - Version 2.5 won't work[^1].
- **[Mod Organizer 2 Skyrim plugin](https://www.nexusmods.com/skyrimspecialedition/mods/6194?tab=files)** - you want `SSE GOG and EGS Support - Mod Organizer 2.4.x`

## Steps

- First, install Bottles, and set up a new Bottle. I'd recommend importing [the included configuration file](./bottles/backup_Skyrim.yml), since this is my working setup. You can always tweak it later. At a minimum, you'll need to have the latest dotnet, d3dx11 and vcredist dependencies installed in Dependencies, but your experience may vary.
- Now install Skyrim. Either install GOG Galaxy via Bottles' script (recommended) and download Skyrim, or run the offline installer exe in the bottle.
- Launch Skyrim and start a new game, to confirm everything works and create your config files.
- Now install MO2. In the bottle, run the MO2 exe file from the releases page, and complete setup. Be sure to choose a *portable installation*.
- Once installation is complete, replace the Skyrim plugin in the MO2 plugins folder with the download from NexusMods. This will enable GOG support.

## Usage & Gotchas

- You're now done! Boot up MO2, setup your mods and profiles and play the game. Happy modding!
- I haven't successfully got downloads from the Nexus working yet, this may be doable if you use a browser inside the Bottle, but for now you'll need to download mods manually and install them in MO2 from their archives.

[^1]: If you do manage to get it working, please do let me know!