# Aux Dalamud Repo

Custom Dalamud feed for Aux plugins.

## Feed URL

Use this in XIVLauncher -> Dalamud Settings -> Experimental -> Custom Plugin Repositories:

`https://raw.githubusercontent.com/Spoooki/AuxDalamudRepo/main/repo.json`

## Included Plugins

- **AuxEmotion** - auto-react to chat triggers with emotes, expressions, and macro slot actions.
- **AuxMarketboard** - import crafting/shopping lists and estimate gil cost from live Universalis market data.

## Repository Contents

- `repo.json` - feed manifest consumed by Dalamud.

## Release Update Checklist

1. Publish `AuxEmotion.zip` and/or `AuxMarketboard.zip` to the respective plugin GitHub Releases.
2. Update each plugin entry in `repo.json` (`AssemblyVersion`, `LastUpdate`, and download links if changed).
3. Commit and push to `main`.
