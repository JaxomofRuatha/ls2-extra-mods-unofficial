# ls2-extra-mods-unofficial
Information about adding and testing mods for compatibility with Living Skyrim modlist

## Notes on how to use/contribute

**Recommendation ratings**

For the moment, I'm using the following rating system for any recommmendations:

1. Must-Add
2. Highly Recommended
3. Okay
4. Not Needed
5. Avoid

**Installing patches/individual files from existing LS2 mods**

For several patches and files, there is already a downloaded version with LS2, but the patches aren't selected for non-included mods. To add them without reinstalling over the original mod, do the following:

1. Select "Reinstall Mod..." from the mod in question
2. Rename the mod (can be anything as long as it's different, I recommend adding a description of the patch/file to the end of the name)
3. Only install the relevant files/patches you're trying to overwrite/add (if possible)
4. If the FOMOD doesn't allow for selecting only specific files/patches, finish installing and go to "Information..." on the mod. From there, it is possible under the "Filetree" tab to delete any unused files in the mod, so that the originals remain intact from the first installation

## Depths of Skyrim - An Underwater Overhaul SSE

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/26913

**Summary:** Adds underwater content and plant life

**LS2 Compatibility Status:** Good (no stability issues known after patching)

**Recommendations:** 
* JaxomofRuatha (Must-Add)

**Official Patches:**
* [Legacy of the Dragonborn](https://www.nexusmods.com/skyrimspecialedition/mods/30980)

**Custom Patches:**
* [JOR - Depths of Skyrim / Kynes Grass Patch](custom-patches/JOR_DepthsOfSkyrim_KynesGrass_Patch.esp)

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.2.1)
  * DepthsOfSkyrim.esp is immediately before Kyne's Grass.esp
  * DBM_DepthsofSkyrim_Patch.esp is before ELE_SSE.esp (NOTE: I reinstalled the Legacy of the Dragonborn Official Patches with a different name and no other patches enabled to get this)
  * JOR_DepthsOfSkyrim_KynesGrass_Patch.esp is before ai overhaul patch.esp

## MAPS

**Link:** https://www.nexusmods.com/skyrim/mods/66819

**Summary:** Adds much better textures for maps of Skyrim used in game

**LS2 Compatibility Status:** Excellent (no issues, no patching required)

**Recommendations:** 
* JaxomofRuatha (Must-Add)

**Official Patches:**
_None_

**Custom Patches:**
_None_

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.2.1)
  * MAPS goes after "unofficial performance optimized textures AKA (UPOT)" for install order

## Pastel SkyUI Markers/Colorful Map Markers

**Links:**
* https://www.nexusmods.com/skyrimspecialedition/mods/13604 (Pastel SkyUI Markers)
* https://www.nexusmods.com/skyrimspecialedition/mods/38079 (Colorful Map Markers)

**Summary:** Changes HUD and map markers to colored versions (either pastel or vivid)

**LS2 Compatibility Status:** Excellent (no issues, no patching required)

**Recommendations:** 
* JaxomofRuatha (Highly Recommend, prefer Pastel)

**Official Patches:**
_None_

**Custom Patches:**
_None_

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.2.1)
  * Either mod goes after SkyHUD for install order
 
## Save the Icerunner - Lights Out Alternate Routes

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/34681

**Summary:** Adds quest and dialogue options into the "Lights Out!" vanilla quest

**LS2 Compatibility Status:** Good (no stability issues known after patching)

**Recommendations:** 
* JaxomofRuatha (Highly Recommend)

**Official Patches:**
_None_

**Custom Patches:**
* [JOR - Save The Icerunner / LS2 Merges Patch](custom-patches/JOR_SaveTheIcerunner_LS2Merges_Patch.esp)

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.2.1)
  * JOR_SaveTheIcerunner_LS2Merges_Patch.esp is before ai overhaul patch.esp
  
## Enigma Series SSE / Talkative Dragons

**Links:**
* https://www.nexusmods.com/skyrimspecialedition/mods/34681 (Enigma Series All In One)
* https://www.nexusmods.com/skyrimspecialedition/mods/26955 (Talkative Dragons)

**Summary:** Changes many dragons' speaking voices to be more inhuman and intimidating, and uses vanilla voice lines to have normal dragons speak in combat

**LS2 Compatibility Status:** Good (no stability issues known after patching)

**Recommendations:** 
* JaxomofRuatha (Highly Recommend)

**Official Patches:**
* https://www.nexusmods.com/skyrimspecialedition/mods/33084 (Talkative Dragons, VIGILANT, Wyrmstooth)

**Custom Patches:**
_None_

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.2.1)
  * DragonCombatDialogue.esp seems like it can go anywhere after the vanilla and DLC, I have it after Occlusion.esp currently
  * Enigma Series AIO and Talkative Dragons installed first, then the patches, making sure all of it is after VIGILANT/Wyrmstooth
  
## The Tale of Tsatampra Xiros

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/36707

**Summary:** Daedric quest mod, with a player home once completed

**LS2 Compatibility Status:** Good (no known issues, no patching known but one minor Placed Item conflict)

**Recommendations:** 
_None_

**Official Patches:**
_None_

**Custom Patches:**
_None_

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.2.1)
  * The Tale of Tsatampra Xiros.esp is currently before ELE_SSE.esp

## Miscellaneous Patches and Tweaks

**Re-Add Nirnroot sounds from Immersive Sounds - Compendium**

* Re-install Immersive Sounds - Compendium with a new name, but select whichever Nirnroot sound you prefer. Once installed, go into its Filetree and delete everything except for `sound/fx/itm_is/ingredient/itm_nirnroot_lp.wav`. Then just make sure it's after the original ISC mod in the install order.
