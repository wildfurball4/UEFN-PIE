# UEFN-PIE
 Play-in-Editor for The Big Bang event for 27.11 uefn

tldr it's carbon but in editor instead (and the BR map works if you have a lot of ram!)

## How to install

1. Download and Setup [27.11 PIE](https://github.com/wildfurball4/UEFN-PIE/tree/main/27.11)
2. Download UEFN-PIE's code as a ZIP and extract it to the same location as 27.11 (merging FortniteGame folders).
3. Make a shortcut to the patched exe you just created with the arguments "-enableplugins="DurianRoot" -disableplugins="ValkyrieFortnite""
4. Move [these pak files](https://github.com/wildfurball4/UEFN-PIE/blob/durian/image.png) into another folder, just not in the main paks folder.
5. Make sure you have Neonite open and open your shortcut. When UEFN is loaded, click the three dots next to Platform and scroll down to NetMode, make sure it is set to Play as Client and click play.
6. Once PIE loaded into the frontend, close pie.
7. After closing PIE, head to the Durian plugin folder (Plugins/Events/Durian)
8. To easily forceload every map (except juno) you can simply open the ForceLoad_Durian level
9. You can manually forceload assets by opening the NewBlueprint blueprint
10. use this template for forceloading assets
```
{
	"Tagged": [
		[
			"lev",
			""
		]
	]
}
```
Example:
```
{
	"Tagged": [
		[
			"lev",
			"/Script/LevelSequence.LevelSequence'/Durian/Sequences/Durian_Rufus.Durian_Rufus'"
		]
	]
}
```
11. After setting up your asset with your template select the lev variable, and press "Paste All Properties in Category" and if you did it correctly, you will see your asset refrenced in the variable.
12. To play ingame set the NetMode to Play Standalone and set the GameMode override in the world settings to BattleRoyale_Gamemode, and stream in Durian levels
