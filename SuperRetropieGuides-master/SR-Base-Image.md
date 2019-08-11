![SR Image](https://sinisterspatula.github.io/SuperRetropieGuides/images/SRimage-short.jpg)

[Back to Index](https://sinisterspatula.github.io/SuperRetropieGuides/)

[![https://drive.google.com/drive/folders/1RhvzNFKofJvrKzaiEXZqsB5kJ1cykDVb](https://github.com/SinisterSpatula/SuperRetropieGuides/raw/master/images/theme.png)](https://drive.google.com/drive/folders/1RhvzNFKofJvrKzaiEXZqsB5kJ1cykDVb "Download the base image")

 > Super Retropie Image Rev C Download is now available for the public.  We've worked very hard on this and hope you enjoy it.  If you need help, please consider joining our active retrogaming community.

## Release Information

# Super Retropie Image Rev C

## Features
 1. Brand new Retroboy v2 Theme supporting video snaps.
    1. Many Custom Collections logos
    1. Gamelist font size increased, better readability.
    1. Video view is completely rebuilt and looks super awesome.
1. Bootup logo (appears in only 6 seconds thanks to custom kernel)
1. New pre-installed Ports
    1. Streets of Rage Remake
    1. Outrun Engine (Cannonball)
    1. Open Bor 3400
    1. Open Bor 6xxx
    1. Duke Nukem 3D
1. Advanced Control Framework v2
1. Preconfigured controls for many standalone emulators
1. Pisnes pre-installed, snes9x removed. (Pisnes is actually a newer snes9x, they are the same code base)
1. GBC color correction disabled in retroarch config for lr-gamebatte (better color saturation for GBC)
1. Standard fixes and tweaks
    1. Wait for network on boot -- disabled (faster boot, causes no issues)
    1. Mono mixdown audio
    1. System file checking bypass
    1. Bootup is 100% hidden (no text), and looks smooth, bootup logo appears, then boot movie, then emulation station.
    1. Also hidden are the xboxdrv text from Advanced Controls framework during game launch.

## Getting Started

# What do I need to get things setup after writing the SD card?
> Add your Wifi name and password: First locate the wpa_supplant.conf. Modify the file with your real wifi name and wifi password and then drop it in the boot partition. Remember pi zero only supports 2.4 Ghz networks, so you should set your 2G ssid and not your 5G.

* Add your bios’ and roms
    * Place your bios for the systems you plan to play into your bios directory.
    * Please refer to the Retropie Wiki for more information: [RetroPie-Setup/wiki](https://github.com/RetroPie/RetroPie-Setup/wiki)
    
    * Place your roms to the roms directory under the proper folder.
    * Please refer to the Retropie Wiki for more information: [RetroPie-Setup/wiki](https://github.com/RetroPie/RetroPie-Setup/wiki)
    
    * The games under Ports will also need roms.
    * Please refer to the Retropie Wiki for more information: [RetroPie-Setup/wiki](https://github.com/RetroPie/RetroPie-Setup/wiki)
    

## Some other cool things you can do:

  *	Add video snaps and screenshots by “Scraping” your roms.  See [https://www.skraper.net](https://www.skraper.net)
  * If you want to reduce the size of your video snaps to free up room for games, and make them load faster, see our guide here: [https://sinisterspatula.github.io/SuperRetropieGuides/snapsconversion](https://sinisterspatula.github.io/SuperRetropieGuides/snapsconversion)
  
  * Setup your videos as a screen saver: [Video Snaps ScreenSaver](https://sinisterspatula.github.io/SuperRetropieGuides/VideoSnapsScreenSaver)
  
# FAQ

 > I added a new system and roms but they are not showing up? (only affects early downloads)
 * Delete the systems.cfg in configs/all/emulationstation/systems.cfg
 
 > What version of Retropie does this have?
 * It has version 4.4
 
 > Does it have gpsp and pcsx-rearmed standalone?
 * Yes, and yes.
 
 > My D-pad doesn't seem to be working.
 * Please hold select button and D-pad Up arrow until your power light blinks Purple.
 
 > How do I use the custom collections?
   1. highlight and select "Game Collection Settings"
   1. highlight and select "Create New Custom collecion From Theme"
   1. highlight and select "system of choice"
   1. to add games, highlight "game of choice" and press "Y"
  
 > Can I make the video snaps silent?
 * Yes, in your emulation station settings there is an option to turn off audio for videos.

# Download:
[Click HERE to download the base image](https://drive.google.com/drive/folders/1RhvzNFKofJvrKzaiEXZqsB5kJ1cykDVb)

## Support Thread
[Join our active community for help](https://www.facebook.com/groups/SuperRetroPie/)

[Back to Index](https://sinisterspatula.github.io/SuperRetropieGuides/)

###### Head back to our [Facebook Group](https://www.facebook.com/groups/SuperRetroPie/)

## Image updates since release:

8/10 - Major openbor fixes (thanks Santi for encouraging me to get this fixed).  Both openbor's should work properly now.  Rom's directory moved from roms/ports/openbor to roms/openbor (so they aren't duplicated to the ports section).  Openbor is now it's own system, with a new carousel logo (thanks Travis!).  This also means that the two openbor's are now managed through the runcommand menu (press a key just before launch).  Pisnes is set to full screen by default now, if you prefer pixel perfect, you can change it back by setting maintainaspectraio=1 in /opt/retropie/emulators/pisnes/snes9x.cfg (this update also includes the controller tools update that fixes controls for Gpi cases that have a different ID name - possibly new gamepad firmware?)

8/5 - Added Eulationstation Collections script to the Retropie Menu.  Updated Outrun (cannonball) to use 30 fps for better performance.  Added update protection for the Gpi Case patch, it won’t get overwritten from an update now. (We still advise to always make a backup and don’t recommend you update (especially without a backup first).

