# RIP Bozotendo, 3DS

!!! warning "Important Warning"

    Until I say it isn't, **this megathread will continually be in a state of WIP**! I am continually working to add things to here that may be pertinent to us. If you want information on something, please let me know. I will try my best to update this thread as needed or as I come along certain information.

## Disclaimers

- Please know that there will be some proper terminology to understand! The word "root" may come up a lot in discussion regarding the file structure of your SD card, which means when you are currently not in any folder on your SD card.
    - Additionally, you may see terms like "FBI" and "Universal Updater", which are apps installed after hacking your 3DS. This "3DS" chapter of this megathread is intended to be read sequentially, so you may come across terms you may not quite understand if you aren't reading in the proper order.
- Hopefully, your 3DS is of the "New" variety, because you'll get the most juice out of it. This seems like a no-brainer, but if you really care about stuff like PS1 emulation on the 3DS then it only runs on the "New" models.
    - Additionally, if you have a "New" model 3DS, please know that they run on microSD cards. The "Old" model 3DS family runs on bigger sized SD cards. If you plan to buy a new SD card for this project (you should, as the stock SD card is too small), please plan accordingly. **This megathread will from here on out refer to your storage card as an "SD card", regardless of how big or small your's is in physical size**.
- As for SD card size, technically, the 3DS only supports SD cards up to 32 GB. HOWEVER, you can format your SD card on your computer so that it actually works with your system. The correct format is FAT32, and this megathread will get into how to format it to such in a bit.
    - I would recommend either getting a 64 or 128 GB SD card, as that's all you'll realistically need and any more than that might just lag the system due to its limited strength.
- Everything that is mentioned here can also be applied to a 2DS variant model, but for simplicity's sake I will refer to both 3DS variants and 2DS variants as simply just the 3DS.

## Formatting your SD Card (Assuming You Have a 64+ GB SD Card)

### Windows

