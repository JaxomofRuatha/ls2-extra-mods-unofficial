## Beyond Skyrim - Bruma SE

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/10917

**Summary:** Travel beyond the borders of Skyrim and explore Bruma, the northernmost county in Cyrodiil. Delve into Ayleid ruins, meddle in local affairs or explore the wilds - the journey begins now. 

**LS2 Compatibility Status:** Good (no stability issues known after patching)

**Recommendations:** 
_None_

**Official Patches:**
* https://www.nexusmods.com/skyrimspecialedition/mods/10917 (DLC Integration Patch)
* https://www.nexusmods.com/skyrimspecialedition/mods/18369 (QUASIPC - Unified Patch Compendium v2_5_0, already in LS Downloads)
* https://www.nexusmods.com/skyrimspecialedition/mods/13812 (Bruma and Other Patches for Convenient Horses, already in LS Downloads)
* 

**Custom Patches:**
* [JOR - BS Bruma / Hearthfire Extended Patch](/custom-patches/JOR_BSBruma_HearthfireExtended_Patch.esp)
* [JOR - BS Bruma / Identity Crisis Patch](/custom-patches/JOR_BSBruma_IdentityCrisis_Patch.esp)
* [JOR - BS Bruma / LS2 Merges Patch (2.4.0)](/custom-patches/2.4.0/JOR_BSBruma_LS2Merges_Patch.esp)
* [JOR - BS Bruma / Occlusion Patch (2.4.0)](/custom-patches/2.4.0/JOR_BSBruma_Occlusion_LS2.4.0_Patch.esp)
* [JOR - Qwinn / BS Bruma Patch](/custom-patches/JOR_Qwinn_DBMBruma_Patch.esp)
* [JOR - Beyond Reach / BS Bruma Patch](/custom-patches/JOR_BSBruma_BeyondReach_Patch.esp)
* [JOR - Beyond Reach and BS Bruma / LS2 Music Patch](/custom-patches/JOR_BrumaAndReach_LS2Merges_Patch.esp)
* [JOR - Beyond Reach and BS Bruma / Music Mods Merged Patch](/custom-patches/JOR_BrumaAndReach_MusicMerged_Patch.esp)

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.4.0)
  * Install the Beyond Skyrim - Bruma SE and DLC Integration Patch mods in that order after Beyond Reach (and Midwood Isle if using), but before Darkend
  * BSAssets.esm, BSHeartland.esm, and BS_DLC_patch.esp should be placed before LegacyoftheDragonborn.esm in load order
  * Qw_BeyondSkyrimBruma_USSEP Hotfix Patch.esp and Qw_ACE_BSHeartland Patch.esp should be placed in that order before AI Overhaul.esp and also before the Qwinn's Beyond Reach patches if using (NOTE: I reinstalled the QUASIPC - Qwinn's Unified Automated Self Installing Patch Compendium mod with a different name and disabled the unrelated patches)
  * JOR_Qwinn_DBMBruma_Patch.esp should load after Qw_BeyondSkyrimBruma_USSEP and Qw_ACE_BSHeartland Patch.esp
  * JOR_BSBruma_HearthfireExtended_Patch.esp, JOR_BSBruma_IdentityCrisis_Patch.esp, JOR_BSBruma_LS2Merges_Patch.esp, and JOR_BSBruma_Occlusion_LS2.4.0_Patch.esp should be loaded after zPatch.esp
  * Convenient Horses patch (in my case CH BRU_BRE_MWI.esp since it covers three mods) should be placed after zPatch.esp (NOTE: I reinstalled the Bruma and Other Patches for Convenient Horses mod with a different name to get this patch)
  * If Beyond Reach is installed:
    * As noted above, I have arnima.esm before all of the BS Bruma ESMs in load order
    * JOR_BSBruma_BeyondReach_Patch.esp should load after zPatch.esp
    * Either JOR_BrumaAndReach_LS2Merges_Patch.esp OR JOR_BrumaAndReach_MusicMerged_Patch.esp should be loaded. The "LS2Merges" version should load after Occlusion.esp (this is if you DO NOT have Music Mods Merged installed), the "MusicMerged" version should load after MMM_OCW-patch.esp (this is if you DO have Music Mods Merged installed)