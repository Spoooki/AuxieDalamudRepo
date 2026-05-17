# Auxie Dalamud Plugin Repo

This repository hosts a custom Dalamud plugin feed JSON.

## Files

- `repo.json`: feed consumed by Dalamud custom repositories.

## How to publish

1. Create a GitHub repository (for example `Spoooki/AuxieDalamudRepo`).
2. Push this folder to that repository.
3. Make sure `repo.json` is reachable over HTTPS:
   - Raw URL example:
     - `https://raw.githubusercontent.com/Spoooki/AuxieDalamudRepo/main/repo.json`
4. In XIVLauncher -> Dalamud settings -> Experimental tab, add that URL as a custom plugin repository.

## Updating plugin releases

When you publish a new `AuxMarketboard` or `AuxEmotion` release:

1. Upload a zip artifact named `AuxMarketboard.zip` or `AuxEmotion.zip` to GitHub Releases.
2. Update `repo.json` fields:
   - `AssemblyVersion`
   - `LastUpdate` (unix timestamp seconds)
   - `DownloadLinkInstall`, `DownloadLinkUpdate`, `DownloadLinkTesting` (if URL changes)
3. Commit and push `repo.json`.

## Expected release zip content

`AuxMarketboard.zip` and `AuxEmotion.zip` should include:

- `<PluginName>.dll`
- `<PluginName>.json`
- any additional runtime files required by the plugin
