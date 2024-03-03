# Cabbage ENB setup

The full directory for your Nolvus STOCK GAME folder can be found in C:\Nolvus\Instances\Nolvus Ascension\STOCK GAME, which will be referred to as Nolvus\STOCK GAME.

[Optional] Backup your enbseries folder , enblocal.ini , enbseries.ini , enbcomplexparallax.ini , enbgrasscollisions.ini , and if you have it the Nolvus Reshade.ini for if you want to revert to old enb or break something.

1. Open file explorer to Nolvus\STOCK GAME and delete the contents inside of enbcache folder , enbseries folder , enbseries.ini , enblocal.ini , enbcomplexparallax.ini , enbgrasscollisions.ini , and if you have it the Nolvus Reshade.ini

**NOTE:** Some ENBs do not generate enbcache folder or other files- if you don't have them don't worry about deleting or backing them up. Some ENBs also have their own .ini (e.g. Bjorn Dark Ages.ini), be sure to delete those.

2. Download Cabbage ENB https://www.nexusmods.com/skyrimspecialedition/mods/103042?tab=files

3. Download NAT.ENB - ESP WEATHER PLUGIN v3.1.1C - Fixed
https://www.nexusmods.com/skyrimspecialedition/mods/27141?tab=files

4. Download Season Weathers Framework - NAT-ENB III - 3.1.1C https://www.nexusmods.com/skyrimspecialedition/mods/63562?tab=files

5. In Mod Organizer 2 add both NAT.ENB - ESP WEATHER PLUGIN v3.1.1C - Fixed and Season Weathers Framework - NAT-ENB III - 3.1.1C , place them with your other weather mods and enable them. Now disable Natural Atmopsheric Tamriel III and Natural Atmospheric Tamriel III - Season Weathers. **Note:** Exact position may differ based on install preset/other mods added.
<img src="https://media.discordapp.net/attachments/755346172243214376/1190939448293199882/image.png?ex=65ed73cb&amp;is=65dafecb&amp;hm=2740beee6e4f2e994075d9ddb59c6d79d33559098df4ad9ac65d42af1fc043df&amp;=&amp;format=webp&amp;quality=lossless" alt="Image"/>
**NOTE:** Make sure you also move any added .esp above FNIS.esp in the right side of MO2

6. Extract the files from the **lux** directory of the Cabbage ENB to Nolvus\STOCK GAME overwriting all the files there.

7. Download the Nolvus V5 ENB settings for Cabbage and the Nolvus Reshade from https://www.nolvus.net/guide/asc/enb (Press CTRL+F type "Cabbage") 

8. Extract the files from Nolvus Cabbage ENB Settings into Nolvus\STOCK GAME overwriting all the files there.

9. Extract the file from Nolvus Reshade into Nolvus\STOCK GAME overwriting all the files there.

**NOTE:** Be sure to disable all mods related to your previous ENB used. E.g. Bjorn ENB Dark Ages NAT Patchs. If using Rudy ENB only disable the Rudy ENB Nat Addon file.

Now you're done! Enjoy Cabbage ENB!

# PureDark's DLSS upscaler

1. Make sure you selected **DLAA** as your anti-aliasing option when initially installing Nolvus v5. TAA will not work. With DLAA selected, much of the configuration groundwork needed for DLSS will already be in place.

2. Go to PureDark's patreon. For $5 it will give you instructions for linking your discord account to patreon, so you can access the DLSS files on their discord. You can find the files in their **skyrim-beta-access** channel.

3. If you have an nVidia **40xx** card and want DLSS3 Frame Generation:
 * Download **SkyrimUpscalerFGBuildAlpha03.zip**
 * Download **ModifiedReShadeForDLSS3.zip**
 * Go to step 5

4. If you have any other RTX card, or want DLSS2:
 * Download only **SkyrimUpscalerENBTestBuild11.zip**
 * Skip step 5

5. If you downloaded the **ModifiedReshadeForDLSS3.zip** file, open it now and extract **dxgi.dll** into the `X:\Nolvus\Instances\Nolvus Ascension\STOCK GAME` folder. This will overwrite an existing file.

6. Go to MO2. Nolvus includes a non-paid version of the mod already (called "`Skyrim Upscaler`" in section 1.1 SKSE PLUGINS) - **disable it as well as** "`Upscaler Base Plugin`." 

7. Install the SkyrimUpscalerFG or SkyrimUpscalerENB zip file you downloaded just like any other mod in MO2, and place it in section 1.1 after the Skyrim Upscaler you just disabled. It will be called something like "`SkyrimUpscalerENBTestBuild11`". Enable it.

8. You're done, run the game. 

9. OPTIONAL: I recommend just running it with the defaults out of the box (see step 8), but you can open the **SkyrimUpscaler.ini** file from this mod to configure things like `mUpscaleType = 0` (which is DLSS, which it already should be), change `mQualityLevel` (default 4 Ultra Quality), or change the `mDLSSPreset` (Default 6). 
Consult PureDark's discord for more info about what these do if you want to start playing with them.

10. OPTIONAL: If you have any **sharpness** or **shimmering** issues while using the upscaler, it is recommended to disable **Depth of Field (DoF)** effects.
From the base game:
* While in game, press Escape to open the system menu
* Select Settings and click on Display
* Scroll down to find the Depth of Field slider and drag it all the way to the left

From the ENB:
* While in game, press Shift + Enter to open the ENB menu
* In the bottom portion of the left pane, expand the EFFECT section
* Un-check `EnableDepthOfField` (if it is already unchecked, that's fine)
**---------------------------------------------------------------------------------**

# Potato mode guide

**STORMHAND'S DEFINITIVE POTATO'S GUIDE - THE ONLY CHANCE YOUR POTATO PC HAS TO RUN NOLVUS ULTRA 😅 **

Stormhand's Tweeks for potato PCs:

1. Install Nolvus Ultra with the following options:

* TAA Anti-aliasing (if you want DLAA it means you have a RTX card so you are NOT a proud owner of a potato PC - this guide is not for you ;)
* Choose Low Ini Settings (it doesn't really matter here because you will replace with my personal INI files);
* choose ULTRA performance for LOD Settings;
* you can choose SMP physics if you want, but do NOT take Fake raytracing option
* select FPS stabilizer
* Always play at 1080p (downscale if you have a 1440p monitor);

2. Make sure you have these lines on your enbseries.ini (for Ambient Occlusion settings):
[SSAO_SSIL]
ResolutionScale=0.3
SourceTexturesScale=0.3

And for lightning particles:

[COMPLEXPARTICLELIGHTS]
BigRangeScale=0.25

3. Reinstall Mod Embers XD as guide suggests, but check Performance Option on the FOMOD installer

4. VERY IMPORTANT: use CAO Textures Optimizer - for reducing trees and roads textures https://www.nexusmods.com/skyrimspecialedition/mods/23316

Check your settings as the picture bellow (all tree mods downsized to 2k, all grass mods downsized to 1k);

5. NVIDIA Video Driver Settings
Max Performance on energy management for Skyrim SE specific settings.