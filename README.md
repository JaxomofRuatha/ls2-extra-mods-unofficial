# LS Unofficial Extras
Information about adding and testing mods for compatibility with Living Skyrim modlist

**IMPORTANT NOTE!!!**
This is a completely unofficial listing of mods that I and others from the Living Skyrim community have attempted to make work with the base Living Skyrim modlist. Adding ANY of these completely voids all support from ForgottenGlory and the Living Skyrim development team. Any custom patches are EXPERIMENTAL and load/install suggestions are ONLY SUGGESTIONS, using any of them is completely at your own risk.

I made this to collaborate on ideas, but it is entirely unofficial. You've been warned!

ALSO note that you will **need to ESL flag plugins** from the standard LS list to get any of these to work. The easy guide on how to do that is [here](https://tes5edit.github.io/docs/8-managing-mod-files.html#ESLifyingPluginstheeasyway).

IMPORTANT: You will NOT be able to add EVERY SINGLE MOD HERE. The non-ESL limit for plugins is still 254, so you might have to choose some to get rid of if you want to include others.

<br>

## Changelog

Adding this since I realize not everyone knows how to use Git and it's maybe not clear when things need to be redone.

[CHANGELOG](CHANGELOG.md)

## Notes on how to use/contribute

**Submitting new mods or personal experiences with listed mods**

If there's a mod you've been able to get working with the base LS modlist, or if you want to add your experience/patch/review to a mod that's already here, you'll need to submit an [Issue](https://github.com/JaxomofRuatha/ls2-extra-mods-unofficial/issues/new/choose). Technically you're free to submit whatever you've tried adding, but here's what to keep in mind if you can please:

1. Attempt to clean the mods (see below for how), and note if this is required (mods are dirty).
2. Check for conflicts with other mods in MO2 (install order), and also in SSEEdit (load order). If there are conflicts, either note them or provide patches for them with a comment about what you patched.
3. At least try and play LS with the mod installed and check that things are running stable, at least for a little bit. If there are quirks or noticeable interactions, mention that as well
4. Potentially play through the mod or try its features, though this isn't necessary (just make note that it is "Unreviewed", as I have done). If you have played through, adding a short review in addition to the basic recommendation would be great!

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

**Cleaning mods**

Unless a mod author SPECIFICALLY says otherwise (and even then in some cases, especially for older mods), you should attempt a quick clean of any mods you add. To do this, activate the plugins you want to clean, and go to the LS executable for "SSEEditQuickAutoClean" (it uses a specific EXE from SSEEdit if it's not set up already for whatever reason). Then select the plugin from the list, and it should run the quick clean.

If it doesn't say "dirty" at the bottom of the messages window, that means it didn't find anything that required cleaning. If it DOES say "dirty", it means that the cleaning is required for better stability (so note this if attempting to recommend the mod). Sometimes it will also say "reqManualFix", which normally means that there is some known issue, and often the mod page/posts will recommend how to proceed.

<br><br>

# Added Mods

## Must-Add

#### [3D Snowberries](mod-details/3DSnowberries.md)

###### (:+1: @JaxomofRuatha)

## Highly Recommend

#### [Pastel SkyUI Markers/Colorful Map Markers](mod-details/PastelMarkers.md)

###### (:+1: @JaxomofRuatha)

#### [Save the Icerunner - Lights Out Alternate Routes](mod-details/SaveTheIcerunner.md)

###### (:+1: @JaxomofRuatha)

#### [Enigma Series SSE / Talkative Dragons](mod-details/EnigmaSeriesTalkativeDragons.md)

###### (:+1: @JaxomofRuatha)

#### [Keld-Nar](mod-details/KeldNar.md)

###### (:+1: @JaxomofRuatha)

#### [Strange Runes](mod-details/StrangeRunes.md)

###### (:+1: @JaxomofRuatha)

#### [Bard Instrumentals Mostly / Alternative Bards Songs](mod-details/AlternativeBardSongs.md)

###### (:+1: @JaxomofRuatha)

#### [ENB Light](mod-details/ENBLight.md)

###### (:+1: @JaxomofRuatha)

#### [Dear Diary - Paper SkyUI Menus Replacer SE](mod-details/DearDiary.md)

###### (:+1: @JaxomofRuatha)

#### [Halted Stream Camp - Revisited](mod-details/HaltedStreamCampRevisited.md)

###### (:+1: @JaxomofRuatha)

#### [Rudy HQ - More Lights for ENB SE](mod-details/RudyHQMoreLightsForENB.md)

###### (:+1: @JaxomofRuatha)

#### [Fluffy Snow](mod-details/FluffySnow.md)

###### (:+1: @JaxomofRuatha)

#### [Music Mods Merged](mod-details/MusicModsMerged.md)

###### (:+1: @JaxomofRuatha)

#### [Barenziah's Glowing SE](mod-details/BarenziahsGlowing.md)

###### (:+1: @JaxomofRuatha)

#### [A Cat's Life](mod-details/ACatsLife.md)

###### (:+1: @Day7-J)

#### [Identity Crisis](mod-details/IdentityCrisis.md)

###### (:+1: @WinterdrakeX)

#### [Swift Potion Reborn](mod-details/SwiftPotionReborn.md)

###### (:+1: @WinterdrakeX)

#### [Aetherium Armor and Weapons Compilation by Lautasantenni](mod-details/AetheriumArmorAndWeapons.md)

###### (:+1: @WinterdrakeX)

#### [Jiub's Opus](mod-details/JiubsOpus.md)

###### (:+1: @WinterdrakeX)

#### [[SunJeong] Ninirim Collection 6.0](mod-details/NinirimCollection.md)

###### (:+1: @WinterdrakeX)

#### [Jesus In Skyrim](mod-details/JesusInSkyrim.md)

###### (:+1: @WinterdrakeX)

#### [NPC Dialogue Audio Enhancer](mod-details/NPCDialogueEnhancer.md)

###### (:+1: @JaxomofRuatha)

## Okay

#### [Provincial Courier Service](mod-details/ProvincialCourierService.md)

###### (:+1: @JaxomofRuatha)

#### [Midwood Isle SE](mod-details/MidwoodIsle.md)

###### (:+1: @JaxomofRuatha)

#### [Animated Wings Ultimate](mod-details/AnimatedWingsUltimate.md)

###### (:+1: @WinterdrakeX)

#### [RUSTIC CHILDREN](mod-details/RusticChildren.md)

###### (:+1: @JaxomofRuatha)

## Unreviewed

#### [The Tale of Tsatampra Xiros](mod-details/TsatampraXiros.md)

#### [Voyage to the Dreamborne Isles SE](mod-details/DreamborneIsles.md)

#### [Away Come Away](mod-details/AwayComeAway.md)

#### [Maelstrom - Fully Voiced Follower and Quest Mod SSE](mod-details/Maelstrom.md)

#### [Mealtime - A Food and Recipe Mod](mod-details/Mealtime.md)

#### [Fossil Mining - With Legacy Support](mod-details/FossilMining.md)

#### [Amulets of Skyrim](mod-details/AmuletsOfSkyrim.md)

#### [Artifacts of Skyrim](mod-details/ArtifactsOfSkyrim.md)

#### [Legacy of the Dragonborn BadGremlins Collection](mod-details/BadGremlinsCollection.md)

#### [Artifacts - The Ice Blade of the Monarch](mod-details/IceBladeOfTheMonarch.md)

#### [JaySuS Swords SE](mod-details/JaysusSwords.md)

#### [Kthonia's Unique Weapon Pack - Dragonborn Weapons](mod-details/KthoniasUniqueWeapons.md)

#### [New Treasure Hunt SSE](mod-details/NewTreasureHunt.md)

#### [Oblivion Artifact Pack SE](mod-details/OblivionArtifacts.md)

#### [Ruin's Edge](mod-details/RuinsEdge.md)

#### [The Tools of Kagrenac](mod-details/ToolsOfKagrenac.md)

#### [Volkihar Knight - Legacy of the Dragonborn Patch](mod-details/VolkiharKnightLOTD.md)

#### [The Wheels of Lull](mod-details/WheelsOfLull.md)

#### [Beyond Reach](mod-details/BeyondReach.md)

#### [Beyond Skyrim - Bruma SE](mod-details/BSBruma.md)

#### [Beyond Skyrim - Wares of Tamriel SE](mod-details/BSWaresOfTamriel.md)

#### [Final Cataclysm - 2020](mod-details/FinalCataclysm2020.md)

#### [M'Rissi's Tails of Troubles SE](mod-details/MrissisTailsOfTroubles.md)

#### [Sepolcri - A Complete Burial Sites Overhaul](mod-details/Sepolcri.md)

#### [Triumvirate - Mage Archetypes](mod-details/Triumvirate.md)

#### [Carriage and Ferry Travel Overhaul - Fixes and Winterhold](/mod-details/CTFOFixesWinterhold.md)

#### [Legacy Safehouse Plus](mod-details/LegacySafehousePlus.md)

#### [Legacy of the Dragonborn - Followers Patch](mod-details/LOTDFollowers.md)

## Added to LS

#### [MAPS (added LS 2.3.0)](mod-details/MAPS.md)

###### (:+1: @JaxomofRuatha)

#### [Dawnguard Map Markers (added LS 2.3.0)](mod-details/DawnguardMapMarkers.md)

###### (:+1: @JaxomofRuatha)

#### [JS Purses and Septims SE (added LS 2.3.0)](mod-details/JSPursesAndSeptims.md)

###### (:+1: @JaxomofRuatha)

#### [Depths of Skyrim - An Underwater Overhaul SSE (added LS 2.4.0)](mod-details/DepthsOfSkyrim.md)

###### (:+1: @JaxomofRuatha)

#### [Northern Marsh Bridges SE (added LS 2.4.0)](mod-details/NorthernMarshBridges.md)

###### (:+1: @JaxomofRuatha)

#### [Helgen Reborn - NordWarUA Armor Replacer (added LS 2.4.0)](mod-details/HelgenRebornArmorReplacer.md)

###### (:+1: @WinterdrakeX)

## Deprecated or Needs Update/Patch

#### [Chapter II - Jeremy Soule Inspired Music (by Dreyma Music)](mod-details/ChapterII.md)

#### [The Northerner Diaries in Skyrim](mod-details/NorthernerDiaries.md)

<br><br>

# Miscellaneous Patches and Tweaks

## Re-Add Nirnroot sounds from Immersive Sounds - Compendium

* Re-install Immersive Sounds - Compendium with a new name, but select whichever Nirnroot sound you prefer. Once installed, go into its Filetree and delete everything except for `sound/fx/itm_is/ingredient/itm_nirnroot_lp.wav`. Then just make sure it's after the original ISC mod in the install order.

<br><br>

# Experimental/Temporary Bug Fixes and Consistency Patches

## Fix for Archery Gameplay Overhaul and Pretty Combat Animations issue

**Link:** [Patch by TwistedModding](custom-patches/ago_pca_patch.rar)

**Load/Install Order Notes:**
* TwistedModding
  * Place this patch after the mod: Compatibility Patch for Archery Gameplay Overhaul (AGO) and XP32 Skeleton Styles MCM

## Fix for 2.4.0 Revisited mods conflict

**Load/Install Order Notes:**
* ForgottenGlory
  * Move `BleakFallsBarrowRevisited.esp` and `UstengravRevisited` to immediately after `Miscellaneous Patches Merged.esp` and before `BFBR_ELE_Patch.esp`

## Use "No Camp" option for Hedge Mage Armor to prevent crashes/conflicts

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/5269 (Hedge Mage Armor - No Camp)

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.4.0)
  * Hedge Mage Armor - No Camp.esp should be opened in Creation Kit and re-saved as a Form 44 plugin (just open it as the active mod, then save)
  * Hedge Mage Armor.esp should be disabled, and replaced with Hedge Mage Armor - No Camp.esp (currently placed immediately before moonpath.esp in load order)

## Update NPC AI Process Position Fix - SSE

This mod was updated after the LS 2.4.0 release, just install the main file and replace

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/40261

## Fix for human Serana eyes (included in LS 2.4.0)

Currently Serana's eyes once cured are linking to missing textures, this just links it to the one existing in the filepath.

**Link:** [Patch by JaxomofRuatha](custom-patches/JOR_SeranaEyesFix.esp)

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.2.1)
  * Patch ESP should go after LS2 Patches Merged
  
## Fix for 2.2.1 Black Face Bugs

**Link:** [Patch by JaxomofRuatha](custom-patches/2.2.1/LS2%20BFB%20Fixes%20Patch.esp)

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.2.1)
  * Patch ESP should go after LS2 Patches Merged
  
**Extra Notes**

Included NPCs in this patch are Golldir, Erandur, Vorstag, Madanach, Benor, Marcurio, Belrand, and Stenvar. The Men of Winter records were forwarded as is, so if there's changes in new LS releases, that might not be quite the same if there's customized patching.

## Clockwork patches for LOTD display temporary fix (LS 2.2.1)

Currently the Clockwork LOTD display is broken, because the patches for it are above the actual Clockwork ESP. According to several testers, it works to move DBM_Clockwork_Patch.esp and LOTD_TCC_Clockwork.esp below Clockwork.esp.

**Extra Notes**

This doesn't work correctly (from my experience) if done mid-save, the display doesn't get added and the LOTD Checklist gets glitched out. You may be able to rebuild the MCM and have it work.

<br><br>

# Mods Under Review

These are mods that are known through reputation, interest, or prior attempts to integrate, and either haven't been correctly integrated/patched for LS2 yet or haven't had an attempt to add them

<br>

#### [Cheesemod for EVERYONE](mod-details/CheesemodForEveryone.md)