1. Go to [this website](http://ridgecrop.co.uk/index.htm?guiformat.htm).
2. The website generally looks a bit old, but just click the giant image of the formatter and it will install guiformat.exe
3. Insert your old SD card into your computer, the one that's in your 3DS currently before upgrading it.
    - *Make sure your 3DS is turned off before taking it out of your system*!
4. Take anything and everything in that SD card and put it somewhere on your computer you'd remember. This is **CRUCIAL** as formatting your SD card wipes everything. Make sure you also don't play around with the locations of every file inside the folders, alas it should just be dragging and dropping them somewhere.
5. Eject your old SD card from your computer. Do not throw it out just yet.
6. Insert your new SD card into your computer now.
7. In guiformat, select the letter for your SD card (E://, for example. your computer's hard drive is the C:// drive).
8. If your SD card is exactly 64 GB, enter 32768 in the allocation unit size. Otherwise, 65536.
9. Enter anything for the volume label.
10. Make sure "Quick Format" is selected.
11. Press "Start" and "OK", then once done close the application.
12. Drag and drop the contents of your old SD card into the newly formatted SD card.
13. Eject your new SD card from your computer and insert it into your 3DS.
14. Turn your 3DS on. If your system boots correctly, you may now throw away your old SD card. Otherwise, repeat this process from step 3 until it works.

### Linux

1. Using your distro's package manager (`apt-get`, `pacman`, or `flatpak`, to name a few), install GParted. This can be done by opening a Terminal window and installing as outlined by the distro's documentation.
2. Insert your old SD card into your computer, the one that's in your 3DS currently before upgrading it.
    - *Make sure your 3DS is turned off before taking it out of your system*!
3. Take anything and everything in that SD card and put it somewhere on your computer you'd remember. This is **CRUCIAL** as formatting your SD card wipes everything. Make sure you also don't play around with the locations of every file inside the folders, alas it should just be dragging and dropping them somewhere.
4. Eject your old SD card from your computer. Do not throw it out just yet.
5. Insert your new SD card into your computer now.
6. Back in your Terminal, type `sudo gparted`.
7. Find your SD card in the drop-down box at the top right of the GParted window.
8. Right-click on the unallocated /dev/sdb1 and select Format to and click fat32.
9. Click the green checkmark and then the Apply button to apply the changes. This may take a bit.
10. Once this is finished, close out of GParted.
11. Drag and drop the contents of your old SD card into the newly formatted SD card.
12. Eject your new SD card from your computer and insert it into your 3DS.
13. Turn your 3DS on. If your system boots correctly, you may now throw away your old SD card. Otherwise, repeat this process from step 2 until it works.

### MacOS

1. Insert your old SD card into your computer, the one that's in your 3DS currently before upgrading it.
    - *Make sure your 3DS is turned off before taking it out of your system*!
2. Take anything and everything in that SD card and put it somewhere on your computer you'd remember. This is **CRUCIAL** as formatting your SD card wipes everything. Make sure you also don't play around with the locations of every file inside the folders, alas it should just be dragging and dropping them somewhere.
3. Eject your old SD card from your computer. Do not throw it out just yet.
4. Insert your new SD card into your computer now.
5. Open a Terminal window on your Mac.
6. Enter `diskutil list`. A bunch of seemingly-gibberish will show up, however, your SD card will follow the format of `/dev/diskX` on the list of disks, along with the "name" of the SD card showing up somewhere in its respective section
7. Enter `sudo diskutil eraseDisk FAT32 (name) MBRFormat /dev/diskX`. Make sure you change X to the disk number you got earler, and change (name) with the name of your SD card. You will be prompted to enter your admin password, so please do so.
8. Once it is finished, drag and drop the contents of your old SD card into the newly formatted SD card.
9. Eject your new SD card from your computer and insert it into your 3DS.
10. Turn your 3DS on. If your system boots correctly, you may now throw away your old SD card. Otherwise, repeat this process from step 1 until it works.

## 3DS Hacks Guide

!!! info ""

    <https://3ds.hacks.guide/>

This website will continuously stay up to date with the latest information on how to hack your 3DS.

!!! danger "AVOID AT ALL COSTS"

    Do **NOT** attempt to follow video guides on how to hack your 3DS! The written guide linked above is continuously being updated, and it could be even a matter of days until a video guide goes outdated as they all follow what they see on this exact guide. The instructions on the written guide are easy enough to follow along to!

## Updating Luma3DS

!!! info "Please Read!"

    Luma3DS is the name of the custom OS you install on your 3DS after hacking it. However, it does not have anything to do with the system version that is displayed in your System Settings application. By updating Luma3DS, you are **NOT** updating your system's firmware. You are simply updating the tool that allows for unsigned homebrew to run on your system in the first place, allowing for less buggier experiences running homebrew. In fact, some newer homebrew require the use of an updated version of Luma3DS.

1. Open Universal Updater from your Home Menu.
2. Search for "Luma3DS". It should look like a light blue Luma from Super Mario Galaxy.
3. Download the `boot.firm` file.

!!! danger ""

    Do ***NOT*** download the nightly version unless you are willing to work around potential bugs! It may give you access to features early, but you'd have to update it every night and these nightly releases aren't exactly bug tested. It's best to avoid unless you know what you are doing!

4. Once that's finished, press Start to exit the Universal Updater.
5. Turn off your 3DS.
6. Turn your 3DS back on, but this time press and hold Select before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.
7. You should now see the Luma menu. Note that there is a version number at the top. It should be higher than what it originally was.
8. Press Start to resume the normal boot process.

## Pirating Games/DLC/Updates/(Official) Themes

!!! info "About hShop/3hs"

    hShop is an archive of most of all 3DS and (as of November 2026) DS content that was available. hShop provides their service for absolutely zero cost to the end user. They do provide a standalone app called 3hs, which eliminates the need for a computer when downloading their content. However, there are some drawbacks to that such as needing your 3DS to be on a stable internet connection when the 3DS just does not have proper Wi-Fi drivers compared to a proper computer in today's age (meaning slower download times from 3hs). This section of the megathread tells you how to download content from this archive irrespective of which method you prefer.

!!! warning "Branching Pathways"

    Due to the nature of the platform we will be using now following 2 respective worlds of content, the pathways below will branch out based on the kind of content you will be looking at. I have formatted the guide accordingly. **HOWEVER**, if you are pirating a DS game, you will need a tool called TwiLightMenu++ installed. I have also attached instructions for that here as well.

### (Prerequisite for DS Games) Installing TwiLightMenu++

!!! info "What Is This?"

    TwiLightMenu++ is a piece of homebrew that acts as a frontend launcher for another piece of homebrew called ndsBootstrap, which allows you to run ROMs of DS games on a (3)DS family system utilizing the native hardware rather than emulation. If you install the former, you will not need to install the latter, since it will bundle ndsBootstrap with the program. It tries to mimic the feel of the Home Menu of a DSi, so if you have/had one of those, you'll feel very familiar with it already! It should also go without saying that if you already have this installed, you will not need to reinstall it unless you want to update the program.

1. Open Universal Updater from your Home Menu.
2. Search for "TwiLightMenu++". The icon should look like "TM" with 2 plusses below it.
3. Download `TwiLightMenu++`. If you'd like, you can also download any of the other addons the install provides, though it won't be necesary for this guide.

!!! danger ""

    Do *NOT* install the nightly version, for the same reasons as you wouldn't install the nightly Luma3DS version.

!!! warning ""

    It may ask you to extract a `roms` folder. Since this is a first install, this is recommended for new users.

4. On your Home Menu, open TwiLightMenu++.
5. After some time (be patient), it will ask you for a language. Select the language you want.
6. Next, it will ask you for a region. Choose your region of choice.
7. Be patient as the application will now initialize everything. Once it's finished, you should see a bunch of folders.
8. Navigate to the `nds` folder and press A to select it
9. Exit out of TwiLightMenu++ by pressing the Home button and then A.

### Through hShop

Use this method if you can't connect your 3DS to the internet!

1. Go to [this website](https://hshop.erista.me/).
2. Search for whatever you want on their website.
3. Click on "Direct Download (.cia)" or "Direct Download (.nds)".
4. Turn off your 3DS.
5. Take out its SD card and insert it into your computer.

#### For 3DS Games

6. Take the `.cia` file that you downloaded from hShop and drag it into the `cias` folder that you should have made when hacking your 3DS.
    - If this `cias` folder does not exist, please make one in the root of your SD card.
7. Take your SD card out of your PC.

!!! warning ""

    Make sure you do it safely by manually clicking eject on the file explorer, as we do not want to risk corrupting your game file!

8. Put your SD card back in your 3DS and turn it back on.
9. Open FBI from your Home Menu.
10. In FBI, select "SD".
11. Navigate to your `cias` folder.
12. Select "&lt;current directory>".
13. Select "Install and delete all CIAs".
14. Once your game is finished installing, press B as much as you can to back out to FBI's main menu. Press Start after that.
15. Your game should now appear in the Home Menu as a "gift". Themes that you download will *not* automatically be installed, rather an installer will appear on the Home Menu which when ran once will uninstall itself while downloading the theme for use with Anemone3DS. This theme will now be "unofficial" to your system, at which point you can follow steps 7-10 of my section on installing unofficial themes found later in this megathread.

!!! warning "Games Crashing?"

    **If your game works from here, you're done**! However, some games (for example, Rhythm Heaven Megamix) may require you to download a seed for them to work otherwise the console will crash. hShop will tell you whether or not the seed is needed. The following steps will detail how to import that seed and for it to work with your 3DS. Do be warned, however, that if you've used 3hs before (outlined in the next section), you may not need to use these steps.

!!! danger "Make Sure To Do This!"

    If you are on Pretendo servers (instructions on how to do that are found later), make sure to switch back to Nintendo servers before doing this!

16. Back on your computer, re-open the page for the game you downloaded from hShop if it isn't open already.
17. Click on "Download seed for FBI".

!!! danger "Do NOT!"

    Do ***NOT*** change the name of the file for the seed that you just downloaded! This will mess things up come time for use with your 3DS!

18. Turn off your 3DS.
19. Take out its SD card and insert it into your computer.
20. Take the `.dat` file that you downloaded from hShop and drag it into the `/fbi/seed` folder that you should have made when hacking your 3DS.
    - If this `seed` folder does not exist, please make one in the `fbi` folder of your SD card.
21. Take your SD card out of your PC.
22. Put your SD card back in your 3DS and turn it back on.
23. Open FBI from your Home Menu.
24. In FBI, select "Titles".
25. Navigate to the game you had installed prior and select it.
26. Navigate to "Import Seed" and select it.
27. Confirm the selection.
28. Press A once the importing has finished. This process is very quick!
29. Press B and then Start to exit out of FBI.
30. Launch your game!

#### For DS Games

6. Take the `.nds` file that you downloaded from hShop and drag it into the `/roms/nds` folder that you should have made when installing TwiLightMenu++.
7. Take your SD card out of your PC.

!!! warning ""

    Make sure you do it safely by manually clicking eject on the file explorer, as we do not want to risk corrupting your game file!

8. Put your SD card back in your 3DS and turn it back on.
9. Open TwiLightMenu++ from your Home Menu.
10. Navigate to your game.
11. Launch your game!

### Through 3hs

Use this method as much as possible! That is, whenever your 3DS is connected to the internet.

1. Go to [this website](https://hshop.erista.me/3hs).
2. Click "Direct Download (CIA)"
3. Turn off your 3DS.
4. Take out its SD card and insert it into your computer.
5. Take the `.cia` file that you downloaded from hShop and drag it into the `cias` folder that you should have made when hacking your 3DS.
    - If this `cias` folder does not exist, please make one in the root of your SD card.
6. Take your SD card out of your PC.
7. Put your SD card back in your 3DS and turn it back on.
8. Open FBI from your Home Menu.
9. In FBI, select "SD".
10. Navigate to your `cias` folder.
11. Select "&lt;current directory>".
12. Select "Install and delete all CIAs".
13. Once 3hs is finished installing, press B as much as you can to back out to FBI's main menu. Press Start after that.
14. 3hs should now appear in the Home Menu as a "gift".
15. Open 3hs.
16. Search for whatever content you want and hit "Install".
17. Wait for the game to finish installing.
18. Press Start once the game is done installing to exit to the Home Menu.
    - If your game is a 3DS title or theme, it should now appear in the Home Menu as a "gift". Themes that you download will *not* automatically be installed, rather an installer will appear on the Home Menu which when ran once will uninstall itself while downloading the theme for use with Anemone3DS. This theme will now be "unofficial" to your system, at which point you can follow steps 7-10 of my section on installing unofficial themes found later in this megathread.
    - If your game is a DS title, do not panic if you don't see it on your Home Menu right away. It should have downloaded directly to your `/roms/nds` folder for use with TwiLightMenu++. As such, it won't appear on your Home Menu and you'll have to launch it through TwiLightMenu++.

!!! info ""

    **If you prefer the hShop method, know that to get a new game you have to start from step 1 every time**. However, **if you choose the 3hs method, 3hs is a one-time install, meaning that to get a new game you have to start at step 15**.

#### (Optional) Theming 3hs

Tired of the bland look of 3hs with no music playing in the background? I've scoured a few obscure places on the internet for you so that you can properly theme the app like how I did. There are other options out there, but for the purpose of everyone's sanity deteriorating by doomscrolling forum boards I won't be posting/promoting them.

You're going to need proper music and theme files. More traditional audio formats like `.mp3`, `.flac`, or `.wav` do not work with the 3hs app. Additionally, theming the 3hs app's interface doesn't take traditional formats for pictures like `.jpg`, `.png`, or `.gif`. You'd need to make them from scratch and/or convert existing `.wav` files into their format. Frankly, I think that's a waste of time for everyone involved.

1. Download a track and a theme from the sections below. You can do this by clicking on the link for them and following the instructions I've listed below for each.

!!! note "**<u>Music</u>**"

    - [nintendo 3ds eshop music but it's lofi](https://fileditchfiles.me/file.php?f=/s22/hXdFSJzNaVZeWVjbjFpi.hwav) *Click on "Download", then rename when saving. You can (and should) rename it to "nintendo 3ds eshop music but it's lofi" since this is the name of the [original SoundCloud track](https://soundcloud.com/roldyduarte/nintendo-3ds-eshop-music-but-its-lofi) I ripped this from.*
    - [June 2011 eShop Music](https://www.dropbox.com/scl/fo/vd35sx4s3gy0fix5t8fba/AFwPdq5s6eZ21H08HROjmbA/Nintendo%20eShop%20Music%20-%202011%20June.hwav?rlkey=xi1lekujj8wut5np75bfj6c51&e=2&dl=0) *Click on "Download", then click on "Continue with Download Only". This is the official eShop theme from June 2011, aka the launch of the 3DS.*

!!! note "**<u>Themes</u>**"

    - [Theme I Use](https://my.opendesktop.org/s/JHKJpSAkqrDYfge/download?path=%2F&files=heShopGreenNewEra%2Bbag.hstx) *Just click on this link.*
    - [Orange Variant Of Above](https://my.opendesktop.org/s/JHKJpSAkqrDYfge/download?path=%2F&files=heShop%2Bbag.hstx) *Just click on this link.*

2. Turn off your 3DS.
3. Take out its SD card and insert it into your computer.
4. Inside the `/3ds/3hs` folder of your SD card, create 2 folders if they don't already exist: `music` and `themes`.
5. Take the `.hwav` file you downloaded and put it in `/3ds/3hs/music`.
6. Take the `.hstx` file you downloaded and put it in `/3ds/3hs/themes`.
7. Take your SD card out of your PC.

!!! warning ""

    Make sure you do it safely by manually clicking eject on the file explorer, as we do not want to risk corrupting your files!

8. Put your SD card back in your 3DS and turn it back on.
9. Open 3hs from your Home Menu.
10. On the touch screen, with one of your fingers or your stylus tap on the icon that looks like 3 lines.
11. Navigate to the "Themes" section and select it.
12. Navigate to the theme you extracted earlier and select it.
13. Press B.
14. Navigate to the "Audio" section and select it.
15. On the touch screen, with one of your fingers or your stylus tap on the checkbox for "Repeat playlists and songs".
16. On the touch screen, with one of your fingers or your stylus tap on the button for "Manage playlists".
17. Press A to add a new playlist.
18. Name this playlist whatever you want, as the name of this playlist is unimportant.
19. Press A to enter the tracklisting for the new playlist you just created.
20. Press A to add a file.
21. Press A to add the track you extracted earlier.
22. Press B twice.
23. On the touch screen, with one of your fingers or your stylus tap on the textbox for "Default playlist".
24. Press A to select the playlist we created earlier.
25. On the touch screen, with one of your fingers or your stylus tap on the button for "playlist" under the `Select...` section.
26. Press A to select the playlist we created earlier.
27. On the touch screen, with one of your fingers or your stylus tap on the button on the bottom right to "Save" the configuration.
28. Press B twice.
29. Happy hShopping!

### (Optional) Making DS Games Show On Home Menu

Tired of having to open TwiLightMenu++ before being able to play a DS game? Why not make it show up on your Home Menu instead as if it was a normal 3DS title? Well, you can do that by just following the steps below! Do note, however, that if you pirate a new DS game you'll have to repeat these steps again.

1. Open Universal Updater from your Home Menu.
2. Search for "ndsForwarder". The icon should look like smiling cartoon narwhal.
3. Download `ndsForwarder.3dsx`.
4. Press Start to exit out of the Universal Updater.
5. Open The Homebrew Launcher.
6. Navigate to `NDS Forwarder Generator` and select it.
7. In this piece of homebrew, navigate to `/roms/nds/`.
8. Select `< Install All nds >`. Hit "Yes" to confirm.
9. Once finished, press Start to back out into The Homebrew Launcher.
10. Press the Home button to exit out into the Home Menu.
11. Your DS games should now appear on the Home Menu!

!!! warning "Title Limit"

    Nintendo was very restrictive in designing how the 3DS works in regards to how many titles one can have installed on their system at any given time. The 3DS can have at maximum 300 titles installed at once, 40 of which can be DSiWare. The forwarders created by homebrew count towards your 40 DSiWare title limit, meaning that **you can only have up to 40 DS games show up on your Home Menu at a time. You will need to play the rest through TwiLightMenu++.**

## Dumping 3DS Games

### From Cartridge To Home Menu

!!! info "Regarding Fresh Game Data"

    If you are dumping a brand new game and/or do not have any important save data, only follow steps 1, 2, 8-18, and 24.

1. Insert your cartridge of choice and open the game just for a quick second.
2. Close your game after a few seconds or so by pressing the Home button and closing the software.

!!! danger ""

    Do **NOT** take out your game cartridge at this point in time!!!

3. Open Checkpoint.
4. Find your game tied to your cartridge in the app. Checkpoint should tell you if the game is installed on the SD card or from a cartridge.
5. Select your game and press L to backup your save data. Press A to confirm.
6. Name this backup whatever you wish, as it's not important.
7. Once that's finished, press Start to exit out into the Home Menu.
8. Turn off your system.
9. Turn your 3DS back on, but this time press and hold Start before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.
10. You should now be greeted with GodMode9. It may ask you to reset the RTC datetime offset. Do not change the provided date, just mash A until you get to the menu.
11. Navigate to `[C:] GAMECART ()`
12. Select the `[game title ID].trim.3ds` file and choose "NCSD Image Options".
13. Select "Install Game Image".
14. Press A to unlock.
15. Follow the on-screen D-pad prompts.
16. Wait for your game to install, however long that takes.
17. Once that's done, back out as much as you can with the B button and then press Start. This will reboot the system like normal.

!!! note ""

    After the system is done rebooting, it's now safe to remove the cartridge from your system.

18. The game you see on your Home Menu will be a blank copy of your game. No save data, just raw game data. Open this so that Checkpoint will be able to recognize it.
19. Close the game after a few seconds or so by pressing the Home button and closing the software.
20. Open Checkpoint.
21. Find your game tied to your SD card in the app and select it.
22. You should have the option to restore the save since it's the same game. Restore it, obviously, by pressing R and selecting the name of the backup you made earlier.
23. Once that's done, close Checkpoint by pressing Start.
24. If you need to, reinstall updates using hShop/3hs.

!!! warning "Title Limit"

    Nintendo was very restrictive in designing how the 3DS works in regards to how many titles one can have installed on their system at any given time. The 3DS can have at maximum 300 titles installed at once, 40 of which can be DSiWare. This means that **you can only have up to 300 games show up on your Home Menu at a time. The rest of your 3DS library needs to be physical cartridges or emulated externally.**

!!! note "Emulators"

    These dumps are compatible with an emulator of your choice! More information on how to use these games with an emulator later.

### To ROM Format

#### From Cartridge

!!! info "Regarding Fresh Game Data"

    If you are dumping a brand new game and/or do not have any important save data, skip steps 1-7 and step 25.

1. Insert your cartridge of choice and open the game just for a quick second.
2. Close your game after a few seconds or so by pressing the Home button and closing the software.

!!! danger ""

    Do **NOT** take out your game cartridge at this point in time!!!

3. Open Checkpoint.
4. Find your game tied to your cartridge in the app. Checkpoint should tell you if the game is installed on the SD card or from a cartridge.
5. Select your game and press L to backup your save data. Press A to confirm.
6. Name this backup whatever you wish, as it's not important.
7. Once that's finished, press Start to exit out into the Home Menu.
8. Turn off your system.
9. Turn your 3DS back on, but this time press and hold Start before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.
10. You should now be greeted with GodMode9. It may ask you to reset the RTC datetime offset. Do not change the provided date, just mash A until you get to the menu.
11. Navigate to `[C:] GAMECART ()`
12. Select the `[game title ID].trim.3ds` file and choose "NCSD Image Options".
13. Wait for your ROM to properly dump.
14. Once that's done, press B to back out to the main menu.
15. Select `[0:] SDCARD`.
16. Navigate to `gm9` and select it.
17. Navigate to `out` and select it.
18. Navigate to the `.cia` file it built, and select it.
19. Select `CIA image options...`.
20. Select `Decrypt file (0:/gm9/out)`.

!!! note "Dual Paths"

    There may be a chance that your file is already decrypted. If that's the case, it will tell you "File is not encrypted". Skip step 21 by just pressing B if your ROM is already decrypted.

21. Wait for it to decrypt and then press A.
22. Press R + Start to shutdown your system.
23. Take out your SD card and insert it into your computer.
24. Your decrypted ROM is located in `/gm9/out/`. Copy your ROM to a location of your choice on your computer's hard drive.
25. Your save file is located in `/3ds/Checkpoint/saves/[game title ID] [game title name]/[backup name]/`. Copy your save file to a location of your choice on your computer's hard drive.
26. Take your SD card out of your PC.
27. Insert your SD card into your 3DS.

!!! note "Emulators"

    These dumps are compatible with an emulator of your choice!

#### From Home Menu

!!! info "Regarding Fresh Game Data"

    If you are dumping a brand new game and/or do not have any important save data, skip steps 1-7 and step 28.

1. Open the game of choice just for a quick second.
2. Close your game after a few seconds or so by pressing the Home button and closing the software.
3. Open Checkpoint.
4. Find your game tied to your cartridge in the app. Checkpoint should tell you if the game is installed on the SD card or from a cartridge.
5. Select your game and press L to backup your save data. Press A to confirm.
6. Name this backup whatever you wish, as it's not important.
7. Once that's finished, press Start to exit out into the Home Menu.
8. Turn off your system.
9. Turn your 3DS back on, but this time press and hold Start before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.
10. You should now be greeted with GodMode9. It may ask you to reset the RTC datetime offset. Do not change the provided date, just mash A until you get to the menu.
11. Press the Home button.
12. Navigate to `Title manager` and select it.
13. Navigate to `[A:] SD CARD` and select it. It will take a few seconds to load all the information regarding installed titles.
14. Navigate to your game of choice and choose `Manage Title...`
15. Navigate to `Build CIA (standard)` and select it.
16. Wait for your ROM to properly dump.
17. Once that's done, press B to back out to the main menu.
18. Select `[0:] SDCARD`.
19. Navigate to `gm9` and select it.
20. Navigate to `out` and select it.
21. Navigate to the `.cia` file it built, and select it.
22. Select `CIA image options...`.
23. Select `Decrypt file (0:/gm9/out)`.

!!! note "Dual Paths"

    There may be a chance that your file is already decrypted. If that's the case, it will tell you "File is not encrypted". Skip step 24 by just pressing B if your ROM is already decrypted.

24. Wait for it to decrypt and then press A.
25. Press R + Start to shutdown your system.
26. Take out your SD card and insert it into your computer.
27. Your decrypted ROM is located in `/gm9/out/`. Copy your ROM to a location of your choice on your computer's hard drive.
28. Your save file is located in `/3ds/Checkpoint/saves/[game title ID] [game title name]/[backup name]/`. Copy your save file to a location of your choice on your computer's hard drive.
29. Take your SD card out of your PC.
30. Insert your SD card into your 3DS.

!!! note "Emulators"

    These dumps are compatible with an emulator of your choice!

## Dumping DS Cartridges

!!! info "Regarding Fresh Game Data"

    If you are dumping a brand new game and/or do not have any important save data, only follow steps 8-23, 30, 34-39.

1. Insert your cartridge of choice and open the game just for a quick second.
2. Close your game after a few seconds or so by pressing the Home button and closing the software.

!!! danger ""

    Do **NOT** take out your game cartridge at this point in time!!!

3. Open Checkpoint.
4. Find your game tied to your cartridge in the app. Checkpoint should tell you if the game is installed on the SD card or from a cartridge.
5. Select your game and press L to backup your save data. Press A to confirm.
6. Name this backup whatever you wish, as it's not important.
7. Once that's finished, press Start to exit out into the Home Menu.
8. Turn off your system.
9. Turn your 3DS back on, but this time press and hold Start before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.
10. You should now be greeted with GodMode9. It may ask you to reset the RTC datetime offset. Do not change the provided date, just mash A until you get to the menu.
11. Navigate to `[C:] GAMECART ()`.
12. Select the `[game title ID].nds` file and choose "Copy to 0:/gm9/out".

!!! warning "About The `trim.nds` File"

    The `[game title ID].trim.nds` file is generally not recommended for DS games as there may arise playback issues. It's a good thing, however, that DS ROMs aren't that big in size anyway.

13. Wait for your game to copy, however long that takes.
14. Once that's done, back out as much as you can with the B button and then press Start. This will reboot the system like normal.

!!! note ""

    After the system is done rebooting, it's now safe to remove the cartridge from your system.

15. Open FBI from your Home Menu.
16. Select "SD".
17. Navigate to `/gm9/out`.
18. Select your ROM file, and then select "Copy".
19. Press B twice to get to your SD card's root. From there, navigate to `/roms/nds/`.
20. Select `<current directory>`.
21. Select "Paste".

!!! note ""

    **OPTIONAL**: If you would like, you can rename your ROM to whatever you'd like. For example, maybe the game's name. To do this, navigate to the pasted ROM file, select it, and then select "Rename". **Remember to keep its file extension of `.nds`**!

22. Press B twice to go back to your SD card's root. From there, navigate back to `/gm9/out/`.
23. If the original copy of your ROM is still located here, select it and press "Delete".
24. Press B twice to go back to your SD card's root. From there, navigate to `/3ds/Checkpoint/saves/[game title ID] [game title name]/[backup name]/`. This is where your save should be.
25. Select that save file and click "Copy".

!!! warning "Save File Chicanery"

    I've seen cases where some games have multiple `.sav` files attached to them, which confuses the owners of those games. What I can gather is that the `.sav` with the biggest file size is the correct one. When hovering over a file in FBI, the top screen should tell you the file size. If that doesn't work at the end of step 32, come back to this step and redo the same step using the other `.sav` file instead of the bigger one.

26. Press B four times to go back to your SD card's root. From there, navigate to `/roms/nds/saves/`.
27. Select `<current directory>`.
28. Select "Paste".
29. In the same folder, navigate to your save file. Select it and then select "Rename". It needs to be named the same as the game it's tied to. For example, "Pokémon White Version.nds" in `/roms/nds/` is tied to "Pokémon White Version.sav" in `/roms/nds/saves/`.
30. Press B four times to go back to FBI's main menu. From there, press Start to exit out to the Home Menu.
31. Open TwiLightMenu++.
32. Navigate to `/roms/nds/` and select your ROM. This is a check to see if your save file loaded up properly.
33. Close out of the game by pressing the Home button and then pressing A.
34. Open The Homebrew Launcher.
35. Navigate to NDS Forwarder Generator.
36. n this piece of homebrew, navigate to `/roms/nds/`.
37. Select `< Install All nds >`. Hit "Yes" to confirm.
38. Once finished, press Start to back out into The Homebrew Launcher.
39. Press the Home button to exit out into the Home Menu.

!!! warning "Title Limit"

    As stated earlier, **you can only have up to 40 DS games show up on your Home Menu at a time. You will need to play the rest through TwiLightMenu++.**

!!! note "Emulators"

    These dumps are compatible with an emulator of your choice, should you choose to export these files to use with one! More info on this later.

## Virtual Console Injects (For Retro Games)

!!! note "Personal Preferences"

    Steps 7-9 include art aspects that are personal preferences. When following along with these steps, you may use your own discretion if you like them or not.

1. Open [this Dropbox link](https://www.dropbox.com/scl/fi/hxvfg8cwrebi5gxeikokr/Debug.zip?rlkey=crc9u3oenpvqf5pwnuff166f4&e=1&dl=0) and click on the Download icon at the top right. Do not sign in if you do not want to; just click "Or continue with download only".
2. Extract the `.zip` file you just downloaded using an unarchiving application of your choice (i.e. WinRar, 7-Zip).
3. Open the `.exe` version of the program.

!!! note "Spanish?"

    If when you open the application and the text is in Spanish, click the tiny gear icon at the top below the file menu and change the language to English. From there, close and reopen the app.

4. Click "File -> New -> (Console Name) CIA".
5. Click "Project -> Load ROM".
6. The program might inform you that it was unable to download game information. This is normal. After that, it'll prompt you to search through their database for game information. Choose the right one. If you can't find it, just write any information into the program.
7. As for game icon, find an image of the game's box art on Google or SteamGridDB, and load it into the icon by choosing "Load image from file".
8. In the CIA banner section, in the dropdown menu change it to "3D Frame with Color".
9. Right below it, click "Load image from file". This time, find an image of the game's title screen on Google and load it in there.
10. Once you've finished, click "Project -> Export CIA".
11. Turn off your system.
12. Take out its SD card and insert it into your computer.
13. Drag and drop that new `.cia` file to the `/cias/` folder on your SD card.
14. Take your SD card out of your PC.
15. Insert your SD card back into your 3DS.
16. Turn your system back on.
17. Open FBI.
18. Select "SD".
19. Navigate to `cias`.
20. Select `<current directory>`.
21. Select "Install and delete all CIAs".
22. Once your game is finished installing, press B as much as you can to back out to FBI's main menu. Press Start after that.
23. Your game should now appear in the Home Menu as a "gift".

!!! warning ""

    If you just want a fresh copy of the game, stop reading here. However, if you have an save you want to put into your VC inject that you just created, continue on.

24. Turn off your system.
25. Take out its SD card and insert it into your computer.
26. Drop your save for your game somewhere on the SD card. It doesn't really matter where, but for convenience put it on the root.
27. Take your SD card out of your PC.
28. Insert your SD card back into your 3DS.
29. Turn on your system.
30. Open your new Virtual Console inject.
31. Close this game after a few seconds. This stores into memory that you were playing this Virtual Console game last.
32. Turn off your 3DS.
33. Turn your 3DS back on, but this time press and hold Start before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.
34. You should now be greeted with GodMode9. It may ask you to reset the RTC datetime offset. Do not change the provided date, just mash A until you get to the menu.
35. Navigate to `[0:] SDCARD` and select it.
36. Navigate to the location of your save file, and press Y when hovering on your save file. This copies it to the clipboard.
37. Press B as much as you need to to get back to the GodMode9 main menu.
38. Navigate to "\[S:\] SYSNAND VIRTUAL" and select it.
39. Navigate to `agbsave.bin` and select it.
40. Select "AGBSAVE Options" from the menu on the bottom screen.
41. Navigate to 'Inject GBA VC" and select it.
42. Back out as much as you can once it's injected.
43. Press Start to reboot the system.
44. Whenever you play that VC inject, from now on you can pick up where you previously left off.

### Other Ways To Play Retro Games

#### GameBoy (Color)

Just use a VC inject.

#### GameBoy Advance

!!! info "3DS Native GBA Playback"

    Everyone knows that the 3DS has backwards compatibility with DS games due to it having DSi hardware baked into it, but did you know that that DSi has GBA hardware built into it as well? This means that the DSi and the 3DS families of systems can all play GBA games, they just lacked the GBA port to do that. The 3DS does put that GBA hardware to use, however, in the form of its Virtual Console service.

**open_agb_firm** is a tool that allows for use of the 3DS' native GBA hardware to play your GBA ROM collection.

1. Open Universal Updater from your Home Menu.
2. Search for "open_agb_firm". The icon looks... very indiscriminate.
3. Download "open_agb_firm.firm".
4. Press Start to exit the Universal Updater.
5. Turn off your system.
6. Take out its SD card and insert it into your computer.
7. In a file explorer of your choice, navigate to the `/roms/` folder.
8. If a `gba` folder doesn't exist in it, create one.
9. Drag and drop any GBA ROMs you'd like into this `gba` folder. You can find those over [here](https://vimm.net/vault/GBA).
10. Take your SD card out of your PC.

!!! warning ""

    Make sure you do it safely by manually clicking eject on the file explorer, as we do not want to risk corrupting your game file!

11. Insert your SD card back into your 3DS.
12. Turn your 3DS back on, but this time press and hold Select before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.
13. You should now see the Luma menu. In the Luma menu, make sure `Enable loading external FIRMS and modules` is enabled.
14. Press Start to reboot the system.
15. Turn off your 3DS immediately afterwards.
16. Turn your 3DS back on, but this time press and hold Start before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.
17. You should now be greeted with the Luma Chainloader. Select "open_agb_firm".
18. Navigate to `/roms/gba/`.
19. Select the ROM of the game you'd like to play.
20. When you are finished playing, simply hit the Power button.

!!! info "Regarding Saves"

    If you do not have any save files you would like to import, stop reading here. Otherwise, continue.

21. Take out its SD card and insert it into your computer.
22. Drop any of your saves for your games in `/3ds/open_agb_firm/saves/`. Make sure your save file has the same name as your ROM. For example, "The Minish Cap.gba" in `/roms/gba/` is tied to "The Minish Cap.sav" in `/3ds/open_agb_firm/saves/`.
23. Take your SD card out of your PC.
24. Insert your SD card back into your 3DS.
25. Turn your 3DS back on, but this time press and hold Start before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.
26. You should now be greeted with the Luma Chainloader. Select "open_agb_firm".
27. Navigate to `/roms/gba/`.
28. Select the ROM of the game you'd like to play. Your save should now be imported properly.

#### Nintendo Entertainment System (NES)

Just use a VC inject.

#### Super Nintendo Entertainment System (SNES)

!!! info "3DS SNES Virtual Console"

    Back in the day, Nintendo said the the "Old" variant of the 3DS systems simply could not handle SNES Virtual Console titles and that that luxury was relegeated to "New" variant of the 3DS systems. Everyone knew that was a load of crap coming out of Nintendo, so homebrew developers took it upon themselves to stick it to Nintendo's face in terms of SNES emulation.

**snes_9x** is a very popular SNES emulator, that now has an updated fork for the 3DS.

1. Open Universal Updater from your Home Menu.
2. Search for "Snes9x (updated fork)". The icon looks... very corporate.
3. Download "snes9x_3ds.cia".

!!! note ""

    If you would like, you may choose to install the `.3dsx` version to launch through The Homebrew Launcher. However, for the sake of the tutorial we will be sticking with the `.cia` version.

4. Press Start to exit the Universal Updater.
5. Turn off your system.
6. Take out its SD card and insert it into your computer.
7. In a file explorer of your choice, navigate to the `/roms/` folder.
8. If a `snes` folder doesn't exist in it, create one.
9. Drag and drop any SNES ROMs you'd like into this `snes` folder. You can find those over [here](https://vimm.net/vault/SNES).
10. Take your SD card out of your PC.

!!! warning ""

    Make sure you do it safely by manually clicking eject on the file explorer, as we do not want to risk corrupting your game file!

11. Insert your SD card back into your 3DS.
12. Turn your 3DS back on.
13. Open Snes9x. It should appear as a "present" on the Home Menu.
14. Navigate to `/roms/snes/`.
15. Select the ROM of the game you'd like to play.
16. When you are finished playing, simply hit the Power button.

!!! info "Regarding Saves"

    If you do not have any save files you would like to import, stop reading here. Otherwise, continue.

17. Take out its SD card and insert it into your computer.
18. Drop any of your saves for your games in `/3ds/snes_9x/saves/`. Make sure your save file has the same name as your ROM. For example, "Final Fantasy III.sfc" in `/roms/snes/` is tied to "Final Fantasy III.srm" in `/3ds/snes_9x/saves/`.
19. Take your SD card out of your PC.
20. Insert your SD card back into your 3DS.
21. Turn your 3DS back on.
22. Open Snes9x.
23. Navigate to `/roms/snes/`.
24. Select the ROM of the game you'd like to play. Your save should now be imported properly.

#### Sony PlayStation

!!! warning "New 3DS Only!"

    Only the "New" variant of 3DS systems can emulate PlayStation games. If you do not have one of those, you're out of luck...

**RetroArch** can be used to emulate PS1 games through its *PCSX-ReARMed* core.

1. Go to [this website](https://www.retroarch.com/?page=platforms).
2. Navigate to the Download section for the "3DS / 2DS Family". Click on "Download (cia)".
3. Extract that `.7z` archive you just downloaded using an unarchiving application of your choice. (i.e. WinRar, 7-Zip)
4. Navigate to `/retroarch_cia/retroarch/cores`.
5. Delete all cores in `.cia` format in this folder except for `pcsx_rearmed_libretro.cia`. This is our PS1 emulator.
6. Go back one folder, so now our current working directory is `/retroarch_cia/retroarch/`.
7. Turn off your 3DS.
8. Take out its SD card and insert it into your computer.
9. Drag and drop the `retroarch` folder inside the `retroarch_cia` folder onto the root of your SD card.
10. Drag and drop the `retroarch_3ds.cia` file inside `/retroarch_cia/cia` insides your 3DS' `cias` folder.
11. Take your SD card out of your PC.
12. Insert your SD card back into your 3DS.
13. Turn your 3DS back on.
14. Open FBI.
15. In FBI, select "SD".
16. Navigate to your `cias` folder.
17. Select "&lt;current directory>".
18. Select "Install and delete all CIAs".
19. Once RetroArch is finished installing, press B as much as you can to back out to FBI's main menu. Press Start after that.
20. RetroArch should now appear in the Home Menu as a "gift".
21. Open RetroArch. It should try to initialize all the information with your system. Give it it's time. It will close out on its own once complete.
22. On your Home Menu, you may see that RetroArch installed an unnecessary core to your Home Menu. Ignore it for now. Open the main RetroArch app again.
23. Navigate to "Load core" and select it.
24. Navigate to `/retroarch/cores/pcsx_rearmed_libretro.cia` and select it. In the background, it will install the PS1 emulator directly to your Home Menu and then immediately send you to the PS1 emulator app.
25. Once you've loaded the emulator, close out of it by pressing the Home button and closing out of it.
26. Open the System Settings app.
27. Navigate through Data Management -> 3DS -> Software.
28. Find both the main RetroArch app and (if applicable) that random unnecessary core.
29. Exit out of the System Settings application.
30. Turn off your 3DS.
31. Take out its SD card and insert it into your computer.
32. In a file explorer of your choice, navigate to the `/roms/` folder.
33. If a `psx` folder doesn't exist in it, create one.
34. Drag and drop any PS1 ROMs you'd like into this `psx` folder. You can find those over [here](https://vimm.net/vault/PS1).
35. Take your SD card out of your PC.

!!! warning ""

    Make sure you do it safely by manually clicking eject on the file explorer, as we do not want to risk corrupting your game file!

36. Insert your SD card back into your 3DS.
37. Turn your 3DS back on.
38. Open PCSX_ReARMed.
39. Select "Load Content" and navigate to your PS1 ROM.
40. When finished playing, tap the bottom screen and navigate to close content. Then, close out of the application.

!!! info "Regarding Saves"

    If you do not have any save files you would like to import, stop reading here. Otherwise, continue.

41. Take out its SD card and insert it into your computer.
42. Drop any of your saves for your games in `/retroarch/cores/savefiles/`. Make sure your save file has the same name as your ROM. For example, "Crash Bandicoot.chd" in `/roms/psx/` is tied to "Crash Bandicoot.srm" in `/retroarch/cores/savefiles/`.
43. Take your SD card out of your PC.
44. Insert your SD card back into your 3DS.
45. Turn your 3DS back on.
46. Open PCSX_ReARMed.
47. Navigate to `/roms/psx/`.
48. Select the ROM of the game you'd like to play. Your save should now be imported properly.

#### Nintendo 64

!!! warning "New 3DS Only!"

    Only the "New" variant of 3DS systems can emulate PlayStation games. If you do not have one of those, you're out of luck...

Although it, for some reason, is advertised as doable, I've seen more reports that other people can never get it to work. And even if they can it's not in a very playable state. Therefore, I would advise against trying this.

#### VirtualBoy

Yes, it's possible. Somehow. **There is a VirtualBoy emulator for the 3DS called Red-Viper**. It has the ability to utilize the 3DS' stereoscopic 3D effects to emulate what would have been the VirtualBoy's fields of depth.

1. Open Universal Updater from your Home Menu.
2. Search for "red-viper". The icon looks... very unintuitive.
3. Download "red_viper.3dsx".
4. Press Start to exit the Universal Updater.
5. Turn off your system.
6. Take out its SD card and insert it into your computer.
7. In a file explorer of your choice, navigate to the `/roms/` folder.
8. If a `vb` folder doesn't exist in it, create one.
9. Drag and drop any VirtualBoy ROMs you'd like into this `vb` folder.

!!! info "Regarding ROMs"

    Unfortunately, our bot does not supply VirtualBoy ROMs. You must scout those for yourself until I add support for that to the bot. Sorry!

10. Take your SD card out of your PC.

!!! warning ""

    Make sure you do it safely by manually clicking eject on the file explorer, as we do not want to risk corrupting your game file!

11. Insert your SD card back into your 3DS.
12. Turn your 3DS back on.
13. Open The Homebrew Launcher.
14. Navigate to `red-viper.3dsx` and select it.
15. Navigate to `/roms/vb/`.
16. Select the ROM of the game you'd like to play.
17. When you are finished playing, simply hit the Home button and close out of the application.

## Going Online In 3DS Games

!!! info "About Online Services"

    On April 8th, 2024 5 PM PDT, Nintendo shut down the Nintendo Network. Nintendo Network was the one way the 3DS and Wii U went online in games. However, Pretendo is a WIP open source replacement of Nintendo Network functionality. With Pretendo, you can go online with your 3DS post-Nintendo Network shutdown, along with gaining access a new (and improved) version of Miiverse among other cool things.

!!! warning "Your Friends List"

    Setting up Pretendo does **NOT** carry over your Friends List. Pretendo has stated that while they think a potential NNID -> PNID account transfer is possible, it is outside the scope of the project on top of potential lawsuits from Nintendo that may arise from handling NNID data from them.

1. Open Universal Updater from your Home Menu.
2. Search for "Nimbus". The icon looks like a purple lowercase N.
3. You can choose whether you want to install the `.3dsx` version or the `.cia` version. Keep in mind, the `.3dsx` version is meant to be launched through The Homebrew Launcher, while the `.cia` version is meant to be launched through the Home Menu.

!!! note ""

    For the sake of this guide, we will be installing the `.3dsx` version. Though, instructions shouldn't vary by much if you choose to go the other route. Only by means of how to access the Nimbus application.

4. Press Start to exit out of the Universal Updater once it's finished installing.
5. Turn off your system.
6. Turn your 3DS back on, but this time press and hold Select before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.
7. You should now see the Luma menu. In the Luma menu, make sure both `Enable loading external FIRMS and modules` and `Enable game patching` are enabled.
8. Press Start to reboot the system.
9. Open The Homebrew Launcher.
10. Navigate to Nimbus and select it.
11. Select "Pretendo" on the bottom screen.
12. Once the system finishes reloading, press the Home button to suspend The Homebrew Launcher. Close out of it.
13. Put your 3DS aside for now, but leave it on. Ideally, you can put it in Sleep Mode.
14. Go to [Pretendo's website](https://pretendo.network/) on a computer. Set up an account with them (A "PNID").

!!! danger "About Account Names"

    You may **NOT** use the same account name as your old NNID! For example, if I had registered an NNID with Nintendo with the ID name of "JohnDoe", you can create a PNID with the ID name of "JohnDoe" but your 3DS will not be able to sign into that PNID. As such, try to find a new ID name for your PNID. (i.e. "JohnDoe" uses "DohnJoe" instead).

15. Once you've set up your account with them, open the System Settings application on your 3DS.
16. Open the "Nintendo Network ID Settings" applet.

!!! note "Potential Confusion"

    Even if we are connected to Pretendo's servers, there is no reference to a "Pretendo" in the 3DS' UI. Therefore, please just remember that you are connected to Pretendo servers when trying to access "Nintendo" Network stuff.

17. Log into your PNID as if it were an NNID. Choose "Link existing ID" when signing in. Remember to select the option to use the Mii that's registered with your system as the face of your PNID instead of the default one.
18. Once you're done with that, you should immediately get booted back into the System Settings application. Just close out of it.
19. You're done! This is only a one time set up!

!!! note ""

    If you wish to verify that you are finished with the set up process, try opening the Friends List applet. If you are able to go online and you have an empty list of friends, you are good to go. If not, there are people who can try helping in [their Discord server](https://invite.gg/pretendo).

## Going Online In DS Games

!!! info "About Wiimmfi"

    Nintendo Wi-Fi Connection (Nintendo WFC) was a service that the DS and the Wii used to go connect your games online. It was shut down on May 20th, 2014, due to the outsourced company that was hosting Nintendo's servers being shut down. However, over the course of the years afterwards, dedicated fans were able to revive these servers for Wii and DS games through Wiimmfi! In some cases, it can be as easy as simply entering a DNS code to route your network information to!

!!! info "What Kind Of Game Do You Have?"

    The original DS from 2004 could only connect to Wi-Fi networks with either no security whatsoever that don't have a web based sign in (something like an airport's or a Starbucks Wi-Fi), or ones using the outdated WEP security protocol, which had been cracked by 2001 and was officially deprecated in favor of WPA2 in 2004. The DSi offered enhanced Wi-Fi capabilities, including support for WPA and WPA2 security protocols. This is important for games like the Gen 5 Pokémon games, which are 'DSi Enhanced' and can take advantage of these newer security standards when played on a DSi or 3DS. Thus, it's important to note whether the game you want to go online in is DSi Enhanced or not. [This list](https://gamicus.fandom.com/wiki/List_of_DSi_enhanced_video_games) may tell you. Chances are the game you want to play isn't, however.

### DSi Enhanced Games

1. Open the System Settings app on your 3DS' Home Menu.
2. Select "Internet Settings".
3. Select "Connection Settings".
4. Select the number associated with your Wi-Fi connection. For example, "Connection 1".
5. Select "Change Settings".
6. Tap the right arrow on the right of the bottom screen just once.
7. Select "DNS".
8. Select "No" under the section for "Auto-Obtain DNS".
9. Select "Detailed Setup".
10. Make sure the Primary and Secondary DNS numbers are the same as the ones listed [here](https://wiilink.ca/guide/wii/#connecting-to-dns). If not, configure that. Don't get thrown off by the fact that WiiLink's guide tells you how to set up this DNS with a Wii, as this DNS also works with the DS and should you have been following along this whole time you wouldn't need to follow their steps. Just find and use the DNS numbers on this page.
11. Select "OK".
12. Select "Save" then "OK".
13. It will ask you to do a connection test. This doesn't really matter, but to be on the safe side, select "Test".
14. Once your connection test is successful, back out 3 times by tapping "Back" on the bottom screen thrice.
15. Press X to close out of the System Settings app.
16. Load up your DSi Enhanced game. It may be either through a cartridge or through a dump that you had situated on your 3DS.

### Non-DSi Enhanced Games

!!! note "The Modern Day"

    Chances are that nowadays, your Wi-Fi router at home does not support WEP security. Additionally, it is also common practice for your home internet to have a password attached to it, meaning it has to fall under some other security protocol. As of late 2024, that protocol will likely be WPA3, which obviously is not WEP. This leaves us with a few options...

##### A Password-less Hotspot From An Android Phone

!!! warning ""Why Not iPhones As Well"?"

    This is simply because of software restrictions that Apple has set on their iOS. iOS will simply not allow you to create a password-less hotspot from your phone; an iPhone's hotspot must have some form of encryption to it. By modern standards, the encryption that iOS hotspots are allowed to use are not WEP, which means they cannot be detected by the Nintendo DS.

1. Open the hotspot settings on your Android phone. Instructions on how to do this varies between Android versions and the manufacturers of your phone, so you may need to look up how to do that for your make and model.
2. Configure your hotspot to however you like (i.e. the name/SSID of your hotspot), just make sure that the security parameter is set to "None" and that the speed/bandwidth is set to 2.4 GHz. This means your hotspot will have no password attached to it and can be read at a frequency that your 3DS can read.
3. Save whatever configurations you made.
4. Turn on your hotspot and put your Android phone aside for now. Leave it on the hotspot menu however.
5. Turn on your 3DS.
6. Open the System Settings app on your 3DS' Home Menu.
7. Select "Internet Settings".
8. Select "Connection Settings".
9. Select "Nintendo DS Connections" and then "OK". This will bring you to the DS Wi-Fi settings in built into the 3DS' DSi firmware after a quick automatic reboot.
10. Select "Nintendo Wi-Fi Connection Settings".
11. Select an empty connection number.
12. Select "Manual Setup".
13. Enter the SSID of your hotspot into the box for SSID on your "DS".
14. Select "No" under the section for "Auto-Obtain DNS".
15. Make sure the Primary and Secondary DNS numbers are the same as the ones listed [here](https://wiilink.ca/guide/wii/#connecting-to-dns). If not, configure that. Don't get thrown off by the fact that WiiLink's guide tells you how to set up this DNS with a Wii, as this DNS also works with the DS and should you have been following along this whole time you wouldn't need to follow their steps. Just find and use the DNS numbers on this page.
16. Select "Save Settings".
17. Select the number of the connection you just configured.
18. Select "Test Connection".
19. Once your connection is successful, press the B button 4 times to have your system automatically reboot back into the 3DS' Connection Settings.
20. Select "Back".
21. Press X to close out of the System Settings application.
22. Open a Non-DSi Enhanced Game of your choice. It may be either through a cartridge or through a dump that you had situated on your 3DS.

!!! warning "Data Usage"

    This method will consume a LOT of your monthly allowance for cellular data, if you have such an allowance. Please be cautious with how long you are going online with your game if this is the case. Alternatively, you can also follow the second or third options listed right below.

#### Using The melonDS Emulator

1. Either dump your Non-DSi Enhanced DS game, or scavenge for its ROM online. Instructions for both methods are listed above. If it is already backed up, ignore this step.
2. Turn off your system.
3. Take out its SD card and insert it into your computer.
4. In our Discord server, in any of the command's permitted channels, enter `!w emulation ds`.
5. Follow step 1 and steps 4-6 on the guide provided. Just remember, when following step 4 set your "Save files path" to `/roms/nds/saves` that is on your SD card. This way, it will directly read and write from the save you had extracted and placed properly on your system. Also, when following step 6 locate to your game's ROM in `/roms/nds`.
6. In your game, enter the Wi-Fi settings. For example, in "Mario Kart DS" this can be done by selecting "Nintendo WFC" in the game's title screen and then by selecting "Nintendo WFC Settings".
7. Select "Nintendo Wi-Fi Connection Settings".
8. Select Connection 1. You should see that the SSID is "melonAP".
9. Select "No" under the section for "Auto-Obtain DNS".
10. Make sure the Primary and Secondary DNS numbers are the same as the ones listed [here](https://wiilink.ca/guide/wii/#connecting-to-dns). If not, configure that. Don't get thrown off by the fact that WiiLink's guide tells you how to set up this DNS with a Wii, as this DNS also works with the DS and should you have been following along this whole time you wouldn't need to follow their steps. Just find and use the DNS numbers on this page.
11. Select "Save Settings".
12. Select the number of the connection you just configured.
13. Select "Test Connection".
14. Once your connection is successful, press the B button thrice to have your system automatically go back to your game.
15. Once finished with the game's online features and/or are finished playing the game, select "System -> Stop" from the menu at the top.
16. Close out of melonDS.
17. Take your SD card out of your PC.
18. Insert your SD card back into your 3DS.

!!! warning "Locking Down"

    This method requires the use of a computer with a (micro)SD card slot to insert your card into. Additionally, you would then be tied to using your game with melonDS to go online, as Nintendo WFC configurations from back in the day treated a game and a console as one tied-together unit. If this doesn't seem like something you'd want to do, but have a spare bit of money on you, you could try setting up a network hotspot in your house following the steps listed below.

#### Using A Portable Router

You can buy a cheap "travel" router from tech junk stores or the internet for relatively cheap. [The router I have](https://www.tp-link.com/us/home-networking/wifi-router/tl-wr802n/) fits in my pocket, and is so small people aren't even going to notice it's there unless they *really* looked. You may even forget you have this router once this setup is done! (Please don't.).

!!! warning "Assumptions Made!"

    **This guide assumes that you're using the router I linked above!** This is just so that there is parity with instructions and your setup process.

!!! note "Keep Track"

    Remember, if at any point during the set up of this router (steps 1-36) you ever get disconnected from the router's network that you need to reconnect it in order to continue on to the next step.

1. Buy the router I linked above.
2. Wait however long for that to arrive at your door.
3. Unbox the router. You will get a sticker with the default SSID and password configuration printed on it. Save this for later.
4. The router comes with an included USB to microUSB cable and a power brick. Plug in your router to an outlet accordingly.
5. Wait about 30 seconds to 1 minute to let the router configure itself.
6. On your PC, connect to the default Wi-Fi configuration from that sticker earlier from your PC's Wi-Fi settings.
7. On your PC's web browser, go to `http://192.168.0.1/`. This is the webpage for your router's configuration settings. Your browser may complain that you're accessing an unsecure site (as we are accessing a `http` site versus a `https` site, so make sure you work around this. This process varies depending on browser, so I cannot help you.
8. It will prompt you to set a password. This password is to make sure that no one except for whoever knows it can configure your router, thus, **make sure this password is secure!** You will then be sent to the Quick Setup section.
9. Click on "Next".
10. Click on the box for "WISP" mode, and then click Next.
11. Click on the box for "Dynamic IP (Most common option)" mode, and then click Next.
12. The router will scan for all nearby Access Points (APs). Click on "Connect" in the row and column for your desired Wi-Fi network. You may see several options for the same network. Choose the row which has the highest "Signal strength".
13. In the box for "Wireless password", enter the password for the Wi-Fi network you selected earlier.
14. In the box for "Local Network SSID", enter a new SSID if you wish. This is the name of the Wi-Fi network you see, so if you don't want to see the default name change it to something more meaningful to you.
15. Click on the box for "Disable Wireless Security". **THIS IS IMPORTANT!** We will soon be working to make sure very little other people can connect to this network, if they can even find it, so don't freak out quite yet. Your DS-mode 3DS and your PC will only be able to connect to this open network by the end of this set up.
16. Click on the box that says "Next".
17. The screen will show your configuration just for you to double check. Click on "Finish".
18. The router will now restart. Wait for this progress bar to finish, and then wait another 30 seconds to 1 minute. You will need to reconnect to the new SSID you set earlier.
19. Once done, in the Wireless tab of the configuration page, click on the subsection for "Basic settings".
20. Uncheck the box for "Enable SSID Broadcast".
21. Click on "Save".
22. In the Wireless tab of the configuration page, click on the subsection for "Wireless MAC Filtering".
23. Get your PC's MAC Address. This is necessary so that if you ever need to make changes to the router configuration, your PC can be a base for that. On Windows, read [this guide](https://kb.ucdavis.edu/?id=00209) to figure out how. On MacOS or Linux, open a terminal of choice and enter `ifconfig en0 | grep ether`.
24. Click on the "Add New" button on the router configuration page.
25. Enter the MAC Address you got earlier into the respective textbox. Capitalize any letters you see in that address.
26. In the textbox for description, make a quick one-liner to let you know this is your PC. For example, "My PC".
27. Click on "Save".
28. Click on the "Add New" button again.
29. In the textbox for description, make a quick one-liner to let you know this is your 3DS. For example, "My 3DS".
30. Turn on your 3DS.
31. Open the System Settings application.
32. Navigate through Internet Settings -> Other Information -> Confirm MAC Address. You should then be able to see your 3DS' MAC address.
33. In the textbox for the MAC Address, enter the MAC Address you see on your 3DS' touch screen. Replace any dashes (-) with colons (:).
34. Click on "Save".
35. Click on the box for "Allow the stations specified by any enabled entries in the list to access.".
36. Finally, you can click on the giant "Enable" button at the top of this page.
37. We're done with all network configurations. Close out of the router configuration settings tab in your browser. We won't be needing a PC anymore.
38. On your 3DS, tap on "Back" twice.
39. Tap on "Nintendo DS Connections".
40. Tap on "OK". This will reboot the system into DS mode.

!!! warning "Holding Start or Select?"

    If you didn't already know, when booting into DS mode for whatever reason (most times, loading a DS game), you can hold the Start or Select button while the DS software is booting so that it displays at a 4:3 resolution that the original DS used instead of a 5:3 resolution like the 3DS uses when playing DS games. This can be helpful because the 5:3 resolution can really wash out some colors and stretch the image a bit too much. Accessing DS Wi-Fi settings like this is no exception to this, but there's a catch. Due to the nature of this set up you can connect to a network like this without the need to mod your 3DS, but since this megathread is about things you can do with a modded system this is made under the assumption that your 3DS is modded. In which case, holding Start in this segment will open GodMode9 (or the Luma3DS chainloader if you have open_agb_firm installed as well), whereas holding Select in this segment will open the Luma3DS menu. Pressing Start afterward will *not* reboot you back into 3DS mode, but into DS mode. So in case you get thrown off by this, don't be. :)

41. Select "Nintendo Wi-Fi" Connection Settings.
42. On any of the three available connections, select the box that says "None" for that open connection.
43. Navigate to "Manual Setup" and select it.
44. Select "Edit" in the SSID section.
45. Enter the SSID you created earlier and then select OK. Confirm it from there.
46. Navigate to the "Auto-obtain DNS" section and select "No".
47. Make sure the Primary and Secondary DNS numbers are the same as the ones listed [here](https://wiilink.ca/guide/wii/#connecting-to-dns). If not, configure that. Don't get thrown off by the fact that WiiLink's guide tells you how to set up this DNS with a Wii, as this DNS also works with the DS and should you have been following along this whole time you wouldn't need to follow their steps. Just find and use the DNS numbers on this page.
48. Select "Save Settings".
49. Select the number of the connection you just configured.
50. Select "Test Connection".
51. Once your connection is successful, press the B button thrice to have your system automatically go back to the 3DS Internet Settings.
52. Tap on "Back".
53. Tap on "Close" or press X.
54. Open your Non-DSi Enhanced game.
55. Happy netplay!

From now on, your 3DS will automatically connect to this small router when playing a Non-DSi Enhanced game online. No need to reconfigure your router again afterwards. Just let it sit.

## Using Cheats

!!! danger "Be A Good Samaritan!"

    Please do **NOT** use game-breaking cheats online in your games! Not only can you get banned from using certain online services, it also ruins the fun for other people playing with you!

### 3DS Games

1. Open the game of choice just for a quick second.
2. Close your game after a few seconds or so by pressing the Home button and closing the software.
3. Open Checkpoint.
4. Find your game in the app. Select it.
5. Using the touchscreen, select "Cheats" below the "Restore" option.
6. Select the cheats you'd like to enable from the list.
7. Press B once finished selecting your cheats.
8. Press A to save.
9. Press Start to exit Checkpoint.
10. Open your game of choice.
11. Press L + D-Pad Down + Select.
12. Navigate to "Cheats..." and select it
13. Select the cheats you want to use.
14. Go wild!

### DS Games

!!! warning "Assumption Made!"

    **This guide assumes that you have dumped a ROM of a game or have it set up through TwiLight Menu++**! If you haven't done that already, please do so! Instructions are above.

!!! info "Regarding The Cheats Database"

    If you already have this file installed, skip to step 5.

1. Open the Universal Updater.
2. Search for "NDS(i) Cheat Databases". The logo looks like the Action Replay DS logo.
3. Download the `[twlmenu] usrcheat.dat` file.
4. Press Start to exit out of the Universal Updater.
5. Open TwiLightMenu++ from the Home Menu.
6. Navigate to a game of your choice.
7. Press Y and then X to open the cheats menu.
8. Select whatever cheats you want.
9. Press X to save the cheat information.
10. Press B.
11. Press A to launch your game.
12. Use your cheats!

!!! note "Regarding Forwarded Games"

    If your game is forwarded to the Home Menu, these same cheats will still apply!

## Installing Unofficial Themes

1. On your computer, open [this website](https://themeplaza.art/themes).
2. Search for a general topic for a theme you'd like.
3. Hover your mouse over the picture of a theme you like, and a QR code should appear on screen. Keep your mouse still.
4. Turn on your 3DS and open the Anemone app.
5. Press R for "Scan QR Code".
6. With your 3DS' exterior cameras, scan the QR code that shows over your mouse.
7. After it is finished installing, navigate to your new theme.
8. While holding the A button, press and hold Up on the D-pad. Release your hold on the A button while still holding down Up on the D-pad.
9. Once the theme has finished loading, press Start and turn off the system.
10. Upon reboot, your new theme should be applied to your system.

### (Optional) Mix-Matching Music

You can have music from other themes play on an entirely different theme if you'd like! The process isn't all that much harder either, you just need 2 themes downloaded into Anemone.

1. Open Anemone on your 3DS.
2. Navigate to the theme you'd want displayed. We'll call it the presentor theme.
3. While holding the A button, press and hold Up on the D-pad. Release your hold on the A button while still holding down Up on the D-pad.
4. Once the presentor has finishing loading, press Start and turn off the system.
5. Upon reboot, the presentor should be displaying but we're not done yet. Open Anemone.
6. Navigate to the theme you'd want the music of to be playing. We'll call it the donor theme.
7. While holding the A button, press and hold Left on the D-pad. Release your hold on the A button while still holding down Left on the D-pad.
8. Once the donor has finished loading, press Start and turn off the system.
9. Upon reboot, the presentor should be displaying while the donor's theme music is playing.

### (Optional) Shuffling Themes

You can have it so that whenever you enter the Home Menu of your 3DS, a different theme shows up. This can be through a variety of methods, including but not limited to entering/exiting Sleep Mode or suspending games/apps. Make sure to already have a few themes downloaded!

1. Open Anemone on your 3DS.
2. Scroll through the list of themes you have downloaded. If you want that theme to be included in the shuffle press B when hovering over the theme.
3. When finished with deciding what themes you want to shuffle, hold down on the A button. While holding the A button, press and hold Down on the D-pad. Release your hold on the A button while still holding down Down on the D-pad.
4. Once the themes have finished loading, press Start and turn off the system.
5. Upon reboot, the shuffle should be activated.

## Installing Custom Badges

1. Open Universal Updater from your Home Menu.
2. Search for "GYTB". What stands out to me in its icon is a pixel art ladybug.
3. Download the `gytb.cia` file.

!!! warning ""

    Looking through the program's GitHub repository, it seems that the `.3dsx` homebrew version is meant for 3DS systems that were hacked through a VERY outdated method. Therefore, please avoid it as it by extension is also outdated.

!!! note "Important"

    If you had already played Nintendo Badge Arcade way back when, skip steps 4-6. It is imperative if you know if you did or didn't, but that's easily checked by if your system allows you to select badges from the Home Menu. Alternatively, you'll know if you have by the `badges` folder on the root of your SD card is already populated by files for badges.

4. Press Start to exit out of the Universal Updater.
5. Go to hShop/3hs (whichever method you prefer) and download Nintendo Badge Arcade.
6. Play through its tutorial.
7. Once done, exit out of the application by pressing the Home button and closing out of the app.

!!! note "Important"

    By this point, everyone reading this guide should have now used Nintendo Badge Arcade at least once. However, there may be a subsection of you that have used it in the past and deleted it. If you are one of those people, skip steps 8-11.

8. Open the System Settings application.
9. Navigate through Data Management -> 3DS -> Software.
10. Find Nintendo Badge Arcade and delete it.
11. Exit out of the System Settings application.
12. Run GYTB from your Home Menu. It should appear as a "gift".
13. GYTB should now register the custom badges it came with. Once that's done, press any button to exit the application.
14. Turn off your system.
15. Take out your SD card and insert it into your computer.
16. Go to [this website](https://themeplaza.art/badges).
17. Search for and/or find a sheet of badges you'd like. Click on it.
    - I am not exactly sure why it shows a QR code when hovering over a sheet, but my guess is that it's because this is the same website that manages themes.
18. Click on "Download" to download a ZIP archive of all the badges in that sheet.
19. Extract that ZIP archive using an unarchiving application of your choice. (i.e. WinRar, 7-Zip)
20. Take all the `.png` files from the extraction and drag them into the `badges` folder of your 3DS' SD card.
21. Eject your SD card and insert it back into your 3DS.
22. Turn on your 3DS.
23. Open the GYTB application from the Home Menu.
24. GYTB will now re-register its own custom badges on top of the ones you inserted into the badges folder.

!!! info ""

    If you choose to add more badges after doing this once, GYTB is a one-time setup, meaning that to get more badges **you have to start at step 14 the next time**.

## Mods (Generally Speaking)

1. Go to [GameBanana](https://gamebanana.com/), as they tend to have a lot of mods/texture packs for your game of choice.
2. Once you find the mod of your choice, make sure you click on it to see whether or not the developer of it said that it works on a real 3DS. a lot of the time, the mods they make may only work on Citra or other 3DS emulators. Another quick way to check if it only works on Citra is if the texture pack you downloaded is comprised of image files (such as `.png`), which don't work on a 3DS.
3. Turn on your system.
4. Open FBI.
5. Select "Titles".
6. Navigate to your game of choice, and note down the title ID the top screen should display. It will be important for later.
7. Press B to get to FBI's main menu.
8. Press Start to exit out of FBI.
9. Turn off your system.
10. Take out its SD card and insert it into your computer.
11. In a file explorer of your choice, navigate to the `/luma/` folder.
12. If a `titles` folder doesn't exist in it, create one.
13. Inside the new `titles` folder, create a folder titled with the title ID you noted down somewhere.
14. Inside the title id folder, create a folder called `RomFS`.
15. Place your mod files in this new `RomFS` folder.
16. Take your SD card out of your PC.
17. Insert your SD card back into your 3DS.
18. Turn your 3DS back on, but this time press and hold Select before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.
19. You should now see the Luma menu. In the Luma menu, make sure `Enable game patching` is enabled.
20. Press Start to reboot the system.
21. Whenever you boot up your game of choice, from now on it should be modded.

### Majora's Mask 3D Restoration Mod

1. Go to [this website](https://restoration.zora.re/).
2. Click the "Download for 3DS or Citra" button.
3. Click the "Download Project Restoration (the latest version)" button.
4. Use an unarchiving application of your choice (i.e. WinRar, 7-Zip) to extract the `.7z` file that you downloaded.
5. Turn on your system.
6. Open FBI.
7. Select "Titles".
8. Navigate to *Majora's Mask 3D*, and note down the title ID the top screen should display. It will be important for later.
9. Press B to get to FBI's main menu.
10. Press Start to exit out of FBI.
11. Turn off your system.
12. Take out its SD card and insert it into your computer.
13. In a file explorer of your choice, navigate to the `/luma/` folder.
14. If a `titles` folder doesn't exist in it, create one.
15. Inside the new `titles` folder, create a folder titled with the title ID you noted down somewhere.
16. When you extracted the `.7z` file, there should have been 3 folders called `v100`, `v101`, and `v110`. Start off with the `3ds` folder inside the `v100` folder. drag the `code.bps` and `exheader.bin` files from that folder and drop them in the title ID folder you just made.

!!! note ""

    **OPTIONAL**: If you would like, you can instead drag the `code_faster_aim.bps` file along with the `exheader.bin` file and drop that in the title ID folder. When it is dropped, however, make sure to rename it to `code.bps` within your SD card. This file will give you slightly faster aim when aiming with the Circle Pad.

!!! warning "Trial And Error"

    For this next few steps, you may see yourself repeatedly coming back to step 16 but instead of `/v100/3ds/` you would be using `/v101/3ds/` or `/v110/3ds/`. It's unfortunately just how it is. Some systems react to things differently.

17. Take your SD card out of your PC.
18. Insert your SD card back into your 3DS.
19. Turn your 3DS back on, but this time press and hold Select before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.
20. You should now see the Luma menu. In the Luma menu, make sure `Enable game patching` is enabled.
21. Press Start to reboot the system.
22. Whenever you boot up *MM3D*, you will know that the game is modded if there's a sound that plays immediately after opening the application.

!!! note ""

    If you do not hear that sound, look through the "Trial And Error" warning and start from there.

## Streaming 3DS Games To Azahar Emulator

!!! info "What This Means"

    Your 3DS will store information about the games you play to its internal storage. An emulator acts as a middleman, making your computer behave like the old console so that the games run as if you were playing them on the original system. There should be no reason why an emulator cannot access storage data the same way an actual 3DS can, since an emulator is already trying to fool your computer into thinking it is a 3DS. This is where Artic Base comes in. It allows you to send game information from your 3DS over the internet to your computer for it to be used in an emulator, which in this case is Azahar, as it is currently the best 3DS emulator for PCs and Android devices.

!!! warning "Ups And Downs"

    There are many up sides to using Artic Base. You can essentially use your 3DS like a Nintendo Switch in the sense that you can play handheld at a lower fidelity and performance, and then use Artic Base to connect to your computer to play at a better fidelity and performance right where you left off. Or vice versa. The big downside to this, however, is that when connected to an emulator through Artic Base, loading times for games can range from 2-5 times longer. Additionally, if you have certain mods installed on your 3DS they may or may not work. This can only be checked through trial and error, since I can't seem to find good documentation on this issue.

1. Open Universal Updater from your Home Menu.
2. Search for "Artic Base". The icon looks like an igloo.
3. You can choose whether you want to install the `.3dsx` version or the `.cia` version. Keep in mind, the `.3dsx` version is meant to be launched through The Homebrew Launcher, while the `.cia` version is meant to be launched through the Home Menu.

!!! note ""

    For the sake of this guide, we will be installing the `.3dsx` version. Though, instructions shouldn't vary by much if you choose to go the other route. Only by means of how to access the Artic Base Server application.

4. Press Start to exit out of the Universal Updater once it's finished installing.
5. Go to your PC if you aren't there already while reading this.
6. Download the latest release of Azahar [here](https://azahar-emu.org/pages/download/). If on Windows, the differences between MSVC and MSYS2 aren't something the average person would understand, so just trust me when I say download the MSVC version.
7. Once Azahar is downloaded, extract the archive the download should've come in. You should see a folder emerge from that archive.
8. Inside this folder, you should see an Azahar application. The other stuff is irrelevant. Just drag and drop that application binary to wherever you see fit. Note that when I say "binary", this can mean a `.exe` file or a `.app` file or a `.AppImage` file depending on your operating system.
9. Download the `.3dsx` file from the latest release of [this GitHub repository](https://github.com/azahar-emu/ArticSetupTool/releases/latest).
10. Turn off your 3DS.
11. Take out its SD card and insert it into your computer.
12. Drag and drop that `.3dsx` file you just downloaded into your `3ds` folder.
13. Take your SD card out of your PC.

!!! warning ""

    Make sure you do it safely by manually clicking eject on the file explorer, as we do not want to risk corrupting your files!

14. Turn on your 3DS
15. Open The Homebrew Launcher.
16. Navigate to Azahar Artic Setup Tool and select it.
17. Press A and wait for a few seconds. The top screen will now display an IP address with a port next to it. (Format: [XXX.XXX.XXX.XXX](http://xxx.xxx.xxx.xxx/):PORT).
18. Open the Azahar application binary. Set it up as you'd like. If you need help with that feel free to ask me in our Discord server.
19. Click on "File > Set Up System Files..."
20. Enter in that IP address you see on your top screen.
21. Press "OK". Give it a minute, as Azahar is transferring information from your console to your PC over the internet.

!!! note "In Case Of Curiousity"

    The information being transferred here is actually the unique files your 3DS stores within its NAND that identify it among others. Essentially, what Nintendo would think we're doing here is cloning your 3DS. Pretty neat! Normally, you'd need something like a System Transfer to use the same credentials and whatnot for your NNID, but since those identifiers are now doubled and in 2 separate places your 3DS has now effectively been cloned. Note that your Friend Code and your friends list would not carry over.

22. You will eventually see the System Settings application open. This is normal. It will prompt you to update your system version; please do so.
23. Wait for this update to finish. Once finished you should be booted back into the main Azahar UI.
24. On your 3DS, press Start. You will be booted back into the Home Menu.
25. Re-open The Homebrew Launcher.
26. Navigate to Artic Base and select it.
27. Press A and wait a few seconds.
28. Once the system finishes reloading, press the Home button to suspend The Homebrew Launcher. Close out of it.
29. Open a 3DS game of your choice. You should see that as the Nintendo 3DS splash screen shows up, a small flash of blue should appear on screen.
30. The top screen will now display an IP address with a port next to it. (Format: [XXX.XXX.XXX.XXX](http://xxx.xxx.xxx.xxx/):PORT).
31. Back on your PC, click on File -> Connect to Artic Base.
32. Enter your IP address and port number exactly as you see it on your 3DS' top screen into the emulator's textbox.
33. Give it some time, and your game will now be streamed to your emulator. To exit out, just press Start on your 3DS.

"This is kind of tedious!" you might say. And you'd be right. Which is why once you've set up everything and if you'd like to stream a game to Azahar again, you can start from step 25.

## FTPD (File Transfer Over Internet)

!!! info "What Is FTPD?"

    The "New" variant of 3DS systems can wirelessly transfer files between a Windows computer running Windows 7 or later from the System Settings application -> Data Management -> microSD Management. Once you start up the instance following the on screen prompts, you could access your 3DS' files from the Windows file explorer in its Network section. But what if you don't have a "New" variant system and/or don't have a Windows device, yet you want to wirelessly transfer files between your computer and 3DS? This is where FTPD comes in. It allows you to do exactly that.

!!! warning "Take Into Consideration"

    From my understanding, as of 1/21/2025 or maybe some time before as well, the FTPD application now comes bundled with the process of modding your system. If you're modding your system since then, you can skip steps 1-4.

1. Open Universal Updater from your Home Menu.
2. Search for "FTPD". The icon looks like a black square that says "FTPD" in giant green text.
3. You can choose whether you want to install the `.3dsx` version or the `.cia` version. Keep in mind, the `.3dsx` version is meant to be launched through The Homebrew Launcher, while the `.cia` version is meant to be launched through the Home Menu.

!!! note ""

    For the sake of this guide, we will be installing the `.cia` version. Though, instructions shouldn't vary by much if you choose to go the other route. Only by means of how to access the FTPD application.

4. Once it's finished installing, press Start to close out of the Universal Updater.
5. Open the FTPD application from your Home Menu.
6. The top screen should have an IP address and port number at the top. This will be in the format of [XXX.XXX.XXX.XXX](http://xxx.xxx.xxx.xxx/):(PORT). Keep note of it.
7. Put your 3DS aside for now but leave it on with the screens opened.

!!! note "Divergence"

    This section will now divide into 2 sections for instructions depending on your operating sytem.

### For Windows/MacOS

8. Go to [this website](https://cyberduck.io/download/).
9. Download for your operating system.
10. On Windows, run through the installer for the program and then open Cyberduck. On MacOS, unarchive the `.zip` file you downloaded using an unarchiver of your choice (the MacOS default one works just fine), drag and drop `Cyberduck.app` into your Applications pin in Finder, go to the Applications pin, right click on `Cyberduck.app`, select "Open", then confirm that you want to open the application.
11. In Cyberduck, click "Open Connection" at the top.
12. At the dropdown on the top, make sure "FTP (File Transfer Protocol)" is selected.
13. In the text box for "Server", enter the IP address on your 3DS.
14. In the box for "Port", enter the port number on your 3DS.
15. Cyberduck will now connect to your 3DS' files directly. Open a window in your file explorer from here.
16. Use both Cyberduck and the window you just opened to do whatever dragging and dropping of files in and out of your SD card that you need to do. Note that because we are wirelessly transferring files here, files may take longer to transfer in and out of your system.
17. Once finished, close out of Cyberduck. It may prompt you to pay money, in which case just click "Later". Cyberduck will always be free to you, and you paying money is only to support the developers.
18. Back on your 3DS, press Start to exit out of FTPD.

### For Linux

8. In your file explorer (in my case, Dolphin on my Steam Deck), right click on the file path at the top and make sure "Show file path" is selected.
9. Click on the file path to open a textbox displaying the full file path.
10. Press Ctrl+A to highlight the entire thing and then Backspace to delete it all.
11. Enter the following into the file path bar: `ftp://(the ip address):(the port number)`. You should then almost instantly be able to access the files on your SD card.
12. Open a new tab or window of Dolphin. Use both of these tabs/windows to do whatever dragging and dropping of files in and out of your SD card that you need to do. Note that because we are wirelessly transferring files here, files may take longer to transfer in and out of your system.
13. Once finished, close out of the tab/window that contains your 3DS' files and the other tab/window containing files on your Linux computer.
14. Back on your 3DS, press Start to exit out of FTPD.

## Using External Controllers

!!! warning "Assumptions Made!"

    - **This guide assumes that you have a Windows PC**! The software that you will need is Windows dependant, using .dll and .exe files. I'm not sure if you can run these programs under a compatability layer like Proton on Linux or Whisky on MacOS, but for the sake of working 100% of the time please use a Windows PC for this.
    - **This guide assumes that you are going to be using an Xbox controller**! This works with a tool called XInput, which comes with Xbox controllers. If you do not have an Xbox controller, you can use a tool like [x360ce](https://github.com/x360ce/x360ce/releases/) to remap your buttons accordingly, or open the software outlined below as a Non-Steam Game to utilize Steam Input. This guide will not go over either of these processes.

!!! info "You Can Use One?"

    Luma3DS allows for interoperability between it and a 3rd-party application called InputRedirection. This process will allow you to connect your 3DS to your PC over your local internet connection, at which point you can connect your controller to your PC and operate your 3DS from there. You may then use your external controller for use on your 3DS. This can be for accessibility reasons (ie. if your hands cramp up after long sessions of play), or for better use with games that have wonkier control schemes (ie. Smash Bros, Kid Icarus Uprising, MH4U/G).

1. Connect your controller to your PC. This can be done either via Bluetooth or through a wired connection.
2. Download the latest `.zip` file of the required application from [here](https://github.com/TuxSH/InputRedirectionClient-Qt/releases/). You are looking for the `.zip` file that is NOT the source code; look for the keyword "QT" in the`.zip` file you would download.
3. Extract this `.zip` file to a location of your choice on your PC.
4. Open `InputRedirectionClient-QT.exe`.
5. Turn on your 3DS.
6. Once it boots up, press L + D-Pad Down + Select.
7. Navigate to "Miscellaneous options..." and select it.
8. Navigate to "Start InputRedirection" and select it.
9. You will see that on the top right corner of your touch screen, there will be an IP address. Type this into the box for the IP address in the `.exe` file you opened in step 4.
10. If you do not like how some of the controls are laid out, you can remap them in the "Settings" of the `.exe` application.
11. You are free to game on your controller!

If you'd like to stop InputRedirection when finished playing, simply repeat steps 6-8.

## Patching DS(i) Firmware

!!! info "How "DS(i) Mode" Works"

    The layman approach of explaining how the 3DS is able to play DS games is that "it contains DS hardware inside of it". This is mostly true, but not entirely. While it's not literally a DS motherboard soldered inside, the 3DS does contain hardware that's capable of natively running DS software. Specifically, it includes processors that are compatible with the ARM9 and ARM7 chips used in the original DS. When you boot a DS game, the 3DS essentially powers down its "modern" firmware and enters a firmware called "DS(i) Mode", which closely mimics the DS (and DSi) environment using that hardware-level compatibility.

!!! info "How DS(i) Mode Renders Games"

    In DS(i) mode, the 3DS behaves as if it were a DS or DSi, with most of the newer system's features disabled. Things like wireless, screen brightness controls, and even some SD card access are limited or rerouted through legacy systems. However, DS(i) Mode does take a few liberties when rendering games. For example, even though you have access to the Circle Pad on a 3DS, it’s essentially useless for DS games, as it just maps to the D-pad’s inputs. Thus, you’ll still be using the D-pad to control movement. One "crime" I find particularly egregious is that DS(i) Mode tries to take advantage of the 3DS' larger screens and resolution when playing DS games. It upscales the original DS resolution (256x192) to a 5:3 ratio (400x240) for the 3DS' displays. This upscaling can lead to a lot of blur and distortion, especially on XL variants of the 3DS. While Nintendo did provide an option to fix this (by holding Start or Select as the system boots into DS(i) Mode) which would force the game to render at the original 4:3 resolution, many people didn’t know about it as Nintendo either didn’t market the feature well or left it as a hidden option. **This guide will focus on how to make it so that DS(i) Mode will automatically render games at the original resolution**. Please keep in mind, however, that if you'd like you can mess around with the homebrew we will be installing.

1. Open Universal Updater from your Home Menu.
2. Search for "TWPatch". The icon looks like Mario standing next to a purple brick with "TWL" in big blue text right above them.
3. Download "TWPatch.3dsx".

!!! note ""

    If you would like, you may choose to install the `.cia` version to launch through the Home Menu. However, for the sake of the tutorial we will be sticking with the `.3dsx` version.

4. Press Start to exit the Universal Updater.
5. Open The Homebrew Launcher.
6. Navigate to `TWPatch.3dsx` and select it.
7. Press Y + B once the application opens.
8. Press A to toggle on "Invert START+SELECT function".
9. Press B.
10. Hold Start to begin the patch process. This may take a few minutes, so get a quick drink of water! :)
11. Once the patching is finished, hold Select to exit out to The Homebrew Launcher.
12. Press the Home button to exit out to the Home Menu.
13. Open up your DS game of choice.
14. Enjoy better clarity!
