# HOI4 Character Generator

A browser-based character and country leader generator for Hearts Of Iron 4 modding.

This tool helps modders quickly generate valid HOI4 character definitions, leader entries, ideologies, portraits, localization, and recruit commands without manually writing the files.

Live tool:  
https://plsgivemevisualstudiomicrosoft.github.io/hoi4-character-generator/

---

## Features

- Generate country leaders for all four base ideologies
- Supports vanilla and custom sub-ideologies
- Outputs:
  - `characters = {}` blocks
  - `.gfx` portrait entries
  - Recruit character commands
  - Localization entries
  - Optional full `00_ideologies.txt`
- Automatic filename-safe character keys
- One-click placeholder `.dds` portrait generation with the correct file-names
- Fully client-side

---

## How to Use

1. Open the generator in your browser
2. Enter a country TAG (e.g. `EST`)
3. Fill in character names
4. Select ideologies or define custom ones
5. Click **Generate**
6. Copy the generated blocks into your HOI4 mod files

The generated output is compatible with all mods, if the ideologies are correct, and the recruit_character !! Is not on the last line of the .txt !!

---

## Output Files

Put the files where they belong after generating:
(list in order (I think))
- `common/characters/*.txt` #Where we define the actual charachters
- `interface/*.gfx` #So the game knows where character portraits are
- `history/countries/<TAG>.txt` #So the characters get assigned to a country
- `localisation/english/*.yml` #For the names
- `common/ideologies/00_ideologies.txt` #For any new ideologies
- `gfx/leaders/<TAG>/*.dds` #For the actual images of the portraits (That u download)

Placeholder `.dds` files are provided in the correct dimensions, and go in `gfx/leaders/<TAG>/*.dds` change them to a real portrait after.
Get Portrait Backrounds here ----> https://github.com/Globvs/Ultimate-HOI4-GFX
---

## Hosting

This project is hosted using GitHub and runs entirely in the browser.

Made by Claude and uses The Unlicense, do whatever u want
---

## Disclaimer

This is a fan-made modding utility.  
