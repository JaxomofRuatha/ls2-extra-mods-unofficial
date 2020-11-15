## Nemesis Unlimited Behavior Engine

This is a REPLACEMENT for FNIS, and as such cannot be run alongside it. For the moment, all of the mods that use Nemesis and are incompatible with FNIS will stay on this page.

Also note that some of the additions I'm not personally using and have been a bit weird with interactions between them (mostly CGO and MBO), and even with the ones I have included in my playthough this is all pretty experimental as I'm not super confident in my ability with animation-related mods.

**Link:** https://github.com/ShikyoKira/Project-New-Reign---Nemesis-Main/releases

**Summary:** A replacement for FNIS, allowing for new types of animation and behavior mods to be used in Skyrim.

**Load/Install Notes:**
* Install the "Nemesis" mod from the RAR file downloaded. Also create an empty mod called "Nemesis Output" I place them after their FNIS counterparts ("Fores New Idles in Skyrim SE - FNIS SE" and "FNIS Output") but shouldn't be necessary.
* Go to Tools -> Executables, and "Add from file". Select "Nemesis Unlimited Behavior Engine.exe" from inside the "Nemesis" mod in the MO2 mods folder. Then check "Create files in mod instead of overwrite" and choose "Nemesis Output".
* Disable "Fores New Idles in Skyrim SE - FNIS SE" and "FNIS Output"
* Assuming you're keeping "Archery Gameplay Overhaul SE" installed (recommended), you will need to install the "Nemesis Patch" file from https://www.nexusmods.com/skyrimspecialedition/mods/24296. I installed it as a separate mod right after "Archery Gameplay Overhaul SE".
* Once you have finished adding any mods that have animations and moved them to the correct location in install/load order, run the "Nemesis Unlimited Behavior Engine" executable. Always select "Update Engine" first, then check and of the mods that you are using (plus "Gender Specific Animations"). Then "Launch Nemesis Behavior Engine". Wait for it to finish, then close out. Once you refresh, "Nemesis Output" should be filled, and a new `FNIS.esp` should appear in your plugins (currently I've had no problem ESL-flagging this plugin, since it's only a dummy...I did place it right after `DeadlySpellImpacts.esp` in load order, where the original was, though I don't believe it matters)

**Extra Notes:**
* If you're installing mods that MO2 does not recognize correctly (from this list that should be "Archery Gameplay Overhaul SE - Nemesis Patch" and "The Ultimate Dodge Mod Attack Cancel"), just make sure that the first folder down is the same level as "Nemesis_Engine" (setting the data folder if need be). MO2 still won't recognize it, but just tell it to ignore the error.

### 360 Movement Behavior SE

If you want to use this, disable "360 Walk and Run Plus". This is a strictly superior option in my experience, but it does use an ESP slot and has a few compatibility concerns with other Nemesis mods.

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/33139

**Load/Install Notes:**
* If you are using this mod with "The Ultimate Dodge Mod", install this mod before it
* I installed `DSer360MovementBehavior.esp` immediately after `JZBai_ThrowingWpnsLite.esp`, and before any other Nemesis mod plugins

### The Ultimate Dodge Mod and The Ultimate Dodge Mod Attack Cancel

**Links:**
* https://drive.google.com/file/d/0B2VgBVA9jE6RTjJiYnRTTE9qRUE/view
* https://www.nexusmods.com/skyrimspecialedition/mods/40313 (Optional, allows to attack cancel)

**Load/Install Notes:**
* I installed "The Ultimate Dodge Mod" and "The Ultimate Dodge Mod Attack Cancel" in that order after all the other Nemesis mods
* I loaded `Ultimate Dodge Mod.esp` after `DSer360MovementBehavior.esp` and before `Nemesis PCEA.esp`

### Dynamic Animation Replacer

This mod doesn't really do much by itself that I'm aware of, but it adds additional checks for conditional animations to be used by other mods.

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/33746

**Load/Install Notes:**
* I installed this before "DAR - Dynamic Swimming" and "Jump Behavior Overhaul SE" just because both require it, but I don't believe install order should matter as long as the Nemesis patch is enabled and run.

### DAR - Dynamic Swimming

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/34853

**Load/Install Notes:**
* Shouldn't matter where this is installed, I just put it in the group of Nemesis mods after "Dynamic Animation Replacer"

### Jump Behavior Overhaul

If you're using CGO, there are some instructions on the mod page for how to get them to mostly play nice.

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/36889

**Load/Install Notes:**
* I installed "Jump Behavior Ovehaul SE" after "Ultimate Combat SE" and "360 Movement Behavior SE", but before "The Ultimate Dodge Mod"

### Project New Reign - Nemesis PCEA

To my understanding, this mod is intended to replace other combat animation mods, and allow to dynamically use/change between multiple animation packs in-game. As long as the plugin is installed, you should be able to add or remove animations safely from the list as long as you re-run Nemesis afterward.

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/31667

**Load/Install Notes:**
* It shouldn't matter where you install this, but I did personally disable "Pretty Combat Animations" and "PCA_1hm Animations Overhaul" once this mod was installed (and added the animations from those into this)
* I loaded `Nemesis PCEA.esp` after all other Nemesis plugins, ending up before `WardsFunctionalitiesExtended.esp`
* Usage and installation of animation packs is kind of odd, so here's how I did it for the Pretty Combat Animations one as an example:
  * Under both "Pretty Combat Animations" and "PCA_1hm Animations Overhaul", I copied all of the files from `meshes/actors/character/animations`, combined them in a folder, and then named that folder `1Pretty_Combat_Animations`. I then placed that folder inside the "Project New Reign - Nemesis PCEA" mod under `meshes/actors/character/animations/Nemesis_PCEA`
    * NOTE: the folder can apparently be named whatever you want for this to work, but the folder name with the animations MUST lead with a unique number from what I understand. The default installed animations are `0Dser_Animations`, and if I were to install another pack I would prefix it with a `2`, for example
  * After re-running Nemesis (it should show any of the new packs in the logging), the in-game MCM should show them. Just select the ones you want to use. My understanding is that the higher the number, the higher the priority when it comes to conflicting animation files, and making changes to the animations should take effect after a short delay.

### Movement Behavior Overhaul

I didn't end up actually using this mod, because when using the gamepad it doesn't really provide much value unless you make changes to how the gamepad registers (even with the patch). It also conflicts with CGO if you're using that, though it should technically be "compatible".

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/38950

**Load/Install Notes:**
* It shouldn't matter where this is installed, but I added it after "Dynamic Animation Replacer"
* I loaded `MBO.esp` before `Ultimate Dodge Mod` and after `DSer360MovementBehavior.esp`

### Combat Gameplay Overhaul

This mod does A LOT of things, and conflicts in some way with most other Nemesis mods. Unfortunately, there's not a way to "a la carte", so I ended up not using it for my playthrough, but I love some of the features it adds. As such, I'm just making basic install notes, but really this will likely need to be tweaked for compatibility/consistency if you're planning on using CGO (it seems easiest to just have it overwrite damned near everything, even though the animations don't end up being the nicest).

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/33767

**Load/Install Notes:**
* I installed this after "360 Movement Behavior SE" and before "Jump Behavior Overhaul SE" and especially "The Ultimate Dodge Mod"
* I loaded `DSerCombatGameplayOverhaul.esp` after `DSer360MovementBehavior.esp`, and before `Ultimate Dodge Mod.esp`