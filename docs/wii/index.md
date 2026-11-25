# RIP Bozotendo, Wii

!!! warning "Important Warning"

    Until I say it isn't, **this megathread will continually be in a state of WIP**! I am continually working to add things to here that may be pertinent to us. If you want information on something, please let me know. I will try my best to update this thread as needed or as I come along certain information.

## Disclaimers

- Please know that there will be some proper terminology to understand! The word "root" may come up a lot in discussion regarding the file structure of your SD card, which means when you are currently not in any folder on your SD card.
    - Additionally, you may see terms like "Open Shop Channel" and "USB Loader GX", which are apps installed after hacking your Wii. This chapter of this megathread is intended to be read sequentially, so you may come across terms you may not quite understand if you aren't reading in the proper order.
- You will need an SD card for everything to do in this guide. Thankfully, this is a lot easier of a choice compared to how it is with the 3DS and its "New" and "Old" variants. It uses the same format of FAT32 like the 3DS, but it doesn't need you to choose between whether you need a micro variant SD card or not. All Wiis use a large sized SD card, but for simplicity's sake I will simply refer to that as an SD card.
    - ***If you are using a Wii mini, you will NOT be able to use an SD card with your Wii***! You can use a USB flash drive or a hard drive instead, but for all intents and purposes **you don't really want to mod a Wii mini for its lack of features compared to other models**.
    - I would recommend at least a 128 GB SD card, but no more than 256. Realistically, that is all you need.
- A big problem with Wii homebrew tools for computers is that a lot of the time each operating system has a different application that does the exact same purpose. It can get kind of annoying, but I will try to account for that accordingly.
- There are 2 main ways people play backed up Wii games, WiiFlow Lite or USB Loader GX. I will *NOT* be providing support with use with WiiFlow Lite, mainly because I use USB Loader GX and am too lazy to actually figure out WiiFlow Lite out for myself. :P

## Formatting your SD Card (Assuming You Have a 64+ GB SD Card)

### Windows

