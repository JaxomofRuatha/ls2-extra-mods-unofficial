# LS Unofficial Extras
Information about adding and testing mods for compatibility with Living Skyrim modlist

**IMPORTANT NOTE!!!**
This is a completely unofficial listing of mods that I and others from the Living Skyrim community have attempted to make work with the base Living Skyrim modlist. Adding ANY of these completely voids all support from ForgottenGlory and the Living Skyrim development team. Any custom patches are EXPERIMENTAL and load/install suggestions are ONLY SUGGESTIONS, using any of them is completely at your own risk.

I made this to collaborate on ideas, but it is entirely unofficial. You've been warned!

## ESLifying and Important Caveats

Note that you will **need to ESL flag plugins** from the standard LS list to get any of these to work. The easy guide on how to do that is [here](https://tes5edit.github.io/docs/8-managing-mod-files.html#ESLifyingPluginstheeasyway). **DO NOT ESL FLAG BlockSteal.esp**

You will NOT be able to add EVERY SINGLE MOD HERE. The non-ESL limit for plugins is still 254, so you might have to choose some to get rid of if you want to include others. Depending on what you remove, you'll also have to patch accordingly (I try to treat LS as "one mod" for patching, so usually fine, but make sure to check in SSEEdit)

If you have issues or notice unresolved conflicts/bugs, please report them in an issue! Things may go out of date somewhat quickly, and either way I don't claim perfection with custom patches. Thank you!

<br>

## Changelog

Adding this since I realize not everyone knows how to use Git and it's maybe not clear when things need to be redone.

[CHANGELOG](CHANGELOG.md)

## Example Install/Load Order Files

I'm adding these in here from time to time to give a top-level overview of what running install/load orders look like.

[Install/Load Order Examples](/example-orders/OrdersIndex.md)

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

The only people who have actually used mods in a playthrough of some kind are the ones with their recommendation in the mod page. Mods that have NO recommendations (listed under Unreviewed) didn't show any stability/compatibility problems with brief testing, but have not been used in a playthrough.

**Installing patches/individual files from existing LS2 mods**

For several patches and files, there is already a downloaded version with LS2, but the patches aren't selected for non-included mods. To add them without reinstalling over the original mod, do the following:

1. Select "Reinstall Mod..." from the mod in question
2. Rename the mod (can be anything as long as it's different, I recommend adding a description of the patch/file to the end of the name)
3. Only install the relevant files/patches you're trying to overwrite/add (if possible)
4. If the FOMOD doesn't allow for selecting only specific files/patches, finish installing and go to "Information..." on the mod. From there, it is possible under the "Filetree" tab to delete any unused files in the mod, so that the originals remain intact from the first installation

**Cleaning mods**

Unless a mod author SPECIFICALLY says otherwise (and even then in some cases, especially for older mods), you should attempt a quick clean of any mods you add. To do this, activate the plugins you want to clean, and go to the LS executable for "SSEEditQuickAutoClean" (it uses a specific EXE from SSEEdit if it's not set up already for whatever reason). Then select the plugin from the list, and it should run the quick clean.

If it doesn't say "dirty" at the bottom of the messages window, that means it didn't find anything that required cleaning. If it DOES say "dirty", it means that the cleaning is required for better stability (so note this if attempting to recommend the mod). Sometimes it will also say "reqManualFix", which normally means that there is some known issue, and often the mod page/posts will recommend how to proceed.

**Dummy plugins**

In some cases, there will need to be a dummy plugin that only contains basic information and the expected plugin name for a dependent mod to use as a master. There seems to be two ways of creating such a mod, unsure whether there is any functional difference between them as long as the name of the plugin is correct:

1. (I'm using this method currently) Make a copy of the actual plugin you are trying to make a dummy of (usually hidden due to being part of a merge), open it in SSEEdit, and remove all records from it besides the File Header before saving it.
2. Create a new masterless plugin in the Creation Kit with nothing selected for data or masters

**Other Random Notes**

* In most cases where you're not attempting to create a merge patch it likely is fine to leave BSAs as-is, but I make a habit of unpacking every single one that I can, mainly to see what conflicts there are from installs since it doesn't seem to make any kind of performance difference (other than possibly at load)
* I am starting to notate MODS (left pane of MO2) in quotations (e.g. "Unofficial Skyrim Special Edition Patch") and PLUGINS (right pane of MO2) in block quote format (e.g. `Unofficial Skyrim Special Edition Patch.esp`)

<br>

# **[Link to Added Mods List](/ModDetailsIndex.md)**

<br>

# Miscellaneous Patches and Tweaks

## Re-Add Nirnroot sounds from Immersive Sounds - Compendium

* Re-install Immersive Sounds - Compendium with a new name, but select whichever Nirnroot sound you prefer. Once installed, go into its Filetree and delete everything except for `sound/fx/itm_is/ingredient/itm_nirnroot_lp.wav`. Then just make sure it's after the original ISC mod in the install order.

**Link:** [Pre-made mod](/custom-patches/Immersive%20Sounds%20-%20Compendium%20Re-Add%20Nirnroot%20Sounds.zip)

## Mods that I have disabled/removed for more plugin slots

* "iEquip"
* "Toccata Follower SE (With Elisif Replacer Option)"
* "Not So Fast - Main Quest"
  * Also need to remove a patch from "LOTD Patches Merged" and rebuild
    * Go to Tools -> Tool Plugins -> Merge Plugins Hide, right click "LOTD Patches Merged", Enable Plugins
    * In "Legacy of the Dragonborn Patches (Official)", go to Optional ESPs tab and move `BCS_NotSoFast_Patch.esp` to optional
    * Open zEdit from the MO2 executable link, choose zMerge, and find the "LOTD Patches Merged" merge. Click on "Remove Unavailable Plugins" (it should just be the Not So Fast one missing), and then build and exit zMerge.
    * Go back into Merge Plugins Hide and disable plugins for "LOTD Patches Merged"

<br><br>

# Experimental/Temporary Bug Fixes and Consistency Patches

## Multi-version

### Update NPC AI Process Position Fix - SSE

This mod was updated after the LS 2.4.0 and LS 2.5.0 releases, just install the main file and replace

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/40261

### Organic Factions and Extension Update

This was tested with no stability issues on 2.4.0 by @ErikIEC, and that was without replacing the mod in the merge plugin. I have not played through with this change, but it seems to be stable from what I have seen

**Links:**
* https://www.nexusmods.com/skyrimspecialedition/mods/10289 (SSE OrganicFactions)
* https://www.nexusmods.com/skyrimspecialedition/mods/25471 (SSE OrganicFactionsExtension)
* [Patch by @ErikIEC with changes by @JaxomofRuatha](custom-patches/OrganicFactionsExtendedPatch.esp)

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.5.0)
  * Install and Replace "SSE Organic Factions" and "SSE Organic Factions Extension"
  * Rebuild "NPC Additions Merged"
    * Go to Tools -> Tool Plugins -> Merge Plugins Hide, right click "NPC Additions Merged", Enable Plugins
    * Open zEdit from the MO2 executable link, choose zMerge, and find the "NPC Additions Merged" merge. It should have "Organic Factions Extended" in yellow (and possibly the Serana Dialogue Additions) but otherwise be unchanged. Click "Build", and exit zMerge when done.
  * `OrganicFactions.esm` should be after `EnhancedAIFramework.esm` (this should happen automatically upon replacing the mod), and `OrganicFactionsExtendedPatch.esp` should go after `LS2 Patches Merged.esp`

### Fix for Archery Gameplay Overhaul and Pretty Combat Animations issue

Note: This may not work well in more recent LS versions, was originally for 2.0.2

**Link:** [Patch by TwistedModding](custom-patches/ago_pca_patch.rar)

**Load/Install Order Notes:**
* TwistedModding
  * Place this patch after the mod: Compatibility Patch for Archery Gameplay Overhaul (AGO) and XP32 Skeleton Styles MCM

### Fix for human Serana eyes (included in LS 2.4.0+)

Currently Serana's eyes once cured are linking to missing textures, this just links it to the one existing in the filepath.

**Link:** [Patch by JaxomofRuatha](custom-patches/JOR_SeranaEyesFix.esp)

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.2.1)
  * Patch ESP should go after LS2 Patches Merged

## LS 2.4.0

### Fix for 2.4.0 Revisited mods conflict

**Load/Install Order Notes:**
* ForgottenGlory
  * Move `BleakFallsBarrowRevisited.esp` and `UstengravRevisited.esp` to immediately after `Miscellaneous Patches Merged.esp` and before `BFBR_ELE_Patch.esp`

## LS 2.2.1

### Fix for 2.2.1 Black Face Bugs

**Link:** [Patch by JaxomofRuatha](custom-patches/2.2.1/LS2%20BFB%20Fixes%20Patch.esp)

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.2.1)
  * Patch ESP should go after LS2 Patches Merged
  
**Extra Notes**

Included NPCs in this patch are Golldir, Erandur, Vorstag, Madanach, Benor, Marcurio, Belrand, and Stenvar. The Men of Winter records were forwarded as is, so if there's changes in new LS releases, that might not be quite the same if there's customized patching.

### Clockwork patches for LOTD display temporary fix (LS 2.2.1)

Currently the Clockwork LOTD display is broken, because the patches for it are above the actual Clockwork ESP. According to several testers, it works to move DBM_Clockwork_Patch.esp and LOTD_TCC_Clockwork.esp below Clockwork.esp.

**Extra Notes**

This doesn't work correctly (from my experience) if done mid-save, the display doesn't get added and the LOTD Checklist gets glitched out. You may be able to rebuild the MCM and have it work.

<br><br>