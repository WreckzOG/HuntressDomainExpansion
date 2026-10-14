# Huntress Domain Expansion

## Endless Arrow Rain

Turn the battlefield into a crimson domain: an expanding black sphere, a dying cosmic sky, and relentless arrows raining down on everything caught inside.

An extra ability for **Huntress**. Deal damage to fill the meter, then press **T** to unleash **Endless Arrow Rain**. Your four normal skills remain available.

## Demo

[![Endless Arrow Rain gameplay preview](https://github.com/WreckzOG/HuntressDomainExpansion/releases/download/v1.0.1/huntress-domain-preview.gif)](https://github.com/WreckzOG/HuntressDomainExpansion/releases/download/v1.0.0/huntress-domain-demo.mp4)

**[Watch / download the gameplay demo (1:30)](https://github.com/WreckzOG/HuntressDomainExpansion/releases/download/v1.0.0/huntress-domain-demo.mp4)** · **[View full-size screenshot](https://github.com/WreckzOG/HuntressDomainExpansion/releases/download/v1.0.0/huntress-domain-screenshot.png)**

![Huntress inside Endless Arrow Rain](https://github.com/WreckzOG/HuntressDomainExpansion/releases/download/v1.0.0/huntress-domain-screenshot.png)

## What the domain does

- **62.5 m stationary sphere** centered where you cast.
- **4-second opening**, **12 active seconds**, then a **2-second visual collapse**.
- Enemies struck by the expanding shell are stunned once, subject to their normal stun immunity.
- During the active phase, enemies inside take repeated arrow hits: **6000% total damage per target** across 40 hits by default, before critical hits and item effects. Each hit has a **0.2 proc coefficient**.
- Huntress gains **50% attack speed** and **25% movement speed** during the active phase.
- Enemies inside are reduced to **30% movement speed** and **50% attack speed**. Supported hostile straight-moving projectiles are neutralized; friendly shots are preserved.
- A crimson cosmic environment, terrain effects, arrow rain, native sound effects, and a Frenzy status indicator accompany the cast.

## Earn every cast

Charge comes from damage dealt to enemies. The default requirement is **100 times your level-scaled base damage** (1200 damage at level 1). Charge persists between stages and does not build during the opening or active domain. Casting spends the entire meter.

## Installation

Install with **r2modman** or **Thunderstore Mod Manager** and launch the game modded. BepInExPack installs as a dependency.

For manual installation, install BepInExPack first, then copy the included `plugins/HuntressDomainExpansion` folder into `BepInEx/plugins`.

Restart the game after installing. This is a standalone Huntress release.

## Configuration and difficulty

After the first launch, edit `BepInEx/config/wreckzog.huntressdomainexpansion.cfg` with the game closed. The activation key, charge requirement, radius, duration, damage, frenzy bonuses, enemy slows, visuals, and audio are configurable.

To offset the domain's power, ordinary stage monster directors receive **1.75x ambient spawning income** for a solo Huntress by default. In co-op, the bonus scales with the fraction of participating players who are living Huntresses. This is spawning budget, not a guaranteed enemy-count increase. Boss directors, scripted encounters, and Simulacrum are excluded. Set `[Difficulty] DomainSpawnPressure = false` or `AmbientIncomeMultiplier = 1` to disable it.

## Compatibility

- Built against the current installed Windows version of Risk of Rain 2.
- Every co-op participant must install the **same version**. Gameplay is server-authoritative; a fresh multiplayer playtest of this standalone release is still pending.
- The full scenery projection uses **Direct3D 11**. Other rendering APIs fall back to geometric effects without the projected environment.
- Includes Huntress only; no other survivor domains are enabled.

Made with Codex / ChatGPT.
