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

**Custom Patches:**
* [JOR - BS Bruma / Hearthfire Extended Patch](/custom-patches/JOR_BSBruma_HearthfireExtended_Patch.esp)
* [JOR - BS Bruma / Identity Crisis Patch](/custom-patches/JOR_BSBruma_IdentityCrisis_Patch.esp)
* [JOR - BS Bruma / LS2 Merges Patch (2.4.0)](/custom-patches/2.4.0/JOR_BSBruma_LS2Merges_Patch.esp)
* [JOR - BS Bruma / Occlusion Patch (2.4.0)](/custom-patches/2.4.0/JOR_BSBruma_Occlusion_LS2.4.0_Patch.esp)

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.4.0)
  * Install the Beyond Skyrim - Bruma SE and DLC Integration Patch mods in that order after Beyond Reach (and Midwood Isle if using), but before Darkend
  * BSAssets.esm, BSHeartland.esm, and BS_DLC_patch.esp should be placed before LegacyoftheDragonborn.esm in load order
  * Qw_BeyondSkyrimBruma_USSEP Hotfix Patch.esp and Qw_ACE_BSHeartland Patch.esp should be placed in that order before AI Overhaul.esp and also before the Qwinn's Beyond Reach patches if using (NOTE: I reinstalled the QUASIPC - Qwinn's Unified Automated Self Installing Patch Compendium mod with a different name and disabled the unrelated patches)
  * JOR_BSBruma_HearthfireExtended_Patch.esp, JOR_BSBruma_IdentityCrisis_Patch.esp, JOR_BSBruma_LS2Merges_Patch.esp, and JOR_BSBruma_Occlusion_LS2.4.0_Patch.esp should be loaded after zPatch.esp
  * Convenient Horses patch (in my case CH BRU_BRE_MWI.esp since it covers three mods) should be placed after zPatch.esp (NOTE: I reinstalled the Bruma and Other Patches for Convenient Horses mod with a different name to get this patch)

**Extra Notes:**

I know that there is an unofficial synergy patch between BS Bruma and LOTD, but unfortunately for the moment it isn't compatible now that the 3DNPC patch is officially supported. If this gets updated, I'll take another look to see if it can work.