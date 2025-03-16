# UEFN-PIE
 Play-in-Editor for Unreal Editor for Fortnite

Allows you to go ingame using UEFN on Save the World and Battle Royale gamemodes.

tldr it's carbon but in editor instead

1. Download [27.11 FN and UEFN](https://gofile.io/d/cBUDZ9).
2. Download UEFN-PIE's your required version's code as a ZIP and extract it to the same location your Fortnite folder (merging FortniteGame folders).
3. Download [xdelta](https://www.romhacking.net/download/utilities/598/) and set "PIE_XXXX_v1.xdelta" as the patch and UnrealEditorFortnite-Win64-Shipping.exe in "FortniteGame/Binaries/Win64" as the Source File, make sure the target file is an exe inside the Win64 folder.
4. Download [Fiddler Classic](https://www.telerik.com/download/fiddler), once Fiddler is set up copy the contents of FiddlerScript.txt and paste it into the FiddlerScript tab inside Fiddler, go into Tools -> Options -> HTTPS and make sure Capture HTTPS CONNECTs, Decrypt HTTPS traffic, Ignore server certificate errors (unsafe) are all checked, then click Actions and Trust Root Certificate clicking yes when prompted.
5. Download [Neonite](https://github.com/HybridFNBR/Neonite), and run run.bat.
6. Make a shortcut to the patched exe you just created with the arguments "-disableplugins=ValkyrieFortnite -enableplugins=ValkyriePIE", then go to the path "%localappdata%\UnrealEditorFortnite\Saved\Config\WindowsEditor\" copy the Engine.ini to that location, then make it read only by right clicking on the file, -> properties > attributes: read only.
7. Open your patched exe from xdelta, click on Edit in the top left, then Editor Preferences..., scroll down to Play Credentials and Enable Logins and add Credentials, User Id will be your username on Neonite, Password doesn't matter but needs to be filled in, Type should be set to epic or exchangecode.
8. In UEFN Click the three dots next to Platform and scroll down to NetMode, make sure it is set to Play Standalone and click play, if it loads into lobby, try again.

Once everything is set up you just need to have fiddler and Nenonite open to play PIE! Select a map and set the GameMode override in the world settings to BattleRoyale_Gamemode to load BR, the default gamemode is STW.

Equip items by adding to the Inventory Items to Grant in the Editor Preferences in Save The World Cheats or Battle Royale Settings depending on gamemode.

## Notes
- 24.20 is the best version for PIE.
- Save the World Gamemode doesn't work on 30.XX builds
- Crouching/Sliding doesn't work on Chapter 5 builds

## Features
- Battle Royale and Save the World ingame (both only on 24.20)
- Battle Royale Map Support on 24.20, 27.11, 30.30
- Equipping weapons
- Building and editing
- Using any cosmetic
- Lego and FallGuys Gamemode on 30.30, kinda

## Credits
- boredcrow24 - made most of the patches in this repo
- simonhxd - worked on majority of blueprint functionality for ingame
- wiktorwiktor12a - better animations patch for UEFN
- sizzyleaks and taijames - inventory
- gamerbross - random help
- tkd_kedis - sandbox map
- mineekdev - ingame patch for 27.11
