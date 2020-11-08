## Fossil Mining - With Legacy Support

**Link:** https://www.nexusmods.com/skyrimspecialedition/mods/14107

**Summary:** Adds fossils that you can find while mining to make mining more profitable and interesting, brought to you with the help of the creator of Legacy of the Dragonborn with built-in Legacy support! 

**LS2 Compatibility Status:** Good (no known issues after patching and updating script)

**Recommendations:** 
_None_

**Official Patches:**
* [Legacy of the Dragonborn](https://www.nexusmods.com/skyrimspecialedition/mods/30980)
* [The Curator's Companion](https://www.nexusmods.com/skyrimspecialedition/mods/38529)
* https://www.nexusmods.com/skyrimspecialedition/mods/2656 (FMPSE 9-9 Script (v2.0))

**Custom Patches:**
_None_

**Load/Install Order Notes:**
* JaxomofRuatha (LS2 version 2.4.0, 2.5.2)
  * `Fossilsyum.esp` before `ELE_SSE.esp`
  * `DBM_Fossils_Patch.esp` and `LOTD_TCC_Fossils.esp` in that order, currently before `ELE_SSE.esp` (NOTE: I reinstalled the Legacy of the Dragonborn Official Patches and Legacy of the Dragonborn SSE - The Curators Companion with different names and no other patches enabled to get these)
  * The "FMPSE 9-9 Script (v2.0)" mod can be added anywhere after the main Fossil Mining mod, it just needs to overwrite the script. This way you get 3x the ore from a mining spot, but the fossil chance will trigger. Apparently it is possible to forego this, but there may not be fossil checks on a single ore deposit (it seems like there is a global counter for "number of hits" that persists between nodes)