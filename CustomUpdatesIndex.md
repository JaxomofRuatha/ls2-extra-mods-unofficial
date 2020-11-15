# Custom updates, Merges and Reorganization

This is a list of the updates and changes I make to the base LS installation before starting to add extra mods. Technically most of it can be done at any time, but this just helps to give a better setup to start with and work from.

## Mods that I have disabled/removed for more plugin slots

* "iEquip"
* "Toccata Follower SE (With Elisif Replacer Option)" (NOTE: I ended up merging this plugin into "Pre-Final Steps Merge" and am using it with no issues thus far in my current playthrough)
* "Hunter Archer Armor (by protese for SSE)
* "SkyRem - Mia"
* "Not So Fast - Main Quest"
  * Also need to remove a patch from "LOTD Patches Merged" and rebuild
    * Go to Tools -> Tool Plugins -> Merge Plugins Hide, right click "LOTD Patches Merged", Enable Plugins
    * In "Legacy of the Dragonborn Patches (Official)", go to Optional ESPs tab and move `BCS_NotSoFast_Patch.esp` to optional
    * Open zEdit from the MO2 executable link, choose zMerge, and find the "LOTD Patches Merged" merge. Click on "Remove Unavailable Plugins" (it should just be the Not So Fast one missing), and then build and exit zMerge.
    * Go back into Merge Plugins Hide and disable plugins for "LOTD Patches Merged"
* "Easter Eggs Merged"
  * Go to SSEEdit and select `Settlements Merged.esp`. Right click, Apply Script, Report masters, and select Easter Eggs Merged. Remove all records referencing, and then Clean Masters.
  * Do the same for `enemies_releveled.esp` (I only had one record to remove here). Exit SSEEdit and save changes to both plugins.
  * Go to Tools -> Tool Plugins -> Merge Plugins Hide, right click "LS2 Patches Merged", Enable Plugins. Under the "LS2 Patches" mod, hide the `LS2 Easter Eggs Patch.esp` file (I put it to optional). Then go into zMerge, "remove unavailable plugins" for LS2 Patches Merged (should just be the one), and rebuild the patch. Exit zMerge and Disable Plugins for the merge. Go into SSEEdit, and Clean Masters for `LS2 Patches Merged.esp`.
  * Then disable "Easter Eggs Merged".

## Mods that I have compacted FormIDs to allow for ESL flagging

These mods should be okay to ESL flag once one update is made. Load your full list of mods in SSEEdit, right click on the patch, and select "Compact FormIDs for ESL" from the menu. After this operation completes, you should be able to add an ESL flag to the plugin as usual.

