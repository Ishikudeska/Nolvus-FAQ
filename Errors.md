# Crashes

# PDPerfPlugin.dll+F125
If using DLAA and have black screen or crashes (don't forget DLAA is only compatible with Nvidia RTX cards), do this
uncheck these 2 plugins (In mo2, left panel under 1.1 SKSE PLUGINS) 
https://media.discordapp.net/attachments/908267876497121321/1128638535835070574/image.png?ex=65f1840c&is=65df0f0c&hm=49dbf86926733836450f301e8181f13f507fa29e22f883ad9b014fa33c0a385f&=&format=webp&quality=lossless
Then click on this in MO2
https://media.discordapp.net/attachments/908267876497121321/1128638679334793317/image.png?ex=65f1842e&is=65df0f2e&hm=aaefa4aabc121a0f0ea5384b636aada18e4115bf36c56d7daf3fa67840150085&=&format=webp&quality=lossless
Set bUseTAA to 1 
https://media.discordapp.net/attachments/908267876497121321/1128638849199902771/image.png?ex=65f18456&is=65df0f56&hm=e878f1cc83913f5ecc49533ead3ce75ffe60f8f315cec9cafcc4ae80bbcf96cb&=&format=webp&quality=lossless
Click on Save

# JContainers64.dll+10AE45
install this mod -> https://www.nexusmods.com/skyrimspecialedition/mods/108591?tab=files&file_id=458596
**make sure to place the plugin above FNIS.esp in the plugin window**

# Installer / Dashboard related

## "Failed to Download" Issues

### For Attack MCO mod:
[Click here to download file](https://modding-guild.com/archive/Attack_MCO-DXP_v1.6.0.6.zip)
Rename to `Attack+MCO-DXP+v1.6.0.6.zip`
Place archive file in `\Nolvus\Cache\Downloads` (do not extract it) and restart dashboard

### For ENB Binaries:
[Click here to download file](http://enbdev.com/mod_tesskyrimse_v0347.htm)
Place archive file in `\Nolvus\Cache\Downloads` (do not extract it) and restart dashboard
If the dashboard says something about a "virus," restart the PC, delete the cache folder from the Nolvus directory, then start the dashboard as administrator


### For High Poly Head:
[Click here to download file](https://drive.google.com/file/d/15_0njBUjHKidNnJPmLXEygzGVWsA3Zbq/view?usp=sharing)
Log into Google account if you cannot download in browser
Try with another browser if you still cannot download
Place archive file in `\Nolvus\Cache\Downloads` (do not extract it) and restart dashboard


### For BDOR Nova Pack:
[Click here to download file](https://shorturl.at/xSUZ9)
Log into Google account if you cannot download in browser
Try with another browser if you still cannot download
Place archive file in `\Nolvus\Cache\Downloads` (do not extract it) and restart dashboard

# Skyrim Game files messed up

Steam/Bethesda are having constant issues with providing the correct Anniversary Edition files and all of the Creation Club content. The most common errors reported by the Nolvus Dashboard are related to this issue. It can be frustrating to keep seeing "**Skyrim Anniversary Edition is not installed**" when you know perfectly well it is!

...at leat, it *should* be! If you encounter one of these errors (`hash for game file does not match`; `file does not exist`, etc.), follow the steps outlined here to force Steam to update your game appropriately. 

**IMPORTANT: Do *not* verify integrity of files during this process, as that may actually delete files you need for Nolvus.**

## Things to check first:
1. Make sure your Bethesda account is linked to the Steam account that owns Skyrim - you can do this on the Bethesda site. (There is an issue with family sharing when downloading the CC content, so use the account that owns Skyrim when doing this.)
2. Double-check that the folder where Skyrim is installed is the same folder shown in the error message.
 * If it's not, open **NolvusDashboard.ini** to adjust the `GamePath` accordingly.

## If you're still getting any of these errors after the steps above:
* Skyrim Anniversary Edition is not installed
* Hash for game file [...] does not match!
* [...] does not exist!
Then follow the special process for cleanly reinstalling Skyrim below.

# Clean Reinstall Skyrim:
1. Open your Steam Library and uninstall Skyrim (**Right-click -> Manage -> Uninstall**).
2. Open explorer and browse to the folder where Skyrim was installed (it will still be there).
3. Delete everything left inside this folder - *this step is crucial*.
 * (Example: open explorer to `E:\SteamLibrary\steamapps\common\Skyrim Special Edition`; anything left in there must be manually removed.)
4. Go back to Steam and reinstall Skyrim.
5. When Steam finishes installing, click **Play**.
6. When the main menu loads, you will see the prompt "Thanks for buying Skyrim Anniversary Edition!"
7. Click the **DOWNLOAD** button.
https://media.discordapp.net/attachments/1184826113059475496/1198383070475206757/image.png?ex=65f61334&is=65e39e34&hm=e669f744737d2448f4f9ce16c3d11da1dc0ac7a7238b9a456473c78a7795547e&=&format=webp&quality=lossless&width=893&height=605
8. Wait while Skyrim downloads several Creation Club files.
https://media.discordapp.net/attachments/1184826113059475496/1198383129845567680/image.png?ex=65f61343&is=65e39e43&hm=7538ecb3daa5ed5815883cc1eebe69d77dba6ed372f20f49beae831ace4f93f0&=&format=webp&quality=lossless
9. When completed, you will see another prompt: "The Creation selection / load order has changed. The game will now reload your data files."
10. Click **OK**.
https://media.discordapp.net/attachments/1184826113059475496/1198383204646780959/image.png?ex=65f61354&is=65e39e54&hm=585387eb9466b2d5ef2b61c326eda559d0699bbd65d73895e5910eeba924f294&=&format=webp&quality=lossless&width=489&height=350
11. The main menu will reload and the song will restart - at this point your update is complete, so click **Quit** to close Skyrim.
12. Now run your Nolvus Dashboard to restart the instance installation process.

# If you still get hash does not match, file does not exist, or Anniversary Edition not installed errors, then Steam still has not installed it properly.

As frustrating as it is, **repeat the process** above starting from #3 in the "Things to check first" section: https://discord.com/channels/740569699900719145/1184826113059475496/1198382830795886654
Eventually you *will* get the correct files and the Nolvus installation will be able to proceed.

# A global ModOrganizer instance has been detected
Hey there! See the fine print at the bottom? It's mentioning a folder that needs to be deleted - once that's done the installer should proceed

# Objecct reference not set to an instance of the object
## Error - Object reference not set to an instance of an object
There are two versions of this error, so follow the steps accordingly.
### Version 1: Many mods (sometimes hundreds!) appear with this error while downloading
This is an intermittent issue with the Nexus servers, easily fixed by changing download servers.
1. Close your dashboard, reopen it, and select a different Download Server before resuming.
2. If the mods resume downloading, you have successfully connected to the new server.
3. After that, if you want to switch back to your previous server (such as Nexus CDN, which tends to be faster), you can repeat step 1 above.
### Version 2: A single error occurs when opening the dashboard
This could either be a simple connectivity issue or a sign of a corrupted installation.
1. Make sure the Nolvus website isn't down. If it is, check here: https://discord.com/channels/740569699900719145/755346172243214376/1190760013506035774
2. Try closing and reopening the dashboard a few times to see if it connects.
3. If you still see the same error, close the dashboard and try running **NolvusUpdater.exe** to force an update.
4. If you've already installed Nolvus and just want to play, remember that you can bypass the dashboard and **launch Mod Organizer 2 directly** from `..\Nolvus\Instances\Nolvus Ascension\MO2\ModOrganizer.exe`
5. If you haven't finished installing and none of the above works, follow these steps to fix a corrupted dashboard/install: https://discord.com/channels/740569699900719145/755346172243214376/1191497095102857236

# audiomenu error
https://media.discordapp.net/attachments/755346172243214376/1190433069090480158/Untitled.png?ex=65f4d6b0&is=65e261b0&hm=a58bad4599858e9d6e7446c3872ea40a30d7271ddefaaef490ee7e6c47aea2ea&=&format=webp&quality=lossless&width=549&height=604

# installer not detecting my GPU
https://www.nolvus.net/guide/asc/setup

# Installer blank/frozen
If your Nolvus Dashboard window is blank and there isn't any progress indicated in the status bar at the bottom, close and reopen the dashboard. Remember, it's safe to do so at any time and it will resume where it left off.
https://media.discordapp.net/attachments/755346172243214376/1197025866568445962/image.png?ex=65f12336&is=65deae36&hm=c6b098aa6b68d452c0edea922d7cef43ea2d130f9c5cd7713f7a8c4f2a8479f0&=&format=webp&quality=lossless&width=865&height=605

# How to downscale to a custom resolution
in this case you need to do the things manually, double click on your SSE Display tweaks mod (in mo2) go to ini file tab and change like this. A note tho, if your custom resolution is not listed it could mean windows just does not recognize it (the installer just queries windows to get its available resolutions). Also the installer will not be inline with the custom resolution you manully setup (but it's not an issue, it will just not display it)
https://media.discordapp.net/attachments/755346172243214376/1184840381754515538/image.png?ex=65f2f318&is=65e07e18&hm=8249ac7b03b82640fc2c6222a62f4e29724ef5180a2a906f5a6d3d4be2076d23&=&format=webp&quality=lossless&width=1075&height=605 

# Mod Organizer related
I have this when MO2 starts from the Nolvus Dashboard
https://media.discordapp.net/attachments/908267876497121321/1162638626660810772/image.png?ex=65f53c99&is=65e2c799&hm=a0f978bfb710f750cbbe67c7626dc141a1cf0d55fecbcaf54b40396c0b2ce566&=&format=webp&quality=lossless&width=855&height=605
Just click on switch to this instance button

# Mod Organizer is white / no Nolvus mods showing
Try this
https://media.discordapp.net/attachments/755346172243214376/1198390544527806524/image.png?ex=65f61a2a&is=65e3a52a&hm=89e442358c6bacce425fa3807e05ca28e71d1e74a7b843438daf45acf9384e70&=&format=webp&quality=lossless&width=960&height=605

# DLL Plugin Loader -Initialize() crashed... Contact the author...
I get this error
https://media.discordapp.net/attachments/908267876497121321/1151868710106169434/image.png?ex=65f2f855&is=65e08355&hm=afa03909f90f73ff7e06296ae31f1ef52be7496bdde8f54d4ab61eedcd130cdd&=&format=webp&quality=lossless
1. This happens if you try to launch skyrim from MO2 when a SkyrimSE.exe instance is already running. 
2. Close it first (maybe kill the process in the Task Manager) 
3. Close MO2
4. Restart MO2
5. Restart the game from MO2

# Trampoline.h(187): Failed to handle allocation request
EngineFixes.dll says "SKSE/Trampoline.h(187): Failed to handle allocation request"
* Open Windows Explorer and Right-click on the **Documents** folder (the one in quick access)
* Select **Properties** and then **Location**
* If you see the path is still OneDrive, try to restore default.
* If that doesn't work, follow the steps in this article: https://support.microsoft.com/en-gb/topic/operation-to-change-a-personal-folder-location-fails-in-windows-ffb95139-6dbb-821d-27ec-62c9aaccd720

# In-Game related:

## Static Skill Leveling menu not appearing? Points not assigning? Sleep menu says "Wait" instead of "Rest?" Exhaustion not reducing?

**How it happens:**
* Never start a new character or load a save without completely exiting the game first. Doing so can cause scripts to break and has been known to mess with things like the sleep menu and static skill leveling.
* Never change stances while in the middle of another animation (like mid-swing). If your stances break, it can cause other issues like with the sleep menu and static skill leveling.
* If you're using SunHelm, always be sure to sleep long enough! If you wake up still tired, weary, or exhausted, the skills you assign may not apply to your character and will be lost forever. (There is a patch that prevents this from happening here: https://www.nexusmods.com/skyrimspecialedition/mods/110009)

**How to fix:**
* If your exhaustion level is not going down no matter where you sleep, check whether your sleep menu says "Wait" instead of "Rest."
* If your static skills menu never shows up after sleeping, check whether your sleep menu says "Wait" instead of "Rest."
* Draw your weapon and check to see if stances are working. If not, quit the game completely, then reload a save from before it broke.
* Now lay in a bed; if your sleep menu still says "Wait" instead of "Rest," **check the Go To Bed MCM and make sure the "Sleep Modifier" key is *unmapped*** (screenshot below). If not, unmap it!
* If none of the above work and you still can't seem to sleep or level up, there is a magical tea you can add to the game that resolves exhaustion and forces sleep: https://www.nexusmods.com/skyrimspecialedition/mods/110018
https://media.discordapp.net/attachments/755346172243214376/1199795000075100261/image.png?ex=65f1fbab&is=65df86ab&hm=ea1670a859464c5cd790e13b9330af123dae10355c720749f60dd39ad78c6a0f&=&format=webp&quality=lossless&width=550&height=341

# windows DPI custom scaling
If you use Windows Custom scaling (right click on your desktop => Display Properties => Scaling percentage) is higher than 100% your game will be zoomed in

In this case you have 2 possibilities

Set your windows scaling back to 100%
Keep your custom scaling and follow these steps
Go to your SSD:\NOLVUS\STOCK GAME directory (for manual installation) or SSD:\NOLVUS\INSTANCES\[INSTANCE_NAME]\STOCK GAME (for auto installation) . Right click on SkyrimSE.exe and set as follow.

# my game window is too small / not filling the screen
Nolvus Skyrim is windowed borderless by default, don't change that. 

**If your game window is too small** then make sure that your dashboard and windows resolutions match.

# I have graphic glitches, overly dark or crazy color grading
I have graphic glitches, dark color grading,...
 
If you use Medal software disable it


# This is the only FAQ for customized modlists
Keep in mind that the Flat Map Framework will give you a 
# blue or purple screen 
if anything overrides it. This is similar to all map mods; no matter what else you add or change in your customized list, **make sure the mods (left side) are not overridden by anything, and the plugins (right side) are always in the order shown, and are at the very bottom of the load order with nothing else below them.**
https://media.discordapp.net/attachments/1168063977029382235/1168067167766466591/image.png?ex=65ed4cd2&is=65dad7d2&hm=e1d9411d538658579fb05a7ab2e62e4dc42500694a4054328badc7fd94fd4b43&=&format=webp&quality=lossless&width=550&height=273 
