Uploading this open source mod from Nexus Mods because it's not on Thunderstore yet.

Developer: [daccaor](https://www.nexusmods.com/valheim/users/111680948)

Original mod link: https://www.nexusmods.com/valheim/mods/351

## Change the graphic settings in a deeper way in order to improve performance or go beyond the limits of standard options.

About

It started as a simple mod that allows you to change the graphic settings aiming to improve performance on old pcs, now it's becoming a full granular controler over all graphics configuration. Note: the default configuration has the standard values for the game. In order to see changes you have to manually alter the config file or download one of the config files in the files tab. This mod will override shadows, vSync and distance/lod options, use the config file to change these options instead of game menu.

These settings are experimental. There are a lot of settings and we don't have time to thoroughly test all of them. If you find something that doesn't work or have any suggestion please let us know.

How to Use

Extract the mod into your BepInEx/plugins folder.

WARNING: If you're updating from a version previous to 1.1.0 be sure to delete the GraphicsConfigPlus folder from BepInEx/plugins!
Open the game to generate a config file in BepInEx/config and alter the values to your liking, OR download one of the config files in the files tab and place it into BepInEx/config.
Note: You can apply any changes made to the config file while playing, just press the Home key. You can change the key in config file.

Config Files

The balanced config file is used to run the game on a GTX 650Ti at 30 fps (i lock the fps with vSync option) with some effects enabled. Shadows are disabled because they coust too much for my old GPU, but by enabling SSAO with some quality changes the game doesn't  become too plain.
The performance config is used to play the game on i5 intel graphics notebook at 30 fps (with some drops to 20). It's not perfect and the game is kinda ugly, but it's a miracle it runs at all.

If you are here not to increase performance but give a boost on graphics you can just start the game to create the default config file and take a look at these settings: MaxFPS or vSyncCount, ShadowResolution, ShadowDistance, SunShaftsResolution, AOsampleCount and MBsampleCount.

Available Options

General

Select the hot key to reload config file while playing
Print the original values and current values for the configurations on the BepInEx log
Enable or disable Anisotropic Filtering
Set texture size limit
Set max. pre-rendered frames queued up by graphics driver
Set particle raycast per frame
Set maximum number of light pixels on an object
Enable or disable real-time reflection probes
Set maximum number of bone weights that can affect a vertex
Enable or disable soft blending for particles
Enable or disable two-pass shader for terrain vegetation
Set LOD distance (even beyond game limit)
Set vSync count, enable or disable vSync, but also can be used to lock fps below screen refresh rate without disabling vSync
Set target FPS, can be used to lock fps below or above screen refresh rate when not using vSync

Shadows

Set number of cascades for directional light shadows
Set shadow drawing distance
Set shadow quality

PostProcessing

Enable or disable all Post Processing effects (kills the game presentation but gives a big boost on fps; will invalidate all bloom and sunshaft options)
Set SunShafts resolution
Set SunShafts blend mode (changes how the effect is presented)
Enable or disable Bloom AntiFlicker
Enable or disable SSAO down sampling to reduces the effect quality and gain some performance
Set SSAO far distance
Set SSAO sample count to improve quality or performance
Enable or disable SSAO high precision for a better effect quality
Set Anti-alising method to use between Fxaa and Taa

Flavor

Set bloom intensity
Set bloom radius
Set LensDirt intensity
Set the SunShafts intensity
Set gamma correction
Set SSAO intensity
Set SSAO to only affect ambient light
Set Chromatic Aberration intensity

Advanced

Set the SunShafts max radius
Set the SunShafts blur radius
Set the SunShafts radial blur iterations (decreasing can give a little performance boost)
Set BloomSoftKnee
Set Motion blur frame blending
Set Motion blur sample count
Set Motion blur shutter angle

## **Code**
https://gitlab.com/daccaor/GraphicsConfigPlus/-/tree/master/

## **Credits**
This mod is based on ValheimFPSBoost.
https://www.nexusmods.com/valheim/mods/147