# DAK GaggiMate Profiles

Pressure profiles for GaggiMate / Gaggiuino-style espresso workflows, tuned for selected DAK coffees.

## What this repository is

This repository is a public profile library for GaggiMate PRO JSON pressure profiles focused on DAK coffees. It is intentionally minimal and documentation-first so users can quickly find, load, and test profiles.

## What GaggiMate profiles are

GaggiMate profiles are structured JSON shot programs that define machine behavior across extraction phases (for example preinfusion, ramp, hold, and finish). A profile controls time, pump behavior, valve state, and temperature targets used during a shot.

## Folder structure

```text
.
├── docs/
│   └── profile-schema-notes.md
└── profiles/
    └── dak/
        ├── DAK_Milky_Cake_2_Lattes_pro.json
        ├── DAK_Cream_Donut_pro.json
        ├── DAK_Lush_Buds_pro.json
        └── DAK_Cherry_Focus_pro.json
```

## Included profiles

| Bean | File | Style |
|---|---|---|
| Milky Cake | profiles/dak/DAK_Milky_Cake_2_Lattes_pro.json | Sweet milk-drink profile |
| Cream Donut | profiles/dak/DAK_Cream_Donut_pro.json | Dessert-style milk profile |
| Lush Buds | profiles/dak/DAK_Lush_Buds_pro.json | Fruity / floral profile |
| Cherry Focus | profiles/dak/DAK_Cherry_Focus_pro.json | Cherry-forward milk profile |

## Bean and profile notes

| Bean | Bean style/type | What the profile is doing | Rating |
|---|---|---|---|
| Milky Cake | Sweet, milk-forward espresso style | Biases toward body and sweetness with a smoother pressure progression to keep chocolate/caramel notes round in milk drinks. | 4.7 / 5 |
| Cream Donut | Dessert-style, milk beverage focus | Uses a comfort-profile shape aimed at dense texture and lower astringency for richer, pastry-like cups. | 4.6 / 5 |
| Lush Buds | Fruity / floral espresso style | Keeps clarity higher with a profile behavior that supports brighter acidity and aromatic separation. | 4.5 / 5 |
| Cherry Focus | Cherry-forward milk profile | Pushes fruit definition while maintaining enough body for milk integration, emphasizing cherry sweetness. | 4.6 / 5 |

> Ratings are community-facing, dial-in-dependent reference scores (not official cupping scores).

## How to use

1. Download or clone this repository.
2. Choose a profile from `profiles/dak/`.
3. Import the JSON file into your GaggiMate-compatible workflow.
4. Pull a baseline shot and evaluate taste and extraction.
5. Keep notes for repeatability.

### Use at your own dial-in

Start with the profile as provided, then adjust grind, dose, and yield first before changing the profile itself.

## Naming convention

Profile filenames follow this convention:

`<ROASTER>_<BEAN_NAME>_pro.json`

Examples in this repo use the `DAK_` prefix and preserve bean naming for readability.

## Contributing

Pull requests are welcome for:

- new bean profiles
- revised tasting notes
- grinder-specific dial-in notes
- documentation improvements

Please keep JSON profile files clean, clearly named, and focused on one bean/style per file.

## Planned additions

- more DAK beans
- comparison notes
- grinder-specific dial-in notes
- shot result logs

## Disclaimer

These profiles are experimental, community-use espresso references and are not official DAK or GaggiMate presets.

Results vary by grinder, burr set, machine calibration, basket, puck prep, roast age, and water chemistry.
