# LS Unofficial Extras
Information about adding and testing mods for compatibility with Living Skyrim modlist

**IMPORTANT NOTE!!!**
This is a completely unofficial listing of mods that I and others from the Living Skyrim community have attempted to make work with the base Living Skyrim modlist. Adding ANY of these completely voids all support from ForgottenGlory and the Living Skyrim development team. Any custom patches are EXPERIMENTAL and load/install suggestions are ONLY SUGGESTIONS, using any of them is completely at your own risk.

I made this to collaborate on ideas, but it is entirely unofficial. You've been warned!

ALSO note that you will **need to ESL flag plugins** from the standard LS list to get any of these to work. I will be adding a guide on how to do that in the near future, but the general idea is [here](https://tes5edit.github.io/docs/8-managing-mod-files.html#ESLifyingPluginstheeasyway)

<br>

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

<br><br>

# Added Mods

## Must-Add

[Depths of Skyrim - An Underwater Overhaul SSE](mod-details/DepthsOfSkyrim.md)

[MAPS](mod-details/MAPS.md)

[Dawnguard Map Markers](mod-details/DawnguardMapMarkers.md)

## Highly Recommend

[JS Purses and Septims SE](mod-details/JSPursesAndSeptims.md)

[Pastel SkyUI Markers/Colorful Map Markers](mod-details/PastelMarkers.md)

[Save the Icerunner - Lights Out Alternate Routes](mod-details/SaveTheIcerunner.md)

[Enigma Series SSE / Talkative Dragons](mod-details/EnigmaSeriesTalkativeDragons.md)

[Keld-Nar](mod-details/KeldNar.md)

[Northern Marsh Bridges SE](mod-details/NorthernMarshBridges.md)

[Strange Runes](mod-details/StrangeRunes.md)

[Bard Instrumentals Mostly / Alternative Bards Songs](mod-details/AlternativeBardSongs.md)

[ENB Light](mod-details/ENBLight.md)

[Dear Diary - Paper SkyUI Menus Replacer SE](mod-details/DearDiary.md)

[Halted Stream Camp - Revisited](mod-details/HaltedStreamCampRevisited.md)

[Rudy HQ - More Lights for ENB SE](mod-details/RudyHQMoreLightsForENB.md)

[Fluffy Snow](mod-details/FluffySnow.md)

[Music Mods Merged](mod-details/MusicModsMerged.md)

[A Cat's Life](mod-details/ACatsLife.md)

[Identity Crisis](mod-details/IdentityCrisis.md)

[Swift Potion Reborn](mod-details/SwiftPotionReborn.md)

[Aetherium Armor and Weapons Compilation by Lautasantenni](mod-details/AetheriumArmorAndWeapons.md)

[Helgen Reborn - NordWarUA Armor Replacer](mod-details/HelgenRebornArmorReplacer.md)

[Jiub's Opus](mod-details/JiubsOpus.md)

[[SunJeong] Ninirim Collection 6.0](mod-details/NinirimCollection.md)

[Jesus In Skyrim](mod-details/JesusInSkyrim.md)

## Okay

[Provincial Courier Service](mod-details/ProvincialCourierService.md)

[Midwood Isle SE](mod-details/MidwoodIsle.md)

[Animated Wings Ultimate](mod-details/AnimatedWingsUltimate.md)

## Unreviewed

[The Tale of Tsatampra Xiros](mod-details/TsatampraXiros.md)

[Voyage to the Dreamborne Isles SE](mod-details/DreamborneIsles.md)

[Away Come Away](mod-details/AwayComeAway.md)

[Maelstrom - Fully Voiced Follower and Quest Mod SSE](mod-details/Maelstrom.md)

[Triumvirate - Mage Archetypes](mod-details/Triumvirate.md)

## Deprecated or Needs Update/Patch

[Chapter II - Jeremy Soule Inspired Music (by Dreyma Music)](mod-details/ChapterII.md)

[The Northerner Diaries in Skyrim](mod-details/NorthernerDiaries.md)

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
  
  
## Fix for 2.2.1 Black Face Bugs

**Link:** [Patch by JaxomofRuatha](custom-patches/LS2%20BFB%20Fixes%20Patch.esp)

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.2.1)
  * Patch ESP should go after LS2 Patches Merged
  
**Extra Notes**

Included NPCs in this patch are Golldir, Erandur, Vorstag, Madanach, Benor, Marcurio, Belrand, and Stenvar. The Men of Winter records were forwarded as is, so if there's changes in new LS releases, that might not be quite the same if there's customized patching.

## Clockwork patches for LOTD display temporary fix

Currently the Clockwork LOTD display is broken, because the patches for it are above the actual Clockwork ESP. According to several testers, it works to move DBM_Clockwork_Patch.esp and LOTD_TCC_Clockwork.esp below Clockwork.esp.

**Extra Notes**

This doesn't work correctly (from my experience) mid-save, the display doesn't get added and the LOTD Checklist gets glitched out.

<br><br>

# Mods Under Review

These are mods that are known through reputation, interest, or prior attempts to integrate, and either haven't been correctly integrated/patched for LS2 yet or haven't had an attempt to add them

<br>

[M'Rissi's Tails of Troubles SE](mod-details/MrissisTailsOfTroubles.md)

[Cheesemod for EVERYONE](mod-details/CheesemodForEveryone.md)