From my understanding, it SHOULD be safe to do this where the plugins meet the following criteria:
* They are NOT the master for any other plugins (no other plugins are referring to them)
* If there are scripts in the mod that use the `GetFormFromFile` function (I'd avoid any with scripts to be safe)
* If there are NPC facegen or voice files in or referenced by the mod, or `INFO` and `NPC_` record types in the plugin 

See https://tes5edit.github.io/docs/8-managing-mod-files.html#ImportantdangerswhencompactingFormIDs and https://www.afkmods.com/index.php?/topic/5079-plugin-files-and-you-esmeslesp/ for more details.

Here are the very few plugins I personally decided to compact and ESL flag:
* `EmbershardMineRevisited.esp`
* `SteepfallBurrowRevisited.esp`
* `WhiteRiverWatchRevisited.esp`
* `HaltedStreamCampRevisited.esp`
* `Northern Marsh Bridges SE.esp`

## New and Modified Merges

### Fixes to Miscellaneous Merged

Currently there are 3 patches that are part of both Miscellaneous Merged and also separate in load order. **NOTE: DO NOT ACTUALLY EDIT THIS MERGE. ONLY REBUILD.**

* `CFTO-JK-Patch.esp`
  * Delete `CFTO-JK-Patch.esp.mohidden` from "JK's Skyrim - Patches"
  * Download "JK's Skyrim - Carriage and Ferry Travel (CFTO) Patch" from https://www.nexusmods.com/skyrimspecialedition/mods/6289 (if it tells you it exists already, just use the one in Downloads)
  * Reinstall the patch with Merge option to "JK's Skyrim - Patches"
* `018InigoBanterPatch.esp`
  * Delete `018InigoBanterPatch.esp.mohidden` from "Song of the Green (Auri Follower)"
  * Download "Inigo Banter patch - sfts and Talwin fix" from https://www.nexusmods.com/skyrimspecialedition/mods/11278 (if it tells you it exists already, just use the one in Downloads)
  * Reinstall the patch with Merge option to "Song of the Green (Auri Follower)"
* `BFBR_ELE_Patch.esp`
  * Move `BFBR_ELE_Patch.esp` BELOW `BleakFallsBarrowRevisited.esp` in load order

Once that's done, do the following:

* Go to Tools -> Tool Plugins -> Merge Plugins Hide, Enable Plugins for Miscellaneous Patches Merged
* Go to zMerge and rebuild. Again, DO NOT go into the editing for the merge, just rebuild.
* Exit zMerge and Disable Plugins for Miscellaneous Patches Merged. `BFBR_ELE_Patch.esp` should remain enabled, which isn't ideal, but **touching Miscellaneous Patches Merged in any way other than the above broke my game consistently.**

### Gameplay Merged

This is definitely optional, just frees up one additional plugin slot (and moves the fix to a place where it seems like it does more actual fixing)

* Go to Tools -> Tool Plugins -> Merge Plugins Hide, Enable Plugins for Gameplay Merged
* Go into zMerge, and Edit the Gameplay Merged Plugins to include `Moonpath Music - Sky and Lighting fix - merged.esp`. Under the "Load Order" tab, if needed, move the plugin to the top of the other selected plugins so there's only a block of black plugins on top and green on the bottom. Then build the patch.
* Exit zMerge and Disable Plugins for Gameplay Merged.

### HUD Merged

There's already an unused merge available for this. Go to zMerge and either just build it (MAKING SURE to go to the "Data" tab of the merge and selecting "Copy General Assets") or, if you're using "Gamepad Plus Plus" and/or "Less Intrusive HUD II SE", I add those to this merge as well (`Gamepad++.esp` and `LessIntrusiveHUD.esp`, best to load them in after the others in the merge).

`HUD Merged.esp` should be loaded just before `Men Of Winter.esp`. Once this is enabled, use Merge Plugins Hide to disable the plugins for "HUD Merged".

### Fixes Merged

There is also an unused merge for this, but several things need to get changed.

* In zMerge, remove all of the mods except for `BugfixCompilation.esp`, `Fixed body collision.esp`, `HornsAreForever.esp`, and `ProjectAHO - StartWhenYouWant.esp`. Under "Load Order" tab, move `Dwarfsphere.esp` above `BugfixCompilation.esp`, and build the merge.
* Install "Fixes Merged" above "Flora Respawn Fix", and load `Fixes Merged.esp` after `Project AHO Unofficial Patch.esp`. Use Merge Plugins Hide to disable "Fixes Merged" plugins
* Move 

## Mods that can be updated

### Plug and Play

These mods seem fine to just be directly updated (choose "Replace" option for the given mod)

* "Legacy of the Dragonborn SSE - The Curators Companion" (https://www.nexusmods.com/skyrimspecialedition/mods/38529)
  * You can either reinstall this for only the initial LS mods and then make a separate mod for the extras, or just reinstall one mod with both.
* "Legacy of the Dragonborn Patches (Official)" (https://www.nexusmods.com/skyrimspecialedition/mods/30980)
  * Same as Curator's Companion
* "powerofthree's Papyrus Extender for SSE" (https://www.nexusmods.com/skyrimspecialedition/mods/22854)
* "JContainers SE" (https://www.nexusmods.com/skyrimspecialedition/mods/16495)
* "moreHUD Inventory Edition" (https://www.nexusmods.com/skyrimspecialedition/mods/18619)
* "Ordinator - Perks of Skyrim" (https://www.nexusmods.com/skyrimspecialedition/mods/1137)
* "Growl - Werebeasts of Skyrim" (https://www.nexusmods.com/skyrimspecialedition/mods/31245)
* "Improved NPC Encounter Zones (SkyRem - Inez)" (https://www.nexusmods.com/skyrimspecialedition/mods/27103)
* "Grace - SkyRem Series AIO" (https://www.nexusmods.com/skyrimspecialedition/mods/26207)
* "Legacy of the Dragonborn SSE" (https://www.nexusmods.com/skyrimspecialedition/mods/11802)
* "Frozen Electrocuted Combustion" (https://www.nexusmods.com/skyrimspecialedition/mods/3532)
* "Steepfall Burrow - Revisited" (https://www.nexusmods.com/skyrimspecialedition/mods/34594)
* "Embershard Mine - Revisited" (https://www.nexusmods.com/skyrimspecialedition/mods/34468)
* "NPC AI Process Position Fix - SSE" (https://www.nexusmods.com/skyrimspecialedition/mods/40261)
* "Window Shadows" (https://www.nexusmods.com/skyrimspecialedition/mods/37831)

### Nether's Follower Framework

Again I'm not positive on how stable this is, but I'm updating to the most recent version for my playthrough since there are quite a few changes.

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/18076

**Load/Install Notes:**
* For the FOMOD, here are the selections I made:
  * Core Options
    * Followers Avoid Traps
    * Replace Base Dialogue Scripts
    * Follower Class BAT Files
  * Core Mod Support
    * Interesting NPCs
    * Relationship Dialogue Overhaul (RDO)
    * RDO Comments
  * No Team Magic Damage SSE
    * ESP for Skyrim Special Edition
    * Apocalypse for SSE
* Go to Merge Plugins Hide and enable Plugins for "Pre-Final Steps Merge". Go into zMerge, and the corresponding merge should have `nwsFF_NoTeamMagicDamage.esp` and `nwsFF_NTMD_Apocalypse.esp` showing as changed (at least it did for me, I made a second mod for the updated NFF, but that's probably paranoid). Just rebuild this mod (I also added `Toccata.esp` here, but that's not necessary), then exit zMerge and re-hide the plugins.
*  I installed the mod right where it was previously (right under "Vilja in Skyrim"), and same for load order (right before `OCW_CellSettings.esp`)

### Organic Factions and Extension

This was tested with no stability issues on 2.4.0 by @ErikIEC, and that was without replacing the mod in the merge plugin. I have not played through with this change, but it seems to be stable from what I have seen

**Links:**
* https://www.nexusmods.com/skyrimspecialedition/mods/10289 (SSE OrganicFactions)
* https://www.nexusmods.com/skyrimspecialedition/mods/25471 (SSE OrganicFactionsExtension)
* [Patch by @ErikIEC with changes by @JaxomofRuatha](custom-patches/OrganicFactionsExtendedPatch.esp)

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.5.0, 2.5.2)
  * Install and Replace "SSE Organic Factions" and "SSE Organic Factions Extension"
  * Rebuild "NPC Additions Merged"
    * Go to Tools -> Tool Plugins -> Merge Plugins Hide, right click "NPC Additions Merged", Enable Plugins
    * Open zEdit from the MO2 executable link, choose zMerge, and find the "NPC Additions Merged" merge. It should have "Organic Factions Extended" in yellow (and possibly the Serana Dialogue Additions) but otherwise be unchanged. Click "Build", and exit zMerge when done.
  * `OrganicFactions.esm` should be after `EnhancedAIFramework.esm` (this should happen automatically upon replacing the mod), and `OrganicFactionsExtendedPatch.esp` should go after `LS2 Patches Merged.esp`