1. Go to [this website](http://ridgecrop.co.uk/index.htm?guiformat.htm).
2. The website generally looks a bit old, but just click the giant image of the formatter and it will install `guiformat.exe`
3. Insert your old SD card into your computer, the one that's in your Wii currently before upgrading it. If you didn't have an SD card inside your Wii before attempting, ignore this step.
    - *Make sure your Wii is turned off before taking it out of your system*!
4. Take anything and everything in that SD card and put it somewhere on your computer you'd remember. This is **CRUCIAL** as formatting your SD card wipes everything. Make sure you also don't play around with the locations of every file inside the folders, alas it should just be dragging and dropping them somewhere.
5. Eject your old SD card from your computer. Do not throw it out just yet.
6. Insert your new SD card into your computer now.
7. In guiformat, select the letter for your SD card (E://, for example. your computer's hard drive is the C:// drive).
8. If your SD card is exactly 64 GB, enter 32768 in the allocation unit size. Otherwise, 65536.
9. Enter anything for the volume label.
10. Make sure "Quick Format" is selected.
11. Press "Start" and "OK", then once done close the application.
12. Drag and drop the contents of your old SD card into the newly formatted SD card.
13. Eject your new SD card from your computer and insert it into your Wii.
14. Turn your Wii on. If your system boots correctly, you may now throw away your old SD card. Otherwise, repeat this process from step 3 until it works.

### Linux

1. Using your distro's package manager (`apt-get`, `pacman`, or `flatpak`, to name a few), install GParted. This can be done by opening a Terminal window and installing as outlined by the distro's documentation.
2. Insert your old SD card into your computer, the one that's in your Wii currently before upgrading it. If you didn't have an SD card inside your Wii before attempting, ignore this step.
    - *Make sure your Wii is turned off before taking it out of your system*!
3. Take anything and everything in that SD card and put it somewhere on your computer you'd remember. This is **CRUCIAL** as formatting your SD card wipes everything. Make sure you also don't play around with the locations of every file inside the folders, alas it should just be dragging and dropping them somewhere.
4. Eject your old SD card from your computer. Do not throw it out just yet.
5. Insert your new SD card into your computer now.
6. Back in your Terminal, type `sudo gparted`.
7. Find your SD card in the drop-down box at the top right of the GParted window.
8. Right-click on the unallocated /dev/sdb1 and select Format to and click fat32.
9. Click the green checkmark and then the Apply button to apply the changes. This may take a bit.
10. Once this is finished, close out of GParted.
11. Drag and drop the contents of your old SD card into the newly formatted SD card.
12. Eject your new SD card from your computer and insert it into your Wii.
13. Turn your Wii on. If your system boots correctly, you may now throw away your old SD card. Otherwise, repeat this process from step 2 until it works.

### MacOS

1. Insert your old SD card into your computer, the one that's in your Wii currently before upgrading it. If you didn't have an SD card inside your Wii before attempting, ignore this step.
    - *Make sure your Wii is turned off before taking it out of your system*!
2. Take anything and everything in that SD card and put it somewhere on your computer you'd remember. This is **CRUCIAL** as formatting your SD card wipes everything. Make sure you also don't play around with the locations of every file inside the folders, alas it should just be dragging and dropping them somewhere.
3. Eject your old SD card from your computer. Do not throw it out just yet.
4. Insert your new SD card into your computer now.
5. Open a Terminal window on your Mac.
6. Enter `diskutil list`. A bunch of seemingly-gibberish will show up, however, your SD card will follow the format of `/dev/diskX` on the list of disks, along with the "name" of the SD card showing up somewhere in its respective section
7. Enter `sudo diskutil eraseDisk FAT32 (name) MBRFormat /dev/diskX`. Make sure you change X to the disk number you got earler, and change (name) with the name of your SD card. You will be prompted to enter your admin password, so please do so.
8. Once it is finished, drag and drop the contents of your old SD card into the newly formatted SD card.
9. Eject your new SD card from your computer and insert it into your Wii.
10. Turn your Wii on. If your system boots correctly, you may now throw away your old SD card. Otherwise, repeat this process from step 1 until it works.

## Wii Hacks Guide

!!! info ""

    <https://wii.hacks.guide/>

This website will continuously stay up to date with the latest information on how to hack your Wii.

!!! danger "Please Do This!"

    From the Open Shop Channel section of the guide, **make sure to install Homebrew Browser**! This will make installing homebrew a lot easier on your system. Additionally, from the Recommended Homebrew section, **make sure to download Nintendont, USB Loader GX, and YAWM ModMii Edition**! These are going to be essential for what we do later on!

!!! note "WiiConnect24"

    For the sake of consistency, when following these steps make sure to select Express Setup. Follow the 4 steps below and once this is finished, make sure to do the DNS setting tweak that the WiiLink Guide says is optional.

    1. Select your region.
    2. Choose "Yes" for the regional channels like the Kirby TV Channel.
    3. Choose the Translated option for setting your language, as this translates the regional channels to English.
    4. Finally, for the Food Channel, select the "Domino's" option if you are in the US or Canada, otherwise choose "Standard".

!!! note "The Final Section"

    In the "Nintendo Wi-Fi Connection" section of the guide, stick to only whatever automatically patches your games for Wiimmfi. There are 2 methods to automatically patch discs, however, since we are using the DNS patch for WiiLink make sure to use the automatic disc patching through Priiloader method. Make sure to also follow the automatic backup patching method through USB Loader GX's global settings, even if we don't have any backups installed yet!

## Pirating Wii or GameCube Games

!!! note "About Steps 1-10"

    These steps are just to get the GameCube back end set up. Once this is set up, simply repeat as needed from Step 8.

1. Open the Homebrew Channel on your Wii.
2. Load up Nintendont.
3. Once it is done initializing, press A to select SD as the source.
4. You should see your game in the list. Navigate to it.
5. (*Optional* ***if you do not have a GameCube Memory Card***) Press B access the Nintendont settings. Navigate to "Memcard Emulation" and toggle that on. Press Home once finished. If you already have a GameCube Memory Card and would like to continue using it, just insert it into one of the Memory Card slots on your Wii.
6. Press Home as much as you can to back out of Nintendont
7. Exit the Homebrew Channel.
8. Turn off your Wii.
9. Take out the SD card.
10. Insert your Wii's SD card into your computer. If you're on Windows, take note of the drive letter that your SD card is assigned (ie. D:)
11. On the root of your Wii's SD card, make folders called `wbfs` and `games` if they doesn't exist already. We will be using these for registering all our games with the Wii, with the respective folders belonging to Wii and GameCube games.
12. In our lovely Discord server, I have made it so our fantastic bot can give you access to a library of ROMs that work with the Wii. For our case, whenever the bot is online please type "!w emulation wii" or "!w emulation gamecube" for a library of these files. Note that you're going to have to try to see if your ROM of choice is in a specific set and if not choose another.
13. Download your `.rvz` file of choice from a set.
14. Download, extract, and open [TinyWiiBackupManager](https://github.com/mq1/TinyWiiBackupManager/releases/latest) on your computer. For MacOS, after downloading the file and running the `.dmg` installer, in a Terminal window type `xattr -rd com.apple.quarantine /Applications/TinyWiiBackupManager.app` to disable MacOS' notarization check on the app since it is not notarized by Apple yet.
15. Click on the button at the bottom left that looks like a hard drive.
16. You should see a window pop up that looks like a File Explorer. In the Removable Devices section at the bottom left of this window, you should see the drive letter for your SD card. (ie. D:)
17. At the top right, click the + button.
18. Navigate to your game of choice and select it. If you have multiple, hold Control (Option on MacOS) on your keyboard and click on the next one to have them both selected.
19. Click Open. This will load your games of choice onto your Wii's SD card, which will take some time. Be patient!
20. Once the wheel at the bottom left has stopped and your games have shown up in the UI, close out of TinyWiiBackupManager.
21. Remove the SD card from your computer.
    - Make sure to properly eject it to avoid any and all corruption!
22. Insert your SD card into your Wii.
23. Turn on your Wii.
24. Load up USB Loader GX from the Homebrew Channel. Remember to press A to enter SD card mode.
25. Launch your game. Happy Gaming!

!!! info "What's The Point?"

    You may notice that all this program did was place your game in a folder titled `(game title) [game ID]` inside the `wbfs` folder, while renaming the ROM to the game ID. This is a very menial task anyone can do, so why go through all this hassle? This is mainly because some ROMs will be over 4 GB in size, and a FAT32-formatted drive cannot hold individual files that are bigger than 4 GB. TinyWiiBackupManager does the extremely arduous process of splitting up the ROM accordingly on your SD card for you, so for example you may see a `RSBE01.wbf1` file and a `RSBE01.wbfs` file in the `Super Smash Bros. Brawl [RSBE01]` folder inside your `wbfs` folder when the ROM is over 7 GB big!

## Forwarding USB Loader GX Entries to Home Menu

Would you like to not have to constantly open USB Loader GX to play your Wii games from now on? What if you could just load your USB Loader GX games from the Home Menu as if they were games loaded into the Disc Channel? These instructions are here for you!

!!! warning "Only For Wii"

    Unfortunately, you cannot forward these GameCube titles to the Wii Home Menu without messing with Hex Editors and the like, so unless you're comfortable with that I would advise against that and just load them from USB Loader GX. If you'd like, however, instructions can be found [here](https://gbatemp.net/threads/gamecube-forwarding-in-wii-menu-through-usbloadergx-nintendont.612845/).

!!! danger "DO NOT!!!"

    Do ***NOT*** follow these instructions for *Mario Party 9* and *A Boy and His Blob*! Doing so ***WILL*** brick your Wii! If you do, please note, however, that the Wii Hacks Guide has proper instructions on brick prevention embedded into its hacking guide.

!!! warning "Wine Usage"

    The software we will be using to do this is Windows exclusive! MacOS/Linux users will need to use a compatibility layer like Wine or Proton to work with this software!

1. Turn off your Wii.
2. Take out the SD card.
3. Insert your Wii's SD card into your computer. If you're on Windows, take note of the drive letter that your SD card is assigned (ie. D:)
4. Download, extract, and open [WiiGSC](https://github.com/modmii/WiiGSC/releases/latest).
5. The first launch of the program will talk to you about common key creation. Just click OK on any popups that appear.
6. A disclaimer will appear about this software being "use at your own risk". Check the box to say you've read the information and then close out of that disclaimer window.
7. Click on `Open WBFS Drive`. Click on the drive letter for your SD card. If you're running the program through Wine, assuming you have no other storage devices plugged into your computer the SD card should be D:.
8. Select the game you would like to create a channel for, and then click on `Use for Channel Creation`.
9. For the Loader of choice, select `USB Loader GX (ISO/WBFS) - SD` from the dropdown.
10. Click on `Create Channel`. This should create a `.wad` file that is necessary for the forwarder.
11. Repeat steps 8-10 for as many games as you'd like.
12. On the root of your SD card, if it doesn't already exist create a folder called `WAD`. Drag and drop the `.wad` file(s) we generated earlier into this folder.
13. Close out of WiiGSC.
14. Safely eject your SD card from your PC.
15. Insert your SD card back into your Wii.
16. Turn on your Wii.
17. Open the Homebrew Channel on your Wii.
18. Load up YAWM ModMii Edition.
19. Navigate into the `WAD` folder we created a bit ago. Your `.wad` file(s) should be located there.
20. Install the `.wad` file(s).
21. Once this is done, close out of YAWM ModMii Edition. You should be back in the Homebrew Channel.
22. Press the Home button and select "Exit to Home Menu".
23. Your forwarded game(s) should now appear on the Home Menu! You may even move them around your Home Menu as you'd like by holding A+B and moving the Wiimote around, unlike the Disc Channel!

!!! warning "Only 48 Games!"

    The Wii Menu is limited to 48 channels, not including existing system channels. Please use this efficiently, such as if you only have a small Wii library or just want only the games you play the most on the Home Screen.

## Managing Wii Saves & Miis

!!! warning "Please Do This!"

    Before attempting to back up any game saves, please make sure you've ran your game of choice at least once on your Wii! This is so that we will have information to work with! Seems like a no brainer, but please be weary.

1. Open the Homebrew Channel on your Wii.
2. Load up Homebrew Browser.
3. In the Utilities section, navigate to Save Manager GX and install it.
4. Close out of Homebrew Browser. You should be back in the Homebrew menu.
5. Load up Save Manager GX.

### Saves

#### Backing up

6. Ensure the source is set to Wii. You can do this by going to the left most icon on the bar at the top, pressing A, navigating to `wii` and pressing A.
7. Navigate to your game of choice and press A.
8. Navigate to "Extract" and press A.
9. Navigate to "Default" and press A.
10. Press A on OK to confirm your back up.
11. Do what you want with this back up!

#### Restoring

6. Ensure the source is set to SD. You can do this by going to the left most icon on the bar at the top, pressing A, navigating to `sd` and pressing A.
7. Navigate to where your save file is located at on your SD card and select the file. The default location is usually in `/savegames/`.
8. Navigate to "Install" and press A.
9. Press A on OK to confirm your restoration.
10. Close out of Save Manager GX by pressing the Home Button and then Wii Menu.
11. Load up your game of choice. You should see your newly restored save!

### Miis

#### Backing up

6. Ensure the source is set to Mii. You can do this by going to the left most icon on the bar at the top, pressing A, navigating to `mii` and pressing A.
7. Navigate to your Mii of choice and press A.
8. Navigate to "Extract" and press A.
9. Navigate to "Default" and press A.
10. Press A on OK to confirm your back up.
11. Do what you want with this back up!

#### Restoring

6. Ensure the source is set to SD. You can do this by going to the left most icon on the bar at the top, pressing A, navigating to `sd` and pressing A.
7. Navigate to where your saved Mii's file is located at on your SD card and select the file. The default location is usually in `/savegames/`.
8. Navigate to "Install" and press A.
9. Press A on OK to confirm your restoration.
10. Close out of Save Manager GX by pressing the Home Button and then Wii Menu.
11. Load up the Mii Channel. You should see your newly restored Mii!

## Managing GameCube Saves

!!! note "Why Not Nintendont?"

    This guide will go over how to extract/restore saves from/to a Memory Card on your Wii. Nintendont's emulated memory card data can be found readily on your SD card in `/saves/`.

1. Open the Homebrew Channel on your Wii.
2. Load up Homebrew Browser.
3. In the Utilities section, navigate to GCMM and install it.
4. Close out of Homebrew Browser. You should be back in the Homebrew menu.
5. Load up GCMM.

### Backing up

6. Select "Wii Front SD slot"
7. On your Wiimote, press B and - to enter raw backup mode. If you're using a GameCube controller, press L and Y.
8. Select the slot that has your memory card using the appropriate button (A or B).
9. Back up as you'd like.
10. When the dump is/are complete, press B.
11. Press Home (Wiimote) or Start (GameCube controller) to exit GCMM.
12. Do what you want with this back up! It is stored in the `/MCBACKUP/` folder on your SD card.

### Restoring

6. Select "Wii Front SD slot"
7. On your Wiimote, press B and + to enter raw restore mode. If you're using a GameCube controller, press L and X.
8. Select the slot that has your memory card using the appropriate button (A or B).
9. Restore whichever save you'd like from where it's located on your SD card.
10. When the restoration is complete, press B.
11. Press Home (Wiimote) or Start (GameCube controller) to exit GCMM.
12. Happy gaming!

## Dumping Wii/GameCube Discs

1. Insert your game disc into the slot.
2. Open the Homebrew Channel on your Wii.
3. Load up Homebrew Browser.
4. In the Utilities section, navigate to CleanRip and install it.
5. Close out of Homebrew Browser. You should be back in the Homebrew menu.
6. Read the disclaimer and then press A if any pops up.
7. Press A to enable checksum verification.
8. You'll be prompted to select a device type. We are using an SD card, so navigate to "Front SD" and press A.
9. Your SD card should already be inserted, so press A to continue.
10. Navigate to the "FAT" filesystem type and press A.
11. Navigate to "Yes" if prompted to download [redump.org](http://redump.org/) DAT files. Press A.
12. Your disc should already be inserted. Press A.
13. You may be prompted if your disc is an unlicensed datel disc. Just select "No".
14. (**WII ONLY**) Set `Dump Size` to Auto, `Chunk Size` to Max, and `New device per chunk` to No. Press A.
    - If you're dumping a GameCube Disc, just press A.
15. The disc should now be dumping! This will take a while, especially for Wii games which can take upwards of 30 minutes sometimes. Go for a quick walk in the meantime. :)
16. Once it's done, close out of CleanRip by pressing B. You should be in the Homebrew Channel now.
17. Turn off your Wii.
18. Take out the SD Card.
19. Insert your Wii's SD card into your computer.

!!! warning "Divergence"

    From now until the end of these instructions, there will be a divergence in how to use these backups. I will make subsections in the table of contents accordingly. You can click the subsection you want from this warning.

    1. [Wii Disc to USB Loader GX](../wii/#step-20-wii-disc-to-usb-loader-gx)
    2. [Wii Disc to ROM Format](../wii/#step-20-wii-disc-to-rom-format)
    3. [GameCube Disc to USB Loader GX](../wii/#step-20-gamecube-disc-to-usb-loader-gx)
    4. [GameCube Disc to ROM Format](../wii/#step-20-gamecube-disc-to-rom-format)

### Step 20+: Wii Disc to USB Loader GX

20. Your dump should be on the root of your SD card in 2 parts. For example, *House of the Dead Overkill*'s dump will have 2 files that look like `RHOE8P.part0.iso` and `RHOE8P.part1.iso`. Select these files and drag them to somewhere on your PC, as the SD's card FAT32 file format does not allow you to have files bigger than 4 GB at once on your SD card. Once this is done, you may delete the dumped files from your SD card as we will no longer need them.

21. The instructions here vary for operating system. Look at what bullet point of this step is relevant to you.

    - **Windows**: Open the folder where you dragged your dumped files in File Explorer. In the Address Bar, type `cmd`. A Command Prompt window should have opened in the relevant folder. Copy/paste the following command into the Command Prompt:
        ```
        copy /b *.part?.iso game.iso
        ```
    - **MacOS/Linux**: Open the folder where you dragged your dumped files in Finder/whatever file browser you use. Right click the window and click on "Open in Terminal". A Terminal window should have opened in the relevant folder. Copy/paste the following command into the Terminal:
        ```
        cat `ls *.part?.iso | sort` > game.iso
        ```

    Press Enter. Wait for this to finish, and when it's done close out of Command Prompt/Terminal. You may now delete the dumped files from your PC as well, as we no longer need them. (ie. `RHOE8P.part0.iso` and `RHOE8P.part1.iso`).

22. Follow the [Pirating Wii Games](../wii/#pirating-wii-or-gamecube-games) guide from Step 8 onward, as the installation instructions are exactly the same!

### Step 20+: Wii Disc to ROM Format

!!! warning "Do You Have Save Data?"

    Since we will be transferring between a Wii to Dolphin Emulator, save files will not persist as game save data was stored on the Wii's NAND and NOT on the game disc itself. If you have relevant save data, please be sure to follow [these steps](../wii/#managing-wii-saves-miis) to back up your saves! Additionally, step 29 onward is meant for importing this save to Dolphin emulator!

20. Your dump should be on the root of your SD card in 2 parts. For example, *House of the Dead Overkill*'s dump will have 2 files that look like `RHOE8P.part0.iso` and `RHOE8P.part1.iso`. Select these files and drag them to somewhere on your PC, as the SD's card FAT32 file format does not allow you to have files bigger than 4 GB at once on your SD card. Once this is done, you may delete the dumped files from your SD card as we will no longer need them.

21. The instructions here vary for operating system. Look at what bullet point of this step is relevant to you.

    - **Windows**: Open the folder where you dragged your dumped files in File Explorer. In the Address Bar, type `cmd`. A Command Prompt window should have opened in the relevant folder. Copy/paste the following command into the Command Prompt:
        ```
        copy /b *.part?.iso game.iso
        ```
    - **MacOS/Linux**: Open the folder where you dragged your dumped files in Finder/whatever file browser you use. Right click the window and click on "Open in Terminal". A Terminal window should have opened in the relevant folder. Copy/paste the following command into the Terminal:
        ```
        cat `ls *.part?.iso | sort` > game.iso
        ```

    Press Enter. Wait for this to finish, and when it's done close out of Command Prompt/Terminal. You may now delete the dumped files from your PC as well, as we no longer need them. (ie. `RHOE8P.part0.iso` and `RHOE8P.part1.iso`).

22. In our lovely Discord server, there are instructions tied to our Discord bot about how to set up the Dolphin emulator. All you need to do is follow the instructions to bot gives you when entering the command "!w emulation wii". Just ensure that the path you mention in step 5 of *that* instruction set is the same path where your `game.iso` is located.

23. In the Dolphin UI, right click your game. In the dropdown menu left click on `Convert File...`.

24. In the first dropdown, choose "RVZ" as the Format.

25. Click on Convert.

26. A file explorer window will show up. Save the new `.rvz` file to the same place as your `game.iso`, then click on Save.

27. Once the conversion is finished, click OK. If you'd like, you can open a file explorer window to delete the `game.iso` file where it is located, as we no longer need it.

28. In the Dolphin UI, click "Refresh". Your `.rvz` format ROM should be visible in Dolphin!

!!! note "Are You Done?"

    The final few steps here are for if you have backed up Wii save data you'd like to import. **If you don't have that, you're done! You may (safely) eject your SD card, insert it back into your Wii, and have fun again!** If you do, however, follow along just for a little longer.

29. In the Dolphin UI, click `Tools` -> `Import Wii Save...`.
30. Navigate to where the `.bin` of your save file of choice is saved on your SD card. This is by default usually in `/savegames/`. Press Open.
31. Click Yes on any popups that may appear. Do note that if you had existing save data with Dolphin, this will be overwritten
32. Click OK once your save data has successfully been imported.
33. Double click on your game and enjoy!

### Step 20+: GameCube Disc to USB Loader GX

!!! warning "Do You Have Save Data?"

    If you already have a GameCube Memory Card and do not want Nintendont to use a virtual memory card save simply **put it in a slot on your Wii, make sure in Nintendont settings "Memcard Emulation" is off, and ignore steps 24-26**. Otherwise, this subsection assumes you have already backed up your Memory Card. If not, follow [these steps](../wii/#managing-gamecube-saves-backing-up) to do so.

20. Your dump should be on the root of your SD card as 1 `.iso` file. Select this file and drag it into the `games` folder., creating it if it doesn't already exist.
21. Rename the dump to `game.iso`.
22. Make a new folder inside of this `games` folder. Name that new folder the name of your game; this does not have to be hyper-specific. For example, you may have `/games/Super Smash Bros Melee/` and this will work.
23. Drag that `game.iso` file into this new folder.
24. Go back to the root of your SD card, and then to the `MCBACKUP` folder.
25. Copy the `.raw` backup file from here, and then go back to the root of your SD card once more.
26. Paste the backup file here and rename it to `ninmen.raw`.
27. Safely eject your SD card from your PC.
28. Insert your SD card back into your Wii.
29. Turn on your Wii.
30. Open the Homebrew Channel on your Wii.
31. Open USB Loader GX.
32. Once it is done initializing, press A to select SD as the source.
33. You should see your game in the list. Navigate to it.
34. Launch it. Happy Gaming!

### Step 20+: GameCube Disc to ROM Format

!!! warning "Do You Have Save Data?"

    Since we will be transferring between a GameCube Memory Card to Dolphin Emulator, save files will not persist as game save data was stored on the Wii's NAND and NOT on the game disc itself. If you have relevant save data, please be sure to follow [these steps](../wii/#managing-gamecube-saves-backing-up) to back up your saves! Additionally, step 28 onward is meant for importing this save to Dolphin emulator!

20. Your dump should be on the root of your SD card as 1 `.iso` file. Select this file and drag it to somewhere on your PC. Once this is done, you may delete the dumped file from your SD card as we will no longer need it.
21. In our lovely Discord server, there are instructions tied to our Discord bot about how to set up the Dolphin emulator. All you need to do is follow the instructions to bot gives you when entering the command "!w emulation gamecube". Just ensure that the path you mention in step 5 of *that* instruction set is the same path where your `.iso` is located.
22. In the Dolphin UI, right click your game. In the dropdown menu left click on `Convert File...`.
23. In the first dropdown, choose "RVZ" as the Format.
24. Click on Convert.
25. A file explorer window will show up. Save the new `.rvz` file to the same place as your `.iso`, then click on Save.
26. Once the conversion is finished, click OK. If you'd like, you can open a file explorer window to delete the `.iso` file where it is located, as we no longer need it.
27. In the Dolphin UI, click "Refresh". Your `.rvz` format ROM should be visible in Dolphin!

!!! note "Are You Done?"

    The final few steps here are for if you have backed up GameCube save data you'd like to import. **If you don't have that, you're done! You may (safely) eject your SD card, insert it back into your Wii, and have fun again!** If you do, however, follow along just for a little longer.

28. In the Dolphin UI, click `Config` -> `GameCube`. In the Device Settings section, make sure Slot A has "Memory Card" selected from its dropdown. Click Close afterward.
29. In the Dolphin UI, click `Tools` -> `Memory Card Manager...`.
30. Click Open next to slot B.
31. Navigate to the saves folder on your SD/USB, and open the .raw file named after the game ID of your game.
32. Click Switch to B.
33. Select the save you would like to copy and click "Copy to A".
34. Click Close.
35. Double click on your game and enjoy!

## Retro Gaming

***Coming Soon™...***

## Using Cheats

***Coming Soon™...***

## Mods

***Coming Soon™...***

## Theming

Want to make your Wii feel more personal? Here's a few ways you can theme your Wii! The guide will be split into the three places that support themes.

### Home Menu

1. Open the Homebrew Channel on your Wii.
2. Load up Homebrew Browser.
3. In the Utilities section, navigate to csm-installer and install it.
4. Close out of Homebrew Browser. You should be back in the Homebrew menu.
5. Load up csm-installer.
6. Automatically, the app should create a backup of your "base theme". This is your Wii's current unmodified Home Menu. Press A once finished.
7. Navigate to "Return to Wii System Menu" and select it.
8. Turn off your Wii.
9. Take out the SD card.
10. Insert your Wii's SD card into your computer.
11. On the root of your SD card, create a `themes` folder if it doesn't already exist.
12. On your computer go to [this website](https://www.wiithemer.org/).
13. Click on the "channel" that looks like a penguin building a brick wall. It will give you a console brick warning, but by now you should know how to reverse a brick.
14. From the "Select Theme :" dropdown, choose a theme you'd like.
15. From the "Select System Menu Version :" dropdown, choose your system menu version, which should be 4.3.
16. From the "Select System Region :" dropdown, choose your region code. (U for USA, E for Europe, J for Japan, K for Korea.).
17. Click on "Build Theme". Once it's finished, click on the button that has a file name with a `.csm` extension. This is your theme's file.
18. Drag and drop this `.csm` file to the `themes` folder of your SD card.
19. Safely eject your SD card from your PC.
20. Insert your SD card back into your Wii.
21. Turn on your Wii.
22. Open the Homebrew Channel on your Wii.
23. Open csm-installer.
24. Press A on "Install a theme".
25. Navigate to the `.csm` file from earlier and select it. Wait for it to finish installing.
26. Navigate to "Return to Wii System Menu" and select it.
27. Revel in your artistic excellence!

From now on, if you'd like to add more themes simply follow along from Step 8 onwards.

### Homebrew Channel

1. Turn off your Wii.
2. Take out the SD card.
3. Insert your Wii's SD card into your computer.
4. On your computer go to [this website](https://wiibrew.org/wiki/Homebrew_Channel/Themes).
5. Download a theme that you like. It should be a `.zip` file. Do not extract this yet!
6. Drag and drop this `.zip` file to your `/apps/` folder on your SD card. Unpack this `.zip` file within the folder, and then delete the original `.zip` file.
7. Safely eject your SD card from your PC.
8. Insert your SD card back into your Wii.
9. Turn on your Wii.
10. Open the Homebrew Channel on your Wii.
11. Open the newly created app in your Homebrew Channel. Your theme should be set up now!

### USB Loader GX

1. Turn off your Wii.
2. Take out the SD card.
3. Insert your Wii's SD card into your computer.
4. On your computer go to [this website](https://gbatemp.net/threads/dark-wii-usb-loader-gx-themes.584493/).
5. Download a theme that you like. It should be a `.zip` file. Do not extract this yet!
6. Drag and drop this `.zip` file to your `/apps/usbloader_gx` folder on your SD card. Unpack this `.zip` file within the folder, and then delete the original `.zip` file.
7. Safely eject your SD card from your PC.
8. Insert your SD card back into your Wii.
9. Turn on your Wii.
10. Open the Homebrew Channel on your Wii.
11. Open USB Loader GX.
12. Go to the Settings menu, and then go to Theme Menu.
13. Navigate to your theme and install it. Your theme should be set up now!

## FTPii (File Transfer Over Internet)

!!! info "What Is FTPii?"

    What if you could wirelessly transfer files between your computer and Wii without having to constantly move its SD card in and out of your multiple systems at home? This is where FTPii comes in. It allows you to do exactly that. I would advise, however, only do this for files small in size, as file transfer through FTP can be rather slow.

1. Open the Homebrew Channel on your Wii.
2. Load up Homebrew Browser.
3. In the Utilities section, search for "FTPii" and install it.
4. Once it's finished installing, press Home and return back to the Homebrew Channel.
5. Open the FTPii application.
6. The top of the screen should have an IP address and port number at the top. This will be in the format of [XXX.XXX.XXX.XXX](http://xxx.xxx.xxx.xxx/):(PORT). Keep note of it.
7. Leave your Wii aside for now, but leave it on and visible near you.

!!! note "Divergence"

    This section will now divide into 2 sections for instructions depending on your operating sytem.

### For Windows/MacOS

8. Go to [this website](https://cyberduck.io/download/).
9. Download for your operating system.
10. On Windows, run through the installer for the program and then open Cyberduck. On MacOS, unarchive the `.zip` file you downloaded using an unarchiver of your choice (the MacOS default one works just fine), drag and drop `Cyberduck.app` into your Applications pin in Finder, go to the Applications pin, right click on `Cyberduck.app`, select "Open", then confirm that you want to open the application.
11. In Cyberduck, click "Open Connection" at the top.
12. At the dropdown on the top, make sure "FTP (File Transfer Protocol)" is selected.
13. In the text box for "Server", enter the IP address on your Wii.
14. In the box for "Port", enter the port number on your Wii.
15. Cyberduck will now connect to your Wii's files directly. Open a window in your file explorer from here.
16. Use both Cyberduck and the window you just opened to do whatever dragging and dropping of files in and out of your SD card that you need to do. Note that because we are wirelessly transferring files here, files may take longer to transfer in and out of your system.
17. Once finished, close out of Cyberduck. It may prompt you to pay money, in which case just click "Later". Cyberduck will always be free to you, and you paying money is only to support the developers.
18. Back on your Wii, close out of FTPii.

### For Linux

8. In your file explorer (in my case, Dolphin on my Steam Deck), right click on the file path at the top and make sure "Show file path" is selected.
9. Click on the file path to open a textbox displaying the full file path.
10. Press Ctrl+A to highlight the entire thing and then Backspace to delete it all.
11. Enter the following into the file path bar: `ftp://(the ip address):(the port number)`. You should then almost instantly be able to access the files on your SD card.
12. Open a new tab or window of Dolphin. Use both of these tabs/windows to do whatever dragging and dropping of files in and out of your SD card that you need to do. Note that because we are wirelessly transferring files here, files may take longer to transfer in and out of your system.
13. Once finished, close out of the tab/window that contains your Wii's files and the other tab/window containing files on your Linux computer.
14. Back on your Wii, close out of FTPii.

## Ordering Pizza???

Yes, you can order pizza through your Wii. I mean, this is seriously nothing more than a novelty that loses its charm once you even do it once, but it's cool that you can do this in the first place? This stems from a Japan exclusive Wii channel called "The Demae Channel" that let you order food from local restaurants through your Wii to your front door. You would pay through cash on delivery. Using WiiLink's services in 2025, **which you should have set up if you followed the hacks guide**, you can order pizza from Domino's if you are in either the US or Canada! I wouldn't really recommend it, but I'm not your parent so if you want I won't stop you...

!!! warning "Assumptions Made!"

    **This guide assumes you have already set up WiiLink on your Wii**. The instructions should have been given to you through the Wii Hacks Guide, but you can find them again [here](https://wiilink.ca/guide/wii/). You should also have all the WiiLink patched channels on your Home Menu too.

1. On your computer, create a WiiLink account at [accounts.wiilink.ca](http://accounts.wiilink.ca/).
2. Turn on your Wii.
3. Open the Homebrew Channel.
4. Open the Homebrew Browser.
5. In the Utilities section, navigate to the WiiLink Account Linker app and install it.
6. Once that's finished, close out of the Homebrew Browser. You should be back in the Homebrew Channel now.
7. Open the WiiLink Account Linker.
8. A code should be displayed on screen. Take a picture or mental note of that code, and input it at [sso.riiconnect24.net/device](http://sso.riiconnect24.net/device) on your computer. This assumes you're still signed in.
9. Once this is successful, go back to [accounts.wiilink.ca](http://accounts.wiilink.ca/). Click on Food Delivery Settings.
10. In the dropdown box, select the number associated with your Wii.
11. Click on "Enable Dominos Ordering". You should be done with your computer now.
12. Back on your Wii, close out of the WiiLink Account Linker app, and then close out of the Homebrew Channel.
13. On the Wii's Home Menu, open the Food Channel.
14. If you have not previously set your address information, a prompt telling you to set it will appear. Press the `Address Info` button. Otherwise, select the `Change Address Information` button in the main menu.
15. Now you are in the Address Information menu. Press the arrows to traverse screens. Here you will enter your data. Make sure this data is accurate!
16. When you are finished, select the `Done` button and then `Demae`.
17. Follow the on-screen instructions, then select `Order` in the main menu.
18. You will now be prompted to select your region. Be sure to select your country correctly, as if not restaurants will fail to load. You will then be prompted to select your state/province, then city.
19. Select the `Pizza` button. This will load all the restaurants in your area. The first restaurant in the list is the one closest to you.
20. Select `See Menu` to list the different menu categories. Select the category you would like, then select a food item. In the item screen, you can add toppings and in/decrease quantity.
21. After adding a food item, you will be brought to the basket. To add a food item, scroll to the bottom and select `Add Order`. To proceed to checkout, select `Next`.
22. Double check your order before placing it. When you are ready, select the big green `Order` button.
23. If no error appeared, your order was placed successfully! To track your order, simply visit the Domino’s Tracker for your region and enter the phone number you entered in the Address Information menu.

Remember, this is cash on delivery only! Be sure to have some cash when the driver shows up at your doorstep. Additionally, I think ordering online through your smartphone is probably cheaper than doing this, but again I won't stop you...

If you'd like to order again, simply skip steps 1-12.
