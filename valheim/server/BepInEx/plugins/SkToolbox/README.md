SkToolbox - Valheim
AUTHOR: Skrip (https://steamcommunity.com/id/Skrip037/)
Toolbox Version: 1.10.5
Valheim at time of release: 0.202.19

SkToolbox is a fully clientside utility meant for improving the gameplay experience, by enabling the player to modify their character or the environment to their liking. The mod enables features that could allow a player to drastically change their character or others.

It is recommended that you use discretion when using these commands in Multiplayer, as this will affect the gameplay experience of others.

:: REQUIREMENTS ::
BepInEx for Valheim - If you get errors in your console, remove Valheim.DisplayBepInExInfo from the plugins folder if it exists!
Unstripped UnityEngine, Core, IMGUI, InputLegacy, Physics, and UI modules.

:: FEATURES ::
• This mod works by extending the functionality of the console and chat commands. Most of the commands shown below are usable in both the console and via chat. Most commands work both via console or chat.
• The SkToolbox now allows customization of the look of the console. Changes have been made by default. See the configuration file for details.
• Please see NexusMods page for most up to date feature list.

:: HOW TO INSTALL ::
	Method 1
	• Simply use your mod manager (Vortex is recommended) to download and manage the files. Make sure your mod manager includes a working version of BepInEx.
	• Run the game and enjoy.
	Method 2
	• Simply open the zip file and extract all contents to the game's root directory (You'll see valheim.exe and UnityPlayer.dll in this folder).
