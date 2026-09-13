<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=180&color=0:0B1021,45:2563EB,100:7C3AED&text=InfoLCD%20%E2%80%94%20Apex%20Advanced&fontColor=ffffff&fontAlignY=35&fontSize=32&desc=InfoLCD%20built%20for%20the%20APEX.Advanced!%20survival%20overhaul&descAlignY=57&descSize=16" />
</p>

<p align="center">
  <a href="https://steamcommunity.com/sharedfiles/filedetails/?id=3616712902"><img src="https://img.shields.io/badge/Steam%20Workshop-Subscribe-1B2838?style=for-the-badge&logo=steam&logoColor=white" alt="Steam Workshop" /></a>
  <a href="https://github.com/gitpush-mod/se-infolcd-apex-advanced/issues/new?template=bug_report.md&labels=bug"><img src="https://img.shields.io/badge/Report%20a%20bug-red?style=for-the-badge&logo=github&logoColor=white" alt="Report a bug" /></a>
  <img src="https://img.shields.io/badge/Space%20Engineers-1-0EA5E9?style=for-the-badge" alt="SE1" />
  <img src="https://img.shields.io/badge/Client--side%20only-checkmark-10B981?style=for-the-badge" alt="Client-side" />
</p>

> **"Everything InfoLCD does, speaking APEX.Advanced!'s language."**

**This is [InfoLCD — Apex Update](https://github.com/gitpush-mod/se-infolcd-apex-update), built to understand the [APEX.Advanced!](https://steamcommunity.com/sharedfiles/filedetails/?id=3570977190) survival overhaul.** Same scripts, same options, same client-side design — but it tracks HydroSolution instead of water, understands Nutrient Pellets and Composters, and adds a screen-overflow app the base mod doesn't have.

If you don't play with APEX.Advanced!, you want [Apex Update](https://github.com/gitpush-mod/se-infolcd-apex-update) instead.

<p align="center">
  <img src="InfoLCD - Apex Advanced/thumb.jpg" alt="InfoLCD Apex Advanced preview" width="480" />
</p>

## 🧭 Which one do I install?

**One or the other — never both.** The two mods register the same script names, so running them together will conflict.

| You play... | Install |
|---|---|
| With **APEX.Advanced!** | **This mod** |
| Vanilla, or any other setup | [**Apex Update**](https://github.com/gitpush-mod/se-infolcd-apex-update) |

Everything else is identical. As of **v2.0** the two share a single codebase, so features and fixes land in both — you are not trading anything away by picking the one that matches your world.

## ✨ What APEX.Advanced! support actually means

| | What changes |
|---|---|
| **HydroSolution** | Recognised as the water gas type — tank levels, capacity, and production/consumption rates. Bars read `HydS`, not `H2O` |
| **Nutrient Pellets** | Tracked on the Farming screen with its own bar, and shown as the Irrigation System's feedstock (the base mod reads Ice there) |
| **Organic** | Tracked for composting, and deliberately kept off the Ore screen so it doesn't clutter mining readouts |
| **Composters** | Kept out of the assembler list where they'd be noise, while still appearing under Production on the Systems screen and in Damage Control when damaged |
| **Apex consumables** | Bio-Nutri-Paste, Sparkling Water, MycoBoost and Fruit Tea recognised by name |

## 📺 Extension — the one extra app

`$IOS LCD - Extension` is exclusive to this variant. Point it at another LCD by name and it renders **that screen's overflow** — so a long cargo or production list can spill onto a second panel instead of being cut off.

- Inherits every setting from the parent screen; you only set `SearchId`
- **Chainable** — extend an extension for page 3, 4, and beyond
- `SurfaceIndex` picks which screen to read on multi-screen blocks like cockpits

## 🚀 Install

1. [Subscribe on the Workshop page](https://steamcommunity.com/sharedfiles/filedetails/?id=3616712902)
2. Enable the mod when creating or loading a world
3. Place an Apex LCD block, open its terminal, and select an `$IOS LCD - <thing>` script

Client-side only, with no world-side setup. Safe to add to an existing world.

## 🎯 Compatibility

- ✅ **Space Engineers 1** — actively maintained
- ✅ **APEX.Advanced!** — what this variant exists for
- ✅ **Multiplayer + dedicated servers** — client-side, does nothing server-side
- ✅ **Existing saves** — safe to add or remove; screens fall back to blank if disabled
- ✅ **Other LCD mods** — coexists, since it only touches Apex LCD blocks
- ❌ **InfoLCD — Apex Update** — do not run both; they register the same scripts
- ⚠️ **Non-Apex LCD blocks** — not supported by design

Works fine without APEX.Advanced! installed — the Apex-specific readouts simply find nothing — but there's no reason to choose this variant in that case.

## 🐛 Found a bug?

- **[Open an issue with the bug report template](https://github.com/gitpush-mod/se-infolcd-apex-advanced/issues/new?template=bug_report.md&labels=bug)** — best for reproducible bugs; they get tracked and fixed
- **[Leave a Steam Workshop comment](https://steamcommunity.com/sharedfiles/filedetails/?id=3616712902)** — better for quick "does this work with X?" questions

If the game crashes outright with nothing in the log, say so. That detail is a clue in itself, and it's exactly how the v2.0 crash fix was found.

## 🧑‍🤝‍🧑 Sibling mod

[**se-infolcd-apex-update**](https://github.com/gitpush-mod/se-infolcd-apex-update) is the mainline variant for worlds without APEX.Advanced!. Both are maintained in parallel from the same codebase.

## 🙌 Credits

- **Author:** [Chris Carpenter (Godimas101)](https://github.com/Godimas101)
- **Built with:** the Space Engineers modding SDK + a lot of iteration on real ships
- **Sturmgrenadier Hosting** — [sghq.org](https://sghq.org/), the SE server community that stress-tests these mods

## 🧡 Support

InfoLCD is free and always will be. If it saves you time on your next build, consider supporting on **Patreon** — it's more a running project log than a tip jar. Behind-the-scenes updates, in-progress mod work, and dev notes across everything under [`gitpush-mod`](https://github.com/gitpush-mod) and [The Canadian Space](https://thecanadian.space).

[![Support on Patreon](https://raw.githubusercontent.com/Godimas101/personal-projects/main/patreon/images/buttons/patreon-medium.png)](https://patreon.com/Godimas101)

---

*Part of the [`gitpush-mod`](https://github.com/gitpush-mod) mod collection. Made with ♥ (and a lot of coffee) by Godimas + Claude.*
