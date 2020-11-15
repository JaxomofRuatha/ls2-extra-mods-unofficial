## Gamepad Plus Plus

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/27007

**Summary:** Gamepad++ brings extended functionality for gamepad players adding many controller shortcuts previously only available to keyboard users, as well as making double press, triple press and hold actions plus key combos available allowing up to 80 emulated keypresses to mimic keyboard hotkeys set for other mods.

**LS2 Compatibility Status:** Good (no issues, no patching required)

**Recommendations:** 
* JaxomofRuatha (Highly Recommend)

**Official Patches:**
_None_

**Custom Patches:**
_None_

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.5.2)
  * `Gamepad++.esp` should be able to load anywhere, though I ended up merging the plugin into `HUD Merged.esp` without issue (see [custom updates](/CustomUpdatesIndex.md))
 
**Extra Notes:**

This mod WILL force Skyrim to use gamepad, and it will remain that way even with the mod disabled unless you hide the file `interface/controls/pc/controlmap.txt` in this mod (and "HUD Merged" if you went that route) and delete `ControlMap_Custom.txt` from the base Skyrim directory (if it exists) before reloading the game.