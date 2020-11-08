## Beyond Reach

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/3008

**Summary:** Beyond Reach is a DLC sized mod that takes place in the east of High Rock, commonly known as The Reach. You will experience a story of intrigue, conspiracies sowed by both men and gods, and the struggles of those in the most squalid situations.

**LS2 Compatibility Status:** Good (no stability issues known after patching)

**Recommendations:** 
_None_

**Official Patches:**
* https://www.nexusmods.com/skyrimspecialedition/mods/23439 (Beyond Reach - Tweaks and Enhancements - FOMOD v2.4.3SE)
* https://www.nexusmods.com/skyrimspecialedition/mods/18369 (QUASIPC - Unified Patch Compendium v2_5_0, already in LS Downloads)
* https://www.nexusmods.com/skyrimspecialedition/mods/13812 (Bruma and Other Patches for Convenient Horses, already in LS Downloads)

**Custom Patches:**
* [JOR - Beyond Reach / USSEP Patch](/custom-patches/JOR_BeyondReach_USSEP_Patch.esp)
* [JOR - Beyond Reach / LS2 Merges Patch (2.4.0)](/custom-patches/2.4.0/JOR_BeyondReach_LS2Merges_Patch.esp)
* [JOR - Beyond Reach / Forgotten City Patch](/custom-patches/JOR_BeyondReach_ForgottenCity_Patch.esp)
* [JOR - Beyond Reach Tweaks / Update Patch](/custom-patches/JOR_BeyondReachTweaks_Update_Patch.esp)
* [JOR - Beyond Reach / LS2 Bash Patch (2.4.0)](/custom-patches/2.4.0/JOR_BeyondReach_LS2Bash_Patch.esp)
* [JOR - Beyond Reach / BS Bruma Patch](/custom-patches/JOR_BSBruma_BeyondReach_Patch.esp)
* [JOR - Beyond Reach and BS Bruma / LS2 Music Patch](/custom-patches/JOR_BrumaAndReach_LS2Merges_Patch.esp)
* [JOR - Beyond Reach and BS Bruma / Music Mods Merged Patch](/custom-patches/JOR_BrumaAndReach_MusicMerged_Patch.esp)

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.4.0, 2.5.2)
  * Install the "Beyond Reach" and "Beyond Reach - Tweaks and Enhancments" mods after "Midwood Isle SE" (if using) and before "Darkend" (for the tweaks FOMOD, I personally am using "Skyrim Border Tweaks", "Shields and Cloaks", and "Temper Recipes")
  * `arnima.esm` should be placed before `LegacyoftheDragonborn.esm` (I currently have it between `Midwood Isle.esp` and `BSAssets.esm`)
  * `Beyond Reach - Shields and Cloaks.esp`, `Beyond Reach - Skyrim Border Tweaks.esp`, and `Beyond Reach - Temper Recipes.esp` should be placed before `Landscape Fixes For Grass Mods.esp` (their order shouldn't matter)
  * `Qw_BeyondReach_USSEP Patch.esp`, `Qw_BeyondReach_RDO Patch.esp`, and `Qw_WACCF_arnima Patch.esp` should be placed in that order before `AI Overhaul.esp` (NOTE: I reinstalled the "QUASIPC - Qwinn's Unified Automated Self Installing Patch Compendium" mod with a different name and disabled the unrelated patches)
  * `JOR_BeyondReach_USSEP_Patch.esp`, `JOR_BeyondReach_LS2Merges_Patch.esp`, `JOR_BeyondReach_ForgottenCity_Patch.esp`, `JOR_BeyondReachTweaks_Update_Patch.esp`, and `JOR_BeyondReach_LS2Bash_Patch.esp` should be placed in that order after `zPatch.esp`
  * Convenient Horses patch (in my case `CH BRU_BRE_MWI.esp` since it covers three mods) should be placed after `zPatch.esp` (NOTE: I reinstalled the "Bruma and Other Patches for Convenient Horses" mod with a different name to get this patch)
  * If BS Bruma is installed:
    * As noted above, I have `arnima.esm` before all of the BS Bruma ESMs in load order
    * `JOR_BSBruma_BeyondReach_Patch.esp` should load after `zPatch.esp`
    * Either `JOR_BrumaAndReach_LS2Merges_Patch.esp` OR `JOR_BrumaAndReach_MusicMerged_Patch.esp` should be loaded. The "LS2Merges" version should load after `Occlusion.esp` (this is if you DO NOT have "Music Mods Merged" installed), the "MusicMerged" version should load after `MMM_OCW-patch.esp` (this is if you DO have "Music Mods Merged" installed)
