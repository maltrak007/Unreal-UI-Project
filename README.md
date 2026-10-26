# Unreal UI Project — Industry-Standard FPS HUD

University project (U-TAD) focused on building **industry-quality game UI** in Unreal Engine with C++ and UMG. It takes a first-person shooter template and layers a complete, polished HUD on top.

| | |
|---|---|
| **Engine** | Unreal Engine (C++ / UMG) |
| **Module** | `UTAD_UI_FPS` |
| **Focus** | UI/UX programming, feedback and game feel |

## Features

- **Skill tree** (`SkillTree`) — progression screen for unlocking upgrades.
- **Dynamic crosshair** (`Crosshair`) — reacts to player state, such as movement and firing.
- **Weapon reload bar** (`ReloadBar`) and **ammo indicators** (`AmmoCounter`).
- **Player and enemy health bars** (`PlayerHealthBar`, `EnemyHealthBar`).
- **Hit marker** (`PlayerHitMarker`) — instant feedback when a shot lands.
- **Danger warning** — alerts the player when threatened.
- **Splash screen** (`SplasherScreenWidget`) and a central **`PlayerHUD`** that composes every widget.

## Code map

```
Source/UTAD_UI_FPS/
  UI/                       All UMG widget classes listed above
  TP_WeaponComponent.*      Weapon logic (fire, reload) that drives the HUD
  TP_PickUpComponent.*      Pick-up handling
  UTAD_UI_FPSCharacter.*    Player character
  UTAD_UI_FPS_Enemy.*       Enemy used to test health bars and hit markers
  UTAD_UI_FPSProjectile.*   Projectile
  UTAD_UI_FPSGameMode.*     Game mode
```

## Running it

1. Open `UTAD_UI_FPS.uproject` with a matching Unreal Engine version.
2. Generate project files and build the `UTAD_UI_FPSEditor` target.
3. Press **Play** and try the skill tree, reload bar and crosshair in the test level.

## Author

**Gonzalo Liñán Aldana** — [GitHub](https://github.com/maltrak007)
