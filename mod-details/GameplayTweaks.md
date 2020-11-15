## SSE Gameplay Tweaks

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/41953

**Summary:** Adds various misc options to configure. Read description of mod for details. 

**LS2 Compatibility Status:** Good (no issues, no patching required after updating .NET Script Framework)

**Recommendations:** 
* JaxomofRuatha (Highly Recommend)

**Official Patches:**
_None_

**Custom Patches:**
_None_

**Load/Install Order Notes:**
_None_
 
**Extra Notes:**

You will NEED to update ".NET Script Framework" to the latest version to use this mod.

The mod starts out as being fully disabled, only making changes as they are enabled in the `NetScriptFramework/Plugins/GamePlayTweaks.config.txt` file inside the mod. I don't like a lot of the changes, but here's what I personally ended up changing in that config file:
* CumulativeTrainingTimesPerLevel.Enabled = True
* TeammateDetection.Enabled = True
  * TeammateDetection.TeammateUndetectableWhenSneaking = True
  * TeammateDetection.TeammateUndetectableIfPlayerIs = True
  * TeammateDetection.TeammateUndetectableNoCombat = False
  * TeammateDetection.TeammateRequiresWeaponOut = True
  * TeammateDetection.TeammateRequiresNotSneaking = True