# ls2-extra-mods-unofficial
Information about adding and testing mods for compatibility with Living Skyrim modlist

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
  
## Miscellaneous Patches and Tweaks

**Re-Add Nirnroot sounds from Immersive Sounds - Compendium**

* Re-install Immersive Sounds - Compendium with a new name, but select whichever Nirnroot sound you prefer. Once installed, go into its Filetree and delete everything except for `sound/fx/itm_is/ingredient/itm_nirnroot_lp.wav`. Then just make sure it's after the original ISC mod in the install order.
