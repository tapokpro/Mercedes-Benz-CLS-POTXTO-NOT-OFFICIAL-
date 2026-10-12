# Mercedes-Benz-CLS-POTXTO-NOT-OFFICIAL-
Mercedes Benz CLS By POTXTO price fixing for RLS Career Overhaul 
# CLS-Class (C218/X218) – RLS Career Overhaul Dealership Fix

An **unofficial compatibility patch** that lets the *Mercedes-Benz CLS-Class C218, W218, X218* vehicle mod appear for sale in **RLS Career Overhaul** (BeamNG.drive career mode).

> **This is not the mod itself, and I am not its author.**
> The CLS mod was created by **omg_potxto** (potxto). All models, parts, JBEAM files and configurations belong to the original author.
> This repository contains only edited `info.json` / `info_*.json` metadata files. You must install the original mod first.

Original mod: `https://www.modland.net/beamng.drive-mods/cars/mercedes-benz-cls-class-c218x218-potxto.html`
Original Creator: 'https://www.beamng.com/members/omg_potxto.534766/'

## The problem

In RLS Career Overhaul the CLS never showed up in dealerships or used car lots. The metadata files that the career dealership system reads were incomplete:

- no `Value` (price) in `info.json` or in any config,
- no `Years` (model year range),
- no `Population` in the main `info.json`, and `Population` was only `50` in every config, which is too low to be picked for sale.

The part prices inside the `.jbeam` files were already fine and are **not** the cause, so the JBEAM files are not changed.

## What this patch changes

Only metadata files are touched. Nothing else in the mod is modified.

### `info.json` (main vehicle)

| Field | Value |
|---|---|
| `Value` | 65000 |
| `Population` | 3000 |
| `Years` | 2011 – 2018 |
| `Insurance Class` | `dailyDriver` |
| `Regions` | `["northAmerica"]` |

### `info_*.json` (134 configs)

- **`Years`**: 2011–2014 for *Dorestyling* configs, 2014–2018 for *Restyling* configs.
- **`Population`**: 3000 for normal factory versions, 800 for tuned or rare versions (Brabus, RENNtech, Vorsteiner, GAD Motors, WENGALLBI, Stage 1–3, Drift, Off-Road, Dead Car and similar), so those appear less often.
- **`Value`**: estimated from the model name, since the `Power` field is identical in all configs.

| Version | Approx. price |
|---|---|
| CLS250 / 250d | 38,000 |
| CLS350 | 45,000 |
| CLS400 | 55,000 |
| CLS500 / 550 | 62,000 |
| CLS63 AMG | 78,000 |
| CLS63 AMG S | 92,000 |
| RENNtech, Vorsteiner, GAD, WENGALLBI, Seven Force, DTK1000 | 115,000 |
| Brabus | 125,000 – 170,000 |
| Dead Car | 7,000 |

Modifiers: Wagon +3,000; each Stage level +6,000; "Beaten" versions ×0.45; Drift versions ×0.8.

All prices are my own estimates. Edit the `Value` field in any `info_*.json` to change them.

## Installation

1. Install the original CLS mod and RLS Career Overhaul.
2. Close BeamNG.drive.
3. **Back up** the original `info.json` and `info_*.json` files in `vehicles/clsomg/`.
4. Copy the files from this repository into `vehicles/clsomg/`, overwriting the originals.
5. Clear the game cache if you have one, then start the game.

## Notes and limitations

- **Not guaranteed.** Each RLS dealer has its own rules, such as price and year limits. For example, one dealer's maximum price is 65,000, so more expensive versions can only appear at other dealers or private sellers.
- Dealers show only some cars at a time. Different versions appear as the stock rotates over in-game time.
- The `Insurance Class` and `Regions` values are best guesses based on commonly used defaults.
- If the mod is updated by its author, the update may overwrite these files. Reapply the patch afterwards.
- The files have been checked to be valid JSON with the new fields. In-game results may vary with your BeamNG and RLS versions.

## Credits

- **omg_potxto** – author of the CLS-Class mod (all vehicle content)
- **RLS Modding** – RLS Career Overhaul

## License / permission

I do not own the original mod. These files are edited copies of metadata from it. Before using or redistributing, check the original author's terms. If the author asks for this repository to be changed or removed, I will do so.
