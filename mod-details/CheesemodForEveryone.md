## Cheesemod for EVERYONE

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/36506

**Summary:** Adds a huge amount of hand-placed cheeses and a quest with Sheogorath

**LS2 Compatibility Status:** Seems good with patching, though hard to say with all the Placed Object records. Stability is likely fine, but placement of cheeses is in question.

**Recommendations:** 
_None_

**Official Patches:**
* [Legacy of the Dragonborn](https://www.nexusmods.com/skyrimspecialedition/mods/30980)
* [The Curator's Companion](https://www.nexusmods.com/skyrimspecialedition/mods/38529)
* https://www.nexusmods.com/skyrimspecialedition/mods/33364 (Select Cheesemod from the FOMOD or just grab the patch directly)
* https://www.nexusmods.com/skyrimspecialedition/mods/35910 (Select Cheesemod from the FOMOD or just grab the patch directly)
* https://www.nexusmods.com/skyrimspecialedition/mods/36380 (Can reinstall as separate mod from existing LS installation, or grab patch directly)

**Custom Patches:**
* [JOR - Cheesemod / LOTD Patch](/custom-patches/JOR_Cheesemod_LOTD_Patch.esp)
* [JOR - Cheesemod / Window Shadows Patch](/custom-patches/JOR_Cheesemod_WindowShadows_Patch.esp)
* [JOR - Cheesemod / LS2 Containers and LLs Patch](/custom-patches/JOR_Cheesemod_LS2ContainersLL_Patch.esp)
* [JOR - Cheesemod / Triumvirate Patch](/custom-patches/JOR_Cheesemod_Triumvirate_Patch.esp) (only if using Triumvirate)

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.5.2)
  * Load `yumcheese.esp` before `OCW_Obscure's_CollegeofWinterhold.esp`
  * Load `PCE - Cheesemod Patch.esp`, `Great Town of Ivarstead - Cheesemod Patch.esp`, `JOR_Cheesemod_LOTD_Patch.esp`, `JOR_Cheesemod_WindowShadows_Patch.esp`, and `JOR_Cheesemod_LS2ContainersLL_Patch.esp` in any order after `zPatch.esp`
  * For the two patches related to the JK's interior mods currently merged, you have to be a bit more involved:
    * Unhide plugins for LOTD Patches Merged, and edit the merge in zMerge. Under Plugins, select `JKs Arcadias Cauldron - Cheesemod Patch.esp` and `JKs Dragonsreach - Cheesemod Patch.esp`.
    * Move those two patches to the bottom on the Load Order tab, then build the merge. Exit zMerge, disable the plugins for the merge
  * `DBM_CheeseMod_Patch.esp` and `LOTD_TCC_CheeseMod.esp` in that order, currently before `ELE_SSE.esp` (NOTE: I reinstalled the Legacy of the Dragonborn Official Patches and Legacy of the Dragonborn SSE - The Curators Companion AFTER UPDATING THEM with different names and no other patches enabled to get these)
  * If using, load `JOR_Cheesemod_Triumvirate_Patch.esp` after `zPatch.esp`
