## Music Mods Merged SSE Edition

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/4625

**Summary:** Adds a huge variety of popular music mods for Skyrim, allowing them to all work together

**LS2 Compatibility Status:** Good (no stability issues known after patching)

**Recommendations:** 
* JaxomofRuatha (Highly Recommend)

**Official Patches:**
* [OCW Patch](https://www.nexusmods.com/skyrimspecialedition/mods/4625)

**Custom Patches:**
* [JOR - Music Merged / LS2 Patches and ELE Patch (2.2.1, 2.4.0)](/custom-patches/2.2.1/JOR_MusicMerged_LS2Patches_Patch.esp)

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.2.1, 2.4.0)
  * MusicMerged.esp -> MMM_OCW-patch.esp -> JOR_MusicMerged_LS2Patches_Patch in that order should be anywhere after Occlusion.esp

**Extra Notes:**

This mod SEEMS to be stable if any individual mod/song is removed, but that hasn't been confirmed that I'm aware of with the mod author.

Also follow the instructions on the mod's page exactly and things should work fine. WITH A FEW EXCEPTIONS. These are the LS-specific differences I found:

* Any time that there is mention of a "Data/Music" folder, mods in MO2 are already operating in the "Data" folder, so a "Music" file in the top level of the mod Filetree is "Data/Music"
* Since Yggdrasil, Celtic Music (3 mods), and Immersive Music are already installed with base LS, you can just do the method for reinstalling them UNDER A DIFFERENT NAME (either from the mod or from the Downloads folder). **DO NOT** hide the original plugins if you are in the middle of a playthrough (and I wouldn't necessarily recommend doing it either way if you don't know exactly what you're doing, this mod's plugin overrides everything in any case)
* As a note, you can edit the mod's file structure either by going to "Information..." and then "Filetree" right clicking on the mod, or via the corresponding folder in the "mods" directory of the MO2 installation.
* This technically overwrites BS Bruma and Beyond Reach music options at the moment, I will try to patch this in the future, but I'm not confident in my understanding of how these music mods work at the moment.