After extraction, in the game root folder, you should see the Valheim.exe file, and the BepInEx folder in the same folder. (https://i.imgur.com/QKx9yxU.png)
	• Run the game and enjoy.
	Method 3 (Only Updating or you have a working installation of BepInEx already installed)
	• Place the dll file in the BepInEx plugins directory.
	• Run the game and enjoy.

• I just need to update! What do I do?
	• Extract the .dll file to the plugins folder, run the game.

:: HOW TO USE ::
• Complete one of the two installation methods, then simply run the game and open the console.
	• Type help or /?
	• (/? also works as a chat command)

:: CHANGELOG ::
• Version 1.10.5 (Hearth and Home Update)
	[KNOWN ISSUES]
		- Command Aliasing is not working
	!!	- Command Autorun is not working 
		- Command Chaining is not working
		- Command Hotkeys are not working. Please attempt to use the new bind standard command.
		- Command Autocomplete for specific commands (/give, /spawn, etc)
		- Running commands in the main menu can cause errors in the console.
	[FIX] Mod now works other than the issues listed above. Fixes are in progress.
	[CHG] The On-Screen menu is now clickable when you are in the Escape menu!

• Version 1.10.4
	[NEW] /spawntamed - /spawntamed [Creature Name] [Level=1] - Spawns a tamed creature in front of you. Capitals in name matter!
	[NEW] /optterrain - Optimize old terrain modifications. Added so this can be used from chat by default.
	[FIX] Autorun example command modified.
	[FIX] /echo works properly again.
• Version 1.10.3
	[CHG] More performance changes.
	[FIX] Fixed a scenario that could crash the game when opening the console.
	[CHG] More effective at overriding when other mods try to disable the console.
	[NEW] New config option to completely disable chat output from the mod. (Default chat output is enabled)
• Version 1.10.2
	[NEW] Now runs in it's own thread alongside the game for better performance!
	[NEW] Now attempts to allow console even if other mods attempt to disable it.
	[CHG] Added padding onto the console.
	[NOTE] Sadly the terrain issue persists at this time.
• Version 1.10.1
	[NEW] Added index to config file for easier navigation.
	[NEW] Added configurable limit to how many rows can be stored in the scrollable console.
	[FIX] Numerous bug fixes, small changes, and performance optimizations.
• Version 1.10.0
	[NOTICE] It is recommended you delete your config file when coming to this version.
   ![NEW] Configurable hotkeys now available! Run the game to activate the new config, then check the new settings!
   ![NEW] The console now supports unlimited output history and enables scrolling!
    [NEW] /console [0/1] - Toggle the console. No parameter with toggle. 1 = Open, 0 = Closed. Intended for use with hotkeys and aliases.
• Version 1.9.0
   ![NEW] Command aliasing has been added! Create your own commands to call other commands!
	[NEW] Added command /listprefabs - List all prefabs/creatures. Optionally include name starts with. Ex. /listprefabs Troll returns any prefab that starts with the letters 'Troll'
	[NEW] Added command /echo - Echos text back to the console
	[UPD] Tab autocomplete now checks for all SkToolbox commands and aliases
	[UPD] Tab autocomplete now works on parameters on the following commands: /spawn, /give, /env
	[UPD] Improved Error Handling
	[CHG] Modified /spawn command so if an item is spawned, the quantity will be set to the level parameter.
• Version 1.8.5
	[FIX] Error appeared in console upon opening inventory
• Version 1.8.4
   ![NEW] Rudimentary auto-completion has been added (start typing a SkToolbox command then press tab!)
	[NEW] Console Enabled is now a configuration option. Defaulted to true. 
	[REM] /event and /randomevent removed as they don't work properly in multiplayer.
	[CHG] Changed some command descriptions
• Version 1.8.3
	[FIX] /imacheater now works as expected again
	[FIX] /env works properly. Broke it right before release by accident on 1.8.2.
	[CHG] More performance changes / refactoring
	[CHG] Changes to the on-screen menu options
• Version 1.8.2
	[NEW] /env [Weather Name] - Change the weather. No parameter provided will list all weather. -1 will allow the game to control the weather again.
	[NEW] /event [Event Name] - Start a named event
	[NEW] /randomevent - Start a random event
	[NEW] /freecam - Toggle the freecam
	[NEW] Console input style can now be modified. Now styled by default.
	[FIX] On-screen menu no longer opens if the toggle button is pressed while the console and/or chat is open
	[FIX] Added additional error checking
	[FIX] Refactored the command processor. Significantly refactored the entire toolbox
• Version 1.8.0
   ![NEW] Version Checker has been implemented. Toolbox will now alert when an update has been released.
	[NEW] New configuration option added - OpenConsoleWithSlash
	[NEW] New configuration options added - ConsoleFont, ConsoleFontSize, ConsoleOutputTextColor, ConsoleSelectionColor, ConsoleCaretColor. 	These allow the customization of the look of the console. Console now set to new look settings by default
	[NEW] New configuration options added - Alternate on-screen controls are now fully configurable!
• Version 1.7.0
   ![NEW] AutoRun commands and command chaining now work with any command, including the standard commands and most other custom mods!
	[NEW] New configuration options added - AllowPublicResponse, AllowExecuteOnClear, OpenChatWithSlash, AllowChatCommandInput
	[NEW] /clear - Clears the current output shown in the console
	[NEW] /q - Quickly exit the game from the console
	[CHG] Many behind the scene fixes and optimizations
	[CHG] Terrain modification radius' limits changed again based on new equations
   ![FIX] /seed is back and working!
	[FIX] The caret is now set properly on command scroll in console
	[FIX] /tp is now much more likely to properly calculate the height of the ground and place the player accordingly. Sometimes there is still a 'blocked' issue, but this now happens less often. The workaround is to fly up into the air before teleporting, so nothing can block your destination.
	[FIX] Chat now opens properly when an output from the Toolbox is sent to chat.
• Version 1.6.3
	[NEW] /tu added to world on-screen menu
	[NEW] /resetmap - Reset the map exploration
	[FIX] Terrain modification commands have been significantly optimized, with credit to BlueAmulet for this code. Thanks BlueAmulet!
• Version 1.6.2
	[FIX] /nores - You can now properly remove structures if they were built in a restricted area
• Version 1.6.1
	[CHG] On-Screen menu will no longer open if the console is already open
	[FIX] /farinteract with no range in auto run caused auto run to run twice
• Version 1.6.0
	[NEW] /nores - Toggle no restrictions to where you can build (except ward zones)
	[NEW] /tu [Radius=5] - Undo terrain modifications around you. Radius 40 max.
	[NEW] On-Screen World commands added!
	[NEW] /wind and /resetwind added!
	[CHG] Changes some command descriptions
	[FIX] Terrain commands had a radius actually stuck at 20. Changed this to 40
	[FIX] On-screen toggle text fixed
	[FIX] Fixed a console functionality issue where if you hit ctrl+A then backspace, it would execute the command.
• Version 1.5
    [NEW] Auto-run commands on server-join
    [NEW] Command chaining! For example: "/give Wood 5; /give PickaxeWood" would run both commands!
    [NEW] Command chaining works with auto-run!
	[FIX] Terrain Commands are now working really well, should no longer cause stuttering or game breaking issues!
    [CHG] Modified the position of the /detect window so it no longer covers the inventory
• Version 1.4
	[NEW] /nosup - Toggle building support requirements 
   ![NEW] Terrain Editor - /tr /td /tl - Raise, dig, and level terrain in a radius
	[NEW] Alternate controls now available for on-screen menus. /alt (then use Home, insert, page up, page down, and delete)
	[FIX] Down arrow now properly cycles the console commands as expected
	[FIX] Console no longer strangely executes commands too many times sometimes
• Version 1.3
  !![NEW] Modified the console so you can now press the up arrow to get as many previous commands as you've entered.
  !![NEW] On-Screen Controls!
	[NEW] Teleport to Mouse
	[NEW] /set difficulty [Player Count] - Set the difficulty (default is number of connected players)
	[NEW] /set exploreradius [Radius] - Set the explore radius (default = 100f)
	[NEW] /set jumpforce [Force] - Set jump force (default 10). Careful if you fall too far!
	[NEW] /set pickup [Range] - Auto pickup radius can now be set (default 2)
	[NEW] /set speed [Speed Type] [Speed] - Speed Types: crouch (def: 2), run (def: 120), swim (def: 2)
	[NEW] /clearinventory - Clears the player inventory
	[FIX] Infinite stamina no longer causes lag, and is actually infinite now.
	[CHG] /listitems no longer requires caps
	[FIX] Backend changes. Performance increasecis.
	[CHG] /? is now organized by pages. Ex. /? 1
	[REM] /seed removed until it is properly working
	[REM] /findtrader removed until it is properly working
	[REM] /itp removed until it is properly working
	[REM] /ttp removed until it is properly working
	[CHH] Changes to give command. It now can be used with different parameters: /give [Item] [Qty=1], OR /give [Item] [Qty=1] [Player] [Level=1]
• Version 1.2
	[UPD] Updated BepInEx Version
	[NEW] /listskills will list all possible skills
• Version 1.1
	[CHG] /detect now has a range variable. /detect 50 (/detect performs a default of 20)
	[NEW] /imacheater now enables standard in-game cheats on any server (for you only)
	[FIX] /heal [Player=local] now properly heals other plyers
	[NEW] /set skill [Skill] [Level]
	[NEW] /seed - Display the world seed
	[FIX] /coords now show correctly
	[FIX] /tp now works correctly
	[CHG] /? now has pages. /? 1 or /? 2
	[NEW] /stopevent has been added
	[REM] /imaxstacks has been removed until properly working

:: KNOWN ISSUES ::

:: CREDITS ::
♦ Mod authored by: Skrip
♦ ♦ ♦ https://steamcommunity.com/id/Skrip037/

♦ Thank you to the Harmony team for their patcher.
♦ ♦ https://harmony.pardeike.net 

♦ Thank you to the Doorstop team for their injector.
♦ ♦ https://github.com/NeighTools/UnityDoorstop

♦ Thank you to the BepInEx team for their injector.
♦ ♦ https://github.com/BepInEx/BepInEx

♦ Thank you to BlueAmulet for the optimized terrain modification code.