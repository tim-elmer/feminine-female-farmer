# Feminine Female Farmer

Based on [Alex_01's Feminine Female Farmer](https://www.nexusmods.com/stardewvalley/mods/407)

Minimal testing performed. Feel free to submit issues/PRs.

## Requirements

You'll need [SMAPI](https://www.nexusmods.com/stardewvalley/mods/2400) and [Content Patcher](https://www.nexusmods.com/stardewvalley/mods/1915).

## Config

Setting | Options
--- | ---
Face | Default, Berets
Legs | Default, Sticky
Shirts | Default, Busty

Like most SMAPI mods, there is no included config file, you'll need to run the game with the mod installed once to generate it. Once that's done, you'll have a `config.json` file in your mods folder (probably something like `C:\Program Files (x86)\Steam\steamapps\common\Stardew Valley\Mods\FeminineFemaleFarmer\config.json`). 

In _that_ file, you'll see a series of "keys" and corresponding "values" (e.g., `"Key": "Value"`). Change the desired setting _value_ to one of the options listed above and restart the game.

## Known Issues

_A.K.A, won't be fixed in the forseeable future, at least not by me_

- Not all shirts are replaced, non-replaced shirts will look strange
- Pants aren't replaced at all
  - This includes swimwear

## Source Files

### farmer_girl_base.psd

#### Components

- FFFBeretsFace: The Beret's Face sheet as an overlay
- FFFSticky: The Sticky Leg sheet as an overlay
- FFFNormalOverlay: Overlays to meld the FFF sheet to vanilla
- FFFNormal: The FFF sheet
- Vanilla: The vanilla sheet

#### Masks

Layers that aren't melding overlays have masks set to remove either parts that aren't covered by the replacing sheet (in the case of vanilla), or that aren't relevant (in the case of sticky and beret's face)

#### Other

The `StardewFFFBody.aco` file is a color pallet for commonly used colors in the body sprite sheet.

### shirts.psd

It's literally just four layers, with the normal and busty replacements separated out. Male shirts have been masked off. The overlay layer is used to lengthen side shirts by a pixel.
