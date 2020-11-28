# LS Unofficial Extras
Information about adding and testing mods for compatibility with Living Skyrim modlist

**IMPORTANT NOTE!!!**
This is a completely unofficial listing of mods that I and others from the Living Skyrim community have attempted to make work with the base Living Skyrim modlist. Adding ANY of these completely voids all support from ForgottenGlory and the Living Skyrim development team. Any custom patches are EXPERIMENTAL and load/install suggestions are ONLY SUGGESTIONS, using any of them is completely at your own risk.

I made this to collaborate on ideas, but it is entirely unofficial. You've been warned!

If you have issues or notice unresolved conflicts/bugs, please report them in an issue! Things may go out of date somewhat quickly, and either way I don't claim perfection with custom patches. Thank you!

## ESLifying and Important Caveats

Note that you will **need to ESL flag plugins** from the standard LS list to get any of these to work. The easy guide on how to do that is [here](https://tes5edit.github.io/docs/8-managing-mod-files.html#ESLifyingPluginstheeasyway). **DO NOT ESL FLAG BlockSteal.esp**

You will NOT be able to add EVERY SINGLE MOD HERE. The non-ESL limit for plugins is still 254, so you might have to choose some to get rid of if you want to include others. Depending on what you remove, you'll also have to patch accordingly (I try to treat LS as "one mod" for patching, so usually fine, but make sure to check in SSEEdit)

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

# **[Link to Custom Updates, Merges, and Reorganization](/CustomUpdatesIndex.md)**

<br>

# **[Link to Added Mods List](/ModDetailsIndex.md)**

<br>

# **[Link to MCM Options](/custom-mcm-settings/MCMSettingsIndex.md)**

<br>

# Miscellaneous Patches and Tweaks

## Re-Add Nirnroot sounds from Immersive Sounds - Compendium

* Re-install Immersive Sounds - Compendium with a new name, but select whichever Nirnroot sound you prefer. Once installed, go into its Filetree and delete everything except for `sound/fx/itm_is/ingredient/itm_nirnroot_lp.wav`. Then just make sure it's after the original ISC mod in the install order.

**Link:** [Pre-made mod](/custom-patches/Immersive%20Sounds%20-%20Compendium%20Re-Add%20Nirnroot%20Sounds.zip)


<br><br>

# Experimental/Temporary Bug Fixes and Consistency Patches

## Multi-version

### Patch for calming down Sea of Spirits sharks

This makes the sharks from Sea of Spirits a bit slower and less aggressive, as well as more difficult to end up on land.

**Link:** [Patch by @chosti-factor](/custom-patches/LS2.Sea.of.Spirits.Patch.zip)

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.5.2)
  * I loaded `LS2 Sea of Spirits Patch.esp` before `enemies_releveled.esp`

### Black Face Bug Patches 2.5.2 (possibly 2.4.0+)

This patch should fix most of the black face bugs from LS 2.5.2, specifically Frea and a bunch of other Dragonborn DLC NPCs, a couple of housecarls, and the Onmund fix @seanpbelcher originally created. You should be able to add this mid-playthrough, as long as it's at the VERY END of your load order. I wasn't able to fix Iona (BaseID 000A2C91), since her textures seem to be missing, so if anyone knows how to fix her let me know! Also happy to add any other BFB fixes if they're found when using this.

**Link:** [Patch by @JaxomofRuatha](/custom-patches/2.5.2/JOR_BFB_LS2.5.2_Patch.esp)

I'm including the original Onmund-only patch here as well, since I'm not sure the full one will work for LS versions prior to 2.5.2. If you're using the first patch, you do not need this one.

**Link:** [Onmund-only patch by @seanpbelcher](/custom-patches/2.4.0/Onmund_BFB_fix.7z)

### Fix options for race issues with Grace

There is an issue with the Grace version used by LS (and more importantly patched by LS2 custom patches), and there are two main ways of fixing it:

* Update "Grace - SkyRem Series AIO" to the newest version (5.3 at this time), and add [JOR_GraceUpdated_LS2Patches_Patch.esp](/custom-patches/JOR_GraceUpdated_LS2Patches_Patch.esp), loading the plugin after `zPatch.esp`. This will forward the official fix, and obviously adds any updates from the official mod
* Use [hazarduss' custom patch](/custom-patches/Conjure_Familiar_fix_LS252.7z), loading `Conjure_Familiar_fix_LS252.esp` after `zPatch.esp`. This just changes the Breton version of the Conjure Familiar spell to use the same one as every other race (which means no familiar leveling with player character)

There's also a problem with the Nord flaw in Grace applying the "less effective magic" flaw to things like potions. I haven't personally tested this fix, but [Grace_srRaceNordFlawPerk_fix2.esp](/custom-patches/Grace_srRaceNordFlawPerk_fix2.7z) should make it work as intended (again thanks to hazarduss for the patches!)

### Clarity fix for default load order

`ai overhaul patch.esp` is currently listed before `AI Overhaul.esp` in MO2, but in reality loads after it. I just moved the patch immediately after the main plugin (`AI Overhaul.esp` -> `ai overhaul patch.esp`) for clarity and to make sure that any intended overwrites happen as expected from the listed load order.

### Fix for Archery Gameplay Overhaul and Pretty Combat Animations issue

Note: This may not work well in more recent LS versions, was originally for 2.0.2

**Link:** [Patch by TwistedModding](custom-patches/ago_pca_patch.rar)

**Load/Install Order Notes:**
* TwistedModding
  * Place this patch after the mod: Compatibility Patch for Archery Gameplay Overhaul (AGO) and XP32 Skeleton Styles MCM

### Custom "kitchen sink" conflict resolution patch (only use if you know what you're doing)

I decided to upload the patch I created as the "final catch-all" conflict resolution patch for my "kitchen sink" playthrough of LS 2.5.2. There are some things in here that would probably be helpful even without all the extra stuff I have loaded, so feel free to make more modular edits to this if you know how, and I'll be happy to add them here, but it wasn't worth the effort to make separated patches pre-LS3.

**Link:** [Patch by @JaxomofRuatha](/custom-patches/2.5.2/JOR_FinalPatch_CustomExtras.esp)

**Load/Install Order Notes:**
* This is intended to load as the very last item in load order, as it's basically a custom override for my specific plugins.

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