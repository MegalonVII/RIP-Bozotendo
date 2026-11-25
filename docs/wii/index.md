# RIP Bozotendo, Wii {#rip-bozotendo-wii}

<div class="admonition warning">
  <p class="admonition-title">Important Warning</p>
  <p>Until I say it isn't, <strong>this megathread will continually be in a state of WIP</strong>! I am continually working to add things to here that may be pertinent to us. If you want information on something, please let me know. I will try my best to update this thread as needed or as I come along certain information.</p>
</div>

## Disclaimers {#disclaimers}

<ul>
  <li>Please know that there will be some proper terminology to understand! The word "root" may come up a lot in discussion regarding the file structure of your SD card, which means when you are currently not in any folder on your SD card.<ul>
      <li>Additionally, you may see terms like "Open Shop Channel" and "USB Loader GX", which are apps installed after hacking your Wii. This chapter of this megathread is intended to be read sequentially, so you may come across terms you may not quite understand if you aren't reading in the proper order.</li>
    </ul>
  </li>
  <li>You will need an SD card for everything to do in this guide. Thankfully, this is a lot easier of a choice compared to how it is with the 3DS and its "New" and "Old" variants. It uses the same format of FAT32 like the 3DS, but it doesn't need you to choose between whether you need a micro variant SD card or not. All Wiis use a large sized SD card, but for simplicity's sake I will simply refer to that as an SD card.<ul>
      <li><strong><em>If you are using a Wii mini, you will NOT be able to use an SD card with your Wii</em></strong>! You can use a USB flash drive or a hard drive instead, but for all intents and purposes <strong>you don't really want to mod a Wii mini for its lack of features compared to other models</strong>.</li>
      <li>I would recommend at least a 128 GB SD card, but no more than 256. Realistically, that is all you need.</li>
    </ul>
  </li>
  <li>A big problem with Wii homebrew tools for computers is that a lot of the time each operating system has a different application that does the exact same purpose. It can get kind of annoying, but I will try to account for that accordingly.</li>
  <li>There are 2 main ways people play backed up Wii games, WiiFlow Lite or USB Loader GX. I will <em>NOT</em> be providing support with use with WiiFlow Lite, mainly because I use USB Loader GX and am too lazy to actually figure out WiiFlow Lite out for myself. :P</li>
</ul>

## Formatting your SD Card (Assuming You Have a 64+ GB SD Card) {#formatting-your-sd-card-assuming-you-have-a-64-gb-sd-card}

### Windows {#windows}

<ol>
  <li>Go to <a class="external" href="http://ridgecrop.co.uk/index.htm?guiformat.htm" rel="" target="_blank">this website</a>.</li>
  <li>The website generally looks a bit old, but just click the giant image of the formatter and it will install <code>guiformat.exe</code></li>
  <li>Insert your old SD card into your computer, the one that's in your Wii currently before upgrading it. If you didn't have an SD card inside your Wii before attempting, ignore this step.<ul>
      <li><em>Make sure your Wii is turned off before taking it out of your system</em>!</li>
    </ul>
  </li>
  <li>Take anything and everything in that SD card and put it somewhere on your computer you'd remember. This is <strong>CRUCIAL</strong> as formatting your SD card wipes everything. Make sure you also don't play around with the locations of every file inside the folders, alas it should just be dragging and dropping them somewhere.</li>
  <li>Eject your old SD card from your computer. Do not throw it out just yet.</li>
  <li>Insert your new SD card into your computer now.</li>
  <li>In guiformat, select the letter for your SD card (E://, for example. your computer's hard drive is the C:// drive).</li>
  <li>If your SD card is exactly 64 GB, enter 32768 in the allocation unit size. Otherwise, 65536.</li>
  <li>Enter anything for the volume label.</li>
  <li>Make sure "Quick Format" is selected.</li>
  <li>Press "Start" and "OK", then once done close the application.</li>
  <li>Drag and drop the contents of your old SD card into the newly formatted SD card.</li>
  <li>Eject your new SD card from your computer and insert it into your Wii.</li>
  <li>Turn your Wii on. If your system boots correctly, you may now throw away your old SD card. Otherwise, repeat this process from step 3 until it works.</li>
</ol>

### Linux {#linux}

<ol>
  <li>Using your distro's package manager (<code>apt-get</code>, <code>pacman</code>, or <code>flatpak</code>, to name a few), install GParted. This can be done by opening a Terminal window and installing as outlined by the distro's documentation.</li>
  <li>Insert your old SD card into your computer, the one that's in your Wii currently before upgrading it. If you didn't have an SD card inside your Wii before attempting, ignore this step.<ul>
      <li><em>Make sure your Wii is turned off before taking it out of your system</em>!</li>
    </ul>
  </li>
  <li>Take anything and everything in that SD card and put it somewhere on your computer you'd remember. This is <strong>CRUCIAL</strong> as formatting your SD card wipes everything. Make sure you also don't play around with the locations of every file inside the folders, alas it should just be dragging and dropping them somewhere.</li>
  <li>Eject your old SD card from your computer. Do not throw it out just yet.</li>
  <li>Insert your new SD card into your computer now.</li>
  <li>Back in your Terminal, type <code>sudo gparted</code>.</li>
  <li>Find your SD card in the drop-down box at the top right of the GParted window.</li>
  <li>Right-click on the unallocated /dev/sdb1 and select Format to and click fat32.</li>
  <li>Click the green checkmark and then the Apply button to apply the changes. This may take a bit.</li>
  <li>Once this is finished, close out of GParted.</li>
  <li>Drag and drop the contents of your old SD card into the newly formatted SD card.</li>
  <li>Eject your new SD card from your computer and insert it into your Wii.</li>
  <li>Turn your Wii on. If your system boots correctly, you may now throw away your old SD card. Otherwise, repeat this process from step 2 until it works.</li>
</ol>

### MacOS {#macos}

<ol>
  <li>Insert your old SD card into your computer, the one that's in your Wii currently before upgrading it. If you didn't have an SD card inside your Wii before attempting, ignore this step.<ul>
      <li><em>Make sure your Wii is turned off before taking it out of your system</em>!</li>
    </ul>
  </li>
  <li>Take anything and everything in that SD card and put it somewhere on your computer you'd remember. This is <strong>CRUCIAL</strong> as formatting your SD card wipes everything. Make sure you also don't play around with the locations of every file inside the folders, alas it should just be dragging and dropping them somewhere.</li>
  <li>Eject your old SD card from your computer. Do not throw it out just yet.</li>
  <li>Insert your new SD card into your computer now.</li>
  <li>Open a Terminal window on your Mac. </li>
  <li>Enter <code>diskutil list</code>. A bunch of seemingly-gibberish will show up, however, your SD card will follow the format of <code>/dev/diskX</code> on the list of disks, along with the "name" of the SD card showing up somewhere in its respective section</li>
  <li>Enter <code>sudo diskutil eraseDisk FAT32 (name) MBRFormat /dev/diskX</code>. Make sure you change X to the disk number you got earler, and change (name) with the name of your SD card. You will be prompted to enter your admin password, so please do so.</li>
  <li>Once it is finished, drag and drop the contents of your old SD card into the newly formatted SD card.</li>
  <li>Eject your new SD card from your computer and insert it into your Wii.</li>
  <li>Turn your Wii on. If your system boots correctly, you may now throw away your old SD card. Otherwise, repeat this process from step 1 until it works.</li>
</ol>

## Wii Hacks Guide {#wii-hacks-guide}

<div class="admonition info">
  <p><a class="external" href="https://wii.hacks.guide/" rel="" target="_blank">https://wii.hacks.guide/</a></p>
</div>
<p>This website will continuously stay up to date with the latest information on how to hack your Wii.</p>
<div class="admonition danger">
  <p class="admonition-title">Please Do This!</p>
  <p>From the Open Shop Channel section of the guide, <strong>make sure to install Homebrew Browser</strong>! This will make installing homebrew a lot easier on your system. Additionally, from the Recommended Homebrew section, <strong>make sure to download Nintendont, USB Loader GX, and YAWM ModMii Edition</strong>! These are going to be essential for what we do later on!</p>
</div>
<div class="admonition note">
  <p class="admonition-title">WiiConnect24</p>
  <p>For the sake of consistency, when following these steps make sure to select Express Setup. Follow the 4 steps below and once this is finished, make sure to do the DNS setting tweak that the WiiLink Guide says is optional.</p>
  <ol>
    <li>Select your region. </li>
    <li>Choose "Yes" for the regional channels like the Kirby TV Channel.</li>
    <li>Choose the Translated option for setting your language, as this translates the regional channels to English.</li>
    <li>Finally, for the Food Channel, select the "Domino's" option if you are in the US or Canada, otherwise choose "Standard".</li>
  </ol>
</div>
<div class="admonition note">
  <p class="admonition-title">The Final Section</p>
  <p>In the "Nintendo Wi-Fi Connection" section of the guide, stick to only whatever automatically patches your games for Wiimmfi. There are 2 methods to automatically patch discs, however, since we are using the DNS patch for WiiLink make sure to use the automatic disc patching through Priiloader method. Make sure to also follow the automatic backup patching method through USB Loader GX's global settings, even if we don't have any backups installed yet!</p>
</div>

## Pirating Wii or GameCube Games {#pirating-wii-or-gamecube-games}

<div class="admonition note">
  <p class="admonition-title">About Steps 1-10</p>
  <p>These steps are just to get the GameCube back end set up. Once this is set up, simply repeat as needed from Step 8.</p>
</div>
<ol>
  <li>Open the Homebrew Channel on your Wii.</li>
  <li>Load up Nintendont.</li>
  <li>Once it is done initializing, press A to select SD as the source.</li>
  <li>You should see your game in the list. Navigate to it.</li>
  <li>(<em>Optional</em> <strong><em>if you do not have a GameCube Memory Card</em></strong>) Press B access the Nintendont settings. Navigate to "Memcard Emulation" and toggle that on. Press Home once finished. If you already have a GameCube Memory Card and would like to continue using it, just insert it into one of the Memory Card slots on your Wii.</li>
  <li>Press Home as much as you can to back out of Nintendont</li>
  <li>Exit the Homebrew Channel.</li>
  <li>Turn off your Wii.</li>
  <li>Take out the SD card.</li>
  <li>Insert your Wii's SD card into your computer. If you're on Windows, take note of the drive letter that your SD card is assigned (ie. D:)</li>
  <li>On the root of your Wii's SD card, make folders called <code>wbfs</code> and <code>games</code> if they doesn't exist already. We will be using these for registering all our games with the Wii, with the respective folders belonging to Wii and GameCube games.</li>
  <li>In our lovely Discord server, I have made it so our fantastic bot can give you access to a library of ROMs that work with the Wii. For our case, whenever the bot is online please type "!w emulation wii" or "!w emulation gamecube" for a library of these files. Note that you're going to have to try to see if your ROM of choice is in a specific set and if not choose another.</li>
  <li>Download your <code>.rvz</code> file of choice from a set.</li>
  <li>Download, extract, and open <a class="external" href="https://github.com/mq1/TinyWiiBackupManager/releases/latest" rel="" target="_blank">TinyWiiBackupManager</a> on your computer. For MacOS, after downloading the file and running the <code>.dmg</code> installer, in a Terminal window type <code>xattr -rd com.apple.quarantine /Applications/TinyWiiBackupManager.app</code> to disable MacOS' notarization check on the app since it is not notarized by Apple yet.</li>
  <li>Click on the button at the bottom left that looks like a hard drive.</li>
  <li>You should see a window pop up that looks like a File Explorer. In the Removable Devices section at the bottom left of this window, you should see the drive letter for your SD card. (ie. D:)</li>
  <li>At the top right, click the + button.</li>
  <li>Navigate to your game of choice and select it. If you have multiple, hold Control (Option on MacOS) on your keyboard and click on the next one to have them both selected.</li>
  <li>Click Open. This will load your games of choice onto your Wii's SD card, which will take some time. Be patient!</li>
  <li>Once the wheel at the bottom left has stopped and your games have shown up in the UI, close out of TinyWiiBackupManager.</li>
  <li>Remove the SD card from your computer.<ul>
      <li>Make sure to properly eject it to avoid any and all corruption!</li>
    </ul>
  </li>
  <li>Insert your SD card into your Wii.</li>
  <li>Turn on your Wii.</li>
  <li>Load up USB Loader GX from the Homebrew Channel. Remember to press A to enter SD card mode.</li>
  <li>Launch your game. Happy Gaming!</li>
</ol>
<div class="admonition info">
  <p class="admonition-title">What's The Point?</p>
  <p>You may notice that all this program did was place your game in a folder titled <code>(game title) [game ID]</code> inside the <code>wbfs</code> folder, while renaming the ROM to the game ID. This is a very menial task anyone can do, so why go through all this hassle? This is mainly because some ROMs will be over 4 GB in size, and a FAT32-formatted drive cannot hold individual files that are bigger than 4 GB. TinyWiiBackupManager does the extremely arduous process of splitting up the ROM accordingly on your SD card for you, so for example you may see a <code>RSBE01.wbf1</code> file and a <code>RSBE01.wbfs</code> file in the <code>Super Smash Bros. Brawl [RSBE01]</code> folder inside your <code>wbfs</code> folder when the ROM is over 7 GB big!</p>
</div>

## Forwarding USB Loader GX Entries to Home Menu {#forwarding-usb-loader-gx-entries-to-home-menu}

<p>Would you like to not have to constantly open USB Loader GX to play your Wii games from now on? What if you could just load your USB Loader GX games from the Home Menu as if they were games loaded into the Disc Channel? These instructions are here for you!</p>
<div class="admonition warning">
  <p class="admonition-title">Only For Wii</p>
  <p>Unfortunately, you cannot forward these GameCube titles to the Wii Home Menu without messing with Hex Editors and the like, so unless you're comfortable with that I would advise against that and just load them from USB Loader GX. If you'd like, however, instructions can be found <a class="external" href="https://gbatemp.net/threads/gamecube-forwarding-in-wii-menu-through-usbloadergx-nintendont.612845/" rel="" target="_blank">here</a>.</p>
</div>
<div class="admonition danger">
  <p class="admonition-title">DO NOT!!!</p>
  <p>Do <strong><em>NOT</em></strong> follow these instructions for <em>Mario Party 9</em> and <em>A Boy and His Blob</em>! Doing so <strong><em>WILL</em></strong> brick your Wii! If you do, please note, however, that the Wii Hacks Guide has proper instructions on brick prevention embedded into its hacking guide.</p>
</div>
<div class="admonition warning">
  <p class="admonition-title">Wine Usage</p>
  <p>The software we will be using to do this is Windows exclusive! MacOS/Linux users will need to use a compatibility layer like Wine or Proton to work with this software!</p>
</div>
<ol>
  <li>Turn off your Wii.</li>
  <li>Take out the SD card.</li>
  <li>Insert your Wii's SD card into your computer. If you're on Windows, take note of the drive letter that your SD card is assigned (ie. D:)</li>
  <li>Download, extract, and open <a class="external" href="https://github.com/modmii/WiiGSC/releases/latest" rel="" target="_blank">WiiGSC</a>.</li>
  <li>The first launch of the program will talk to you about common key creation. Just click OK on any popups that appear.</li>
  <li>A disclaimer will appear about this software being "use at your own risk". Check the box to say you've read the information and then close out of that disclaimer window.</li>
  <li>Click on <code>Open WBFS Drive</code>. Click on the drive letter for your SD card. If you're running the program through Wine, assuming you have no other storage devices plugged into your computer the SD card should be D:.</li>
  <li>Select the game you would like to create a channel for, and then click on <code>Use for Channel Creation</code>.</li>
  <li>For the Loader of choice, select <code>USB Loader GX (ISO/WBFS) - SD</code> from the dropdown.</li>
  <li>Click on <code>Create Channel</code>. This should create a <code>.wad</code> file that is necessary for the forwarder.</li>
  <li>Repeat steps 8-10 for as many games as you'd like.</li>
  <li>On the root of your SD card, if it doesn't already exist create a folder called <code>WAD</code>. Drag and drop the <code>.wad</code> file(s) we generated earlier into this folder.</li>
  <li>Close out of WiiGSC.</li>
  <li>Safely eject your SD card from your PC.</li>
  <li>Insert your SD card back into your Wii.</li>
  <li>Turn on your Wii.</li>
  <li>Open the Homebrew Channel on your Wii.</li>
  <li>Load up YAWM ModMii Edition.</li>
  <li>Navigate into the <code>WAD</code> folder we created a bit ago. Your <code>.wad</code> file(s) should be located there.</li>
  <li>Install the <code>.wad</code> file(s).</li>
  <li>Once this is done, close out of YAWM ModMii Edition. You should be back in the Homebrew Channel.</li>
  <li>Press the Home button and select "Exit to Home Menu".</li>
  <li>Your forwarded game(s) should now appear on the Home Menu! You may even move them around your Home Menu as you'd like by holding A+B and moving the Wiimote around, unlike the Disc Channel!</li>
</ol>
<div class="admonition warning">
  <p class="admonition-title">Only 48 Games!</p>
  <p>The Wii Menu is limited to 48 channels, not including existing system channels. Please use this efficiently, such as if you only have a small Wii library or just want only the games you play the most on the Home Screen.</p>
</div>

## Managing Wii Saves &amp; Miis {#managing-wii-saves-miis}

<div class="admonition warning">
  <p class="admonition-title">Please Do This!</p>
  <p>Before attempting to back up any game saves, please make sure you've ran your game of choice at least once on your Wii! This is so that we will have information to work with! Seems like a no brainer, but please be weary.</p>
</div>
<ol>
  <li>Open the Homebrew Channel on your Wii.</li>
  <li>Load up Homebrew Browser.</li>
  <li>In the Utilities section, navigate to Save Manager GX and install it.</li>
  <li>Close out of Homebrew Browser. You should be back in the Homebrew menu.</li>
  <li>Load up Save Manager GX.</li>
</ol>

### Saves {#saves}

#### Backing up {#backing-up}

<ol start="6">
  <li>Ensure the source is set to Wii. You can do this by going to the left most icon on the bar at the top, pressing A, navigating to <code>wii</code> and pressing A.</li>
  <li>Navigate to your game of choice and press A.</li>
  <li>Navigate to "Extract" and press A.</li>
  <li>Navigate to "Default" and press A.</li>
  <li>Press A on OK to confirm your back up.</li>
  <li>Do what you want with this back up!</li>
</ol>

#### Restoring {#restoring}

<ol start="6">
  <li>Ensure the source is set to SD. You can do this by going to the left most icon on the bar at the top, pressing A, navigating to <code>sd</code> and pressing A.</li>
  <li>Navigate to where your save file is located at on your SD card and select the file. The default location is usually in <code>/savegames/</code>.</li>
  <li>Navigate to "Install" and press A.</li>
  <li>Press A on OK to confirm your restoration.</li>
  <li>Close out of Save Manager GX by pressing the Home Button and then Wii Menu.</li>
  <li>Load up your game of choice. You should see your newly restored save!</li>
</ol>

### Miis {#miis}

#### Backing up {#backing-up_1}

<ol start="6">
  <li>Ensure the source is set to Mii. You can do this by going to the left most icon on the bar at the top, pressing A, navigating to <code>mii</code> and pressing A.</li>
  <li>Navigate to your Mii of choice and press A.</li>
  <li>Navigate to "Extract" and press A.</li>
  <li>Navigate to "Default" and press A.</li>
  <li>Press A on OK to confirm your back up.</li>
  <li>Do what you want with this back up!</li>
</ol>

#### Restoring {#restoring_1}

<ol start="6">
  <li>Ensure the source is set to SD. You can do this by going to the left most icon on the bar at the top, pressing A, navigating to <code>sd</code> and pressing A.</li>
  <li>Navigate to where your saved Mii's file is located at on your SD card and select the file. The default location is usually in <code>/savegames/</code>.</li>
  <li>Navigate to "Install" and press A.</li>
  <li>Press A on OK to confirm your restoration.</li>
  <li>Close out of Save Manager GX by pressing the Home Button and then Wii Menu.</li>
  <li>Load up the Mii Channel. You should see your newly restored Mii!</li>
</ol>

## Managing GameCube Saves {#managing-gamecube-saves}

<div class="admonition note">
  <p class="admonition-title">Why Not Nintendont?</p>
  <p>This guide will go over how to extract/restore saves from/to a Memory Card on your Wii. Nintendont's emulated memory card data can be found readily on your SD card in <code>/saves/</code>.</p>
</div>
<ol>
  <li>Open the Homebrew Channel on your Wii.</li>
  <li>Load up Homebrew Browser.</li>
  <li>In the Utilities section, navigate to GCMM and install it.</li>
  <li>Close out of Homebrew Browser. You should be back in the Homebrew menu.</li>
  <li>Load up GCMM.</li>
</ol>

### Backing up {#backing-up_2}

<ol start="6">
  <li>Select "Wii Front SD slot"</li>
  <li>On your Wiimote, press B and - to enter raw backup mode. If you're using a GameCube controller, press L and Y.</li>
  <li>Select the slot that has your memory card using the appropriate button (A or B).</li>
  <li>Back up as you'd like.</li>
  <li>When the dump is/are complete, press B.</li>
  <li>Press Home (Wiimote) or Start (GameCube controller) to exit GCMM.</li>
  <li>Do what you want with this back up! It is stored in the <code>/MCBACKUP/</code> folder on your SD card.</li>
</ol>

### Restoring {#restoring_2}

<ol start="6">
  <li>Select "Wii Front SD slot"</li>
  <li>On your Wiimote, press B and + to enter raw restore mode. If you're using a GameCube controller, press L and X.</li>
  <li>Select the slot that has your memory card using the appropriate button (A or B).</li>
  <li>Restore whichever save you'd like from where it's located on your SD card.</li>
  <li>When the restoration is complete, press B.</li>
  <li>Press Home (Wiimote) or Start (GameCube controller) to exit GCMM.</li>
  <li>Happy gaming!</li>
</ol>

## Dumping Wii/GameCube Discs {#dumping-wiigamecube-discs}

<ol>
  <li>Insert your game disc into the slot.</li>
  <li>Open the Homebrew Channel on your Wii.</li>
  <li>Load up Homebrew Browser.</li>
  <li>In the Utilities section, navigate to CleanRip and install it.</li>
  <li>Close out of Homebrew Browser. You should be back in the Homebrew menu.</li>
  <li>Read the disclaimer and then press A if any pops up.</li>
  <li>Press A to enable checksum verification.</li>
  <li>You'll be prompted to select a device type. We are using an SD card, so navigate to "Front SD" and press A.</li>
  <li>Your SD card should already be inserted, so press A to continue.</li>
  <li>Navigate to the "FAT" filesystem type and press A.</li>
  <li>Navigate to "Yes" if prompted to download <a class="external" href="http://redump.org/" rel="" target="_blank">redump.org</a> DAT files. Press A. </li>
  <li>Your disc should already be inserted. Press A. </li>
  <li>You may be prompted if your disc is an unlicensed datel disc. Just select "No". </li>
  <li>(<strong>WII ONLY</strong>) Set <code>Dump Size</code> to Auto, <code>Chunk Size</code> to Max, and <code>New device per chunk</code> to No. Press A.<ul>
      <li>If you're dumping a GameCube Disc, just press A.</li>
    </ul>
  </li>
  <li>The disc should now be dumping! This will take a while, especially for Wii games which can take upwards of 30 minutes sometimes. Go for a quick walk in the meantime. :)</li>
  <li>Once it's done, close out of CleanRip by pressing B. You should be in the Homebrew Channel now.</li>
  <li>Turn off your Wii.</li>
  <li>Take out the SD Card.</li>
  <li>Insert your Wii's SD card into your computer.</li>
</ol>
<div class="admonition warning">
  <p class="admonition-title">Divergence</p>
  <p>From now until the end of these instructions, there will be a divergence in how to use these backups. I will make subsections in the table of contents accordingly. You can click the subsection you want from this warning.</p>
  <ol>
    <li><a href="../wii/#step-20-wii-disc-to-usb-loader-gx">Wii Disc to USB Loader GX</a></li>
    <li><a href="../wii/#step-20-wii-disc-to-rom-format">Wii Disc to ROM Format</a></li>
    <li><a href="../wii/#step-20-gamecube-disc-to-usb-loader-gx">GameCube Disc to USB Loader GX</a></li>
    <li><a href="../wii/#step-20-gamecube-disc-to-rom-format">GameCube Disc to ROM Format</a></li>
  </ol>
</div>

### Step 20+: Wii Disc to USB Loader GX {#step-20-wii-disc-to-usb-loader-gx}

<ol start="20">
  <li>Your dump should be on the root of your SD card in 2 parts. For example, <em>House of the Dead Overkill</em>'s dump will have 2 files that look like <code>RHOE8P.part0.iso</code> and <code>RHOE8P.part1.iso</code>. Select these files and drag them to somewhere on your PC, as the SD's card FAT32 file format does not allow you to have files bigger than 4 GB at once on your SD card. Once this is done, you may delete the dumped files from your SD card as we will no longer need them.</li>
  <li class="mb-0 mb-ul-3">
    <p class="mb-0 mt-0">The instructions here vary for operating system. Look at what bullet point of this step is relevant to you.</p>
    <ul>
      <li><strong>Windows</strong>: Open the folder where you dragged your dumped files in File Explorer. In the Address Bar, type <code>cmd</code>. A Command Prompt window should have opened in the relevant folder. Copy/paste the following command into the Command Prompt: <br/>
        <div class="codeblock">
          <div class="clipboard">
            <div class="clippy" tabindex="0" value="copy /b *.part?.iso game.iso">
              <div class="clippy-icon">⎗</div>
              <div class="check-icon d-none cb-tooltip">✓<span class="cb-tooltiptext"></span></div>
            </div>
          </div>
          <table class="highlighttable"><tbody><tr><td class="linenos"><div class="linenodiv"><pre><span class="normal"><a href="#L-1-1">1</a></span></pre></div></td><td class="code"><div class="highlight"><pre><span></span><span id="L-1-1"><a id="L-1-1" name="L-1-1"></a>copy /b *.part?.iso game.iso
</span></pre></div>
          </td></tr></tbody></table>
        </div>
      </li>
      <li><strong>MacOS/Linux</strong>: Open the folder where you dragged your dumped files in Finder/whatever file browser you use. Right click the window and click on "Open in Terminal". A Terminal window should have opened in the relevant folder. Copy/paste the following command into the Terminal: <br/>
        <div class="codeblock">
          <div class="clipboard">
            <div class="clippy" tabindex="0" value="cat `ls *.part?.iso | sort` &gt; game.iso">
              <div class="clippy-icon">⎗</div>
              <div class="check-icon d-none cb-tooltip">✓<span class="cb-tooltiptext"></span></div>
            </div>
          </div>
          <table class="highlighttable"><tbody><tr><td class="linenos"><div class="linenodiv"><pre><span class="normal"><a href="#L-2-1">1</a></span></pre></div></td><td class="code"><div class="highlight"><pre><span></span><span id="L-2-1"><a id="L-2-1" name="L-2-1"></a>cat <span class="sb">`</span>ls *.part?.iso <span class="p">|</span> sort<span class="sb">`</span> &gt; game.iso
</span></pre></div>
          </td></tr></tbody></table>
        </div>
      </li>
    </ul>
    <p>Press Enter. Wait for this to finish, and when it's done close out of Command Prompt/Terminal. You may now delete the dumped files from your PC as well, as we no longer need them. (ie. <code>RHOE8P.part0.iso</code> and <code>RHOE8P.part1.iso</code>).</p>
  </li>
  <li>Follow the <a href="../wii/#pirating-wii-or-gamecube-games">Pirating Wii Games</a> guide from Step 8 onward, as the installation instructions are exactly the same!</li>
</ol>

### Step 20+: Wii Disc to ROM Format {#step-20-wii-disc-to-rom-format}

<div class="admonition warning">
  <p class="admonition-title">Do You Have Save Data?</p>
  <p>Since we will be transferring between a Wii to Dolphin Emulator, save files will not persist as game save data was stored on the Wii's NAND and NOT on the game disc itself. If you have relevant save data, please be sure to follow <a href="../wii/#managing-wii-saves-miis">these steps</a> to back up your saves! Additionally, step 29 onward is meant for importing this save to Dolphin emulator!</p>
</div>
<ol start="20">
  <li>Your dump should be on the root of your SD card in 2 parts. For example, <em>House of the Dead Overkill</em>'s dump will have 2 files that look like <code>RHOE8P.part0.iso</code> and <code>RHOE8P.part1.iso</code>. Select these files and drag them to somewhere on your PC, as the SD's card FAT32 file format does not allow you to have files bigger than 4 GB at once on your SD card. Once this is done, you may delete the dumped files from your SD card as we will no longer need them.</li>
  <li class="mb-0 mb-ul-3">
    <p class="mb-0 mt-0">The instructions here vary for operating system. Look at what bullet point of this step is relevant to you.</p>
    <ul>
      <li><strong>Windows</strong>: Open the folder where you dragged your dumped files in File Explorer. In the Address Bar, type <code>cmd</code>. A Command Prompt window should have opened in the relevant folder. Copy/paste the following command into the Command Prompt: <br/>
        <div class="codeblock">
          <div class="clipboard">
            <div class="clippy" tabindex="0" value="copy /b *.part?.iso game.iso">
              <div class="clippy-icon">⎗</div>
              <div class="check-icon d-none cb-tooltip">✓<span class="cb-tooltiptext"></span></div>
            </div>
          </div>
          <table class="highlighttable"><tbody><tr><td class="linenos"><div class="linenodiv"><pre><span class="normal"><a href="#L-3-1">1</a></span></pre></div></td><td class="code"><div class="highlight"><pre><span></span><span id="L-3-1"><a id="L-3-1" name="L-3-1"></a>copy /b *.part?.iso game.iso
</span></pre></div>
          </td></tr></tbody></table>
        </div>
      </li>
      <li><strong>MacOS/Linux</strong>: Open the folder where you dragged your dumped files in Finder/whatever file browser you use. Right click the window and click on "Open in Terminal". A Terminal window should have opened in the relevant folder. Copy/paste the following command into the Terminal: <br/>
        <div class="codeblock">
          <div class="clipboard">
            <div class="clippy" tabindex="0" value="cat `ls *.part?.iso | sort` &gt; game.iso">
              <div class="clippy-icon">⎗</div>
              <div class="check-icon d-none cb-tooltip">✓<span class="cb-tooltiptext"></span></div>
            </div>
          </div>
          <table class="highlighttable"><tbody><tr><td class="linenos"><div class="linenodiv"><pre><span class="normal"><a href="#L-4-1">1</a></span></pre></div></td><td class="code"><div class="highlight"><pre><span></span><span id="L-4-1"><a id="L-4-1" name="L-4-1"></a>cat <span class="sb">`</span>ls *.part?.iso <span class="p">|</span> sort<span class="sb">`</span> &gt; game.iso
</span></pre></div>
          </td></tr></tbody></table>
        </div>
      </li>
    </ul>
    <p>Press Enter. Wait for this to finish, and when it's done close out of Command Prompt/Terminal. You may now delete the dumped files from your PC as well, as we no longer need them. (ie. <code>RHOE8P.part0.iso</code> and <code>RHOE8P.part1.iso</code>).</p>
  </li>
  <li>In our lovely Discord server, there are instructions tied to our Discord bot about how to set up the Dolphin emulator. All you need to do is follow the instructions to bot gives you when entering the command "!w emulation wii". Just ensure that the path you mention in step 5 of <em>that</em> instruction set is the same path where your <code>game.iso</code> is located.</li>
  <li>In the Dolphin UI, right click your game. In the dropdown menu left click on <code>Convert File...</code>.</li>
  <li>In the first dropdown, choose "RVZ" as the Format.</li>
  <li>Click on Convert.</li>
  <li>A file explorer window will show up. Save the new <code>.rvz</code> file to the same place as your <code>game.iso</code>, then click on Save.</li>
  <li>Once the conversion is finished, click OK. If you'd like, you can open a file explorer window to delete the <code>game.iso</code> file where it is located, as we no longer need it.</li>
  <li>In the Dolphin UI, click "Refresh". Your <code>.rvz</code> format ROM should be visible in Dolphin!</li>
</ol>
<div class="admonition note">
  <p class="admonition-title">Are You Done?</p>
  <p>The final few steps here are for if you have backed up Wii save data you'd like to import. <strong>If you don't have that, you're done! You may (safely) eject your SD card, insert it back into your Wii, and have fun again!</strong> If you do, however, follow along just for a little longer.</p>
</div>
<ol start="29">
  <li>In the Dolphin UI, click <code>Tools</code> -&gt; <code>Import Wii Save...</code>.</li>
  <li>Navigate to where the <code>.bin</code> of your save file of choice is saved on your SD card. This is by default usually in <code>/savegames/</code>. Press Open.</li>
  <li>Click Yes on any popups that may appear. Do note that if you had existing save data with Dolphin, this will be overwritten</li>
  <li>Click OK once your save data has successfully been imported.</li>
  <li>Double click on your game and enjoy!</li>
</ol>

### Step 20+: GameCube Disc to USB Loader GX {#step-20-gamecube-disc-to-usb-loader-gx}

<div class="admonition warning">
  <p class="admonition-title">Do You Have Save Data?</p>
  <p>If you already have a GameCube Memory Card and do not want Nintendont to use a virtual memory card save simply <strong>put it in a slot on your Wii, make sure in Nintendont settings "Memcard Emulation" is off, and ignore steps 24-26</strong>. Otherwise, this subsection assumes you have already backed up your Memory Card. If not, follow <a href="../wii/#managing-gamecube-saves-backing-up">these steps</a> to do so.</p>
</div>
<ol start="20">
  <li>Your dump should be on the root of your SD card as 1 <code>.iso</code> file. Select this file and drag it into the <code>games</code> folder., creating it if it doesn't already exist.</li>
  <li>Rename the dump to <code>game.iso</code>.</li>
  <li>Make a new folder inside of this <code>games</code> folder. Name that new folder the name of your game; this does not have to be hyper-specific. For example, you may have <code>/games/Super Smash Bros Melee/</code> and this will work.</li>
  <li>Drag that <code>game.iso</code> file into this new folder.</li>
  <li>Go back to the root of your SD card, and then to the <code>MCBACKUP</code> folder.</li>
  <li>Copy the <code>.raw</code> backup file from here, and then go back to the root of your SD card once more.</li>
  <li>Paste the backup file here and rename it to <code>ninmen.raw</code>.</li>
  <li>Safely eject your SD card from your PC.</li>
  <li>Insert your SD card back into your Wii.</li>
  <li>Turn on your Wii.</li>
  <li>Open the Homebrew Channel on your Wii.</li>
  <li>Open USB Loader GX.</li>
  <li>Once it is done initializing, press A to select SD as the source.</li>
  <li>You should see your game in the list. Navigate to it.</li>
  <li>Launch it. Happy Gaming!</li>
</ol>

### Step 20+: GameCube Disc to ROM Format {#step-20-gamecube-disc-to-rom-format}

<div class="admonition warning">
  <p class="admonition-title">Do You Have Save Data?</p>
  <p>Since we will be transferring between a GameCube Memory Card to Dolphin Emulator, save files will not persist as game save data was stored on the Wii's NAND and NOT on the game disc itself. If you have relevant save data, please be sure to follow <a href="../wii/#managing-gamecube-saves-backing-up">these steps</a> to back up your saves! Additionally, step 28 onward is meant for importing this save to Dolphin emulator!</p>
</div>
<ol start="20">
  <li>Your dump should be on the root of your SD card as 1 <code>.iso</code> file. Select this file and drag it to somewhere on your PC. Once this is done, you may delete the dumped file from your SD card as we will no longer need it.</li>
  <li>In our lovely Discord server, there are instructions tied to our Discord bot about how to set up the Dolphin emulator. All you need to do is follow the instructions to bot gives you when entering the command "!w emulation gamecube". Just ensure that the path you mention in step 5 of <em>that</em> instruction set is the same path where your <code>.iso</code> is located.</li>
  <li>In the Dolphin UI, right click your game. In the dropdown menu left click on <code>Convert File...</code>.</li>
  <li>In the first dropdown, choose "RVZ" as the Format.</li>
  <li>Click on Convert.</li>
  <li>A file explorer window will show up. Save the new <code>.rvz</code> file to the same place as your <code>.iso</code>, then click on Save.</li>
  <li>Once the conversion is finished, click OK. If you'd like, you can open a file explorer window to delete the <code>.iso</code> file where it is located, as we no longer need it.</li>
  <li>In the Dolphin UI, click "Refresh". Your <code>.rvz</code> format ROM should be visible in Dolphin!</li>
</ol>
<div class="admonition note">
  <p class="admonition-title">Are You Done?</p>
  <p>The final few steps here are for if you have backed up GameCube save data you'd like to import. <strong>If you don't have that, you're done! You may (safely) eject your SD card, insert it back into your Wii, and have fun again!</strong> If you do, however, follow along just for a little longer.</p>
</div>
<ol start="28">
  <li>In the Dolphin UI, click <code>Config</code> -&gt; <code>GameCube</code>. In the Device Settings section, make sure Slot A has "Memory Card" selected from its dropdown. Click Close afterward.</li>
  <li>In the Dolphin UI, click <code>Tools</code> -&gt; <code>Memory Card Manager...</code>.</li>
  <li>Click Open next to slot B.</li>
  <li>Navigate to the saves folder on your SD/USB, and open the .raw file named after the game ID of your game.</li>
  <li>Click Switch to B.</li>
  <li>Select the save you would like to copy and click "Copy to A".</li>
  <li>Click Close.</li>
  <li>Double click on your game and enjoy!</li>
</ol>

## Retro Gaming {#retro-gaming}

<p><strong><em>Coming Soon™...</em></strong></p>

## Using Cheats {#using-cheats}

<p><strong><em>Coming Soon™...</em></strong></p>

## Mods {#mods}

<p><strong><em>Coming Soon™...</em></strong></p>

## Theming {#theming}

<p>Want to make your Wii feel more personal? Here's a few ways you can theme your Wii! The guide will be split into the three places that support themes.</p>

### Home Menu {#home-menu}

<ol>
  <li>Open the Homebrew Channel on your Wii.</li>
  <li>Load up Homebrew Browser.</li>
  <li>In the Utilities section, navigate to csm-installer and install it.</li>
  <li>Close out of Homebrew Browser. You should be back in the Homebrew menu.</li>
  <li>Load up csm-installer.</li>
  <li>Automatically, the app should create a backup of your "base theme". This is your Wii's current unmodified Home Menu. Press A once finished.</li>
  <li>Navigate to "Return to Wii System Menu" and select it.</li>
  <li>Turn off your Wii.</li>
  <li>Take out the SD card.</li>
  <li>Insert your Wii's SD card into your computer.</li>
  <li>On the root of your SD card, create a <code>themes</code> folder if it doesn't already exist.</li>
  <li>On your computer go to <a class="external" href="https://www.wiithemer.org/" rel="" target="_blank">this website</a>.</li>
  <li>Click on the "channel" that looks like a penguin building a brick wall. It will give you a console brick warning, but by now you should know how to reverse a brick.</li>
  <li>From the "Select Theme :" dropdown, choose a theme you'd like.</li>
  <li>From the "Select System Menu Version :" dropdown, choose your system menu version, which should be 4.3.</li>
  <li>From the "Select System Region :" dropdown, choose your region code. (U for USA, E for Europe, J for Japan, K for Korea.).</li>
  <li>Click on "Build Theme". Once it's finished, click on the button that has a file name with a <code>.csm</code> extension. This is your theme's file.</li>
  <li>Drag and drop this <code>.csm</code> file to the <code>themes</code> folder of your SD card.</li>
  <li>Safely eject your SD card from your PC.</li>
  <li>Insert your SD card back into your Wii.</li>
  <li>Turn on your Wii.</li>
  <li>Open the Homebrew Channel on your Wii.</li>
  <li>Open csm-installer.</li>
  <li>Press A on "Install a theme".</li>
  <li>Navigate to the <code>.csm</code> file from earlier and select it. Wait for it to finish installing.</li>
  <li>Navigate to "Return to Wii System Menu" and select it.</li>
  <li>Revel in your artistic excellence!</li>
</ol>
<p>From now on, if you'd like to add more themes simply follow along from Step 8 onwards.</p>

### Homebrew Channel {#homebrew-channel}

<ol>
  <li>Turn off your Wii.</li>
  <li>Take out the SD card.</li>
  <li>Insert your Wii's SD card into your computer.</li>
  <li>On your computer go to <a class="external" href="https://wiibrew.org/wiki/Homebrew_Channel/Themes" rel="" target="_blank">this website</a>.</li>
  <li>Download a theme that you like. It should be a <code>.zip</code> file. Do not extract this yet!</li>
  <li>Drag and drop this <code>.zip</code> file to your <code>/apps/</code> folder on your SD card. Unpack this <code>.zip</code> file within the folder, and then delete the original <code>.zip</code> file.</li>
  <li>Safely eject your SD card from your PC.</li>
  <li>Insert your SD card back into your Wii.</li>
  <li>Turn on your Wii.</li>
  <li>Open the Homebrew Channel on your Wii.</li>
  <li>Open the newly created app in your Homebrew Channel. Your theme should be set up now!</li>
</ol>

### USB Loader GX {#usb-loader-gx}

<ol>
  <li>Turn off your Wii.</li>
  <li>Take out the SD card.</li>
  <li>Insert your Wii's SD card into your computer.</li>
  <li>On your computer go to <a class="external" href="https://gbatemp.net/threads/dark-wii-usb-loader-gx-themes.584493/" rel="" target="_blank">this website</a>.</li>
  <li>Download a theme that you like. It should be a <code>.zip</code> file. Do not extract this yet!</li>
  <li>Drag and drop this <code>.zip</code> file to your <code>/apps/usbloader_gx</code> folder on your SD card. Unpack this <code>.zip</code> file within the folder, and then delete the original <code>.zip</code> file.</li>
  <li>Safely eject your SD card from your PC.</li>
  <li>Insert your SD card back into your Wii.</li>
  <li>Turn on your Wii.</li>
  <li>Open the Homebrew Channel on your Wii.</li>
  <li>Open USB Loader GX.</li>
  <li>Go to the Settings menu, and then go to Theme Menu.</li>
  <li>Navigate to your theme and install it. Your theme should be set up now!</li>
</ol>

## FTPii (File Transfer Over Internet) {#ftpii-file-transfer-over-internet}

<div class="admonition info">
  <p class="admonition-title">What Is FTPii?</p>
  <p>What if you could wirelessly transfer files between your computer and Wii without having to constantly move its SD card in and out of your multiple systems at home? This is where FTPii comes in. It allows you to do exactly that. I would advise, however, only do this for files small in size, as file transfer through FTP can be rather slow.</p>
</div>
<ol>
  <li>Open the Homebrew Channel on your Wii.</li>
  <li>Load up Homebrew Browser.</li>
  <li>In the Utilities section, search for "FTPii" and install it.</li>
  <li>Once it's finished installing, press Home and return back to the Homebrew Channel.</li>
  <li>Open the FTPii application.</li>
  <li>The top of the screen should have an IP address and port number at the top. This will be in the format of <a class="external" href="http://xxx.xxx.xxx.xxx/" rel="" target="_blank">XXX.XXX.XXX.XXX</a>:(PORT). Keep note of it.</li>
  <li>Leave your Wii aside for now, but leave it on and visible near you.</li>
</ol>
<div class="admonition note">
  <p class="admonition-title">Divergence</p>
  <p>This section will now divide into 2 sections for instructions depending on your operating sytem.</p>
</div>

### For Windows/MacOS {#for-windowsmacos}

<ol start="8">
  <li>Go to <a class="external" href="https://cyberduck.io/download/" rel="" target="_blank">this website</a>.</li>
  <li>Download for your operating system.</li>
  <li>On Windows, run through the installer for the program and then open Cyberduck. On MacOS, unarchive the <code>.zip</code> file you downloaded using an unarchiver of your choice (the MacOS default one works just fine), drag and drop <code>Cyberduck.app</code> into your Applications pin in Finder, go to the Applications pin, right click on <code>Cyberduck.app</code>, select "Open", then confirm that you want to open the application.</li>
  <li>In Cyberduck, click "Open Connection" at the top.</li>
  <li>At the dropdown on the top, make sure "FTP (File Transfer Protocol)" is selected.</li>
  <li>In the text box for "Server", enter the IP address on your Wii.</li>
  <li>In the box for "Port", enter the port number on your Wii.</li>
  <li>Cyberduck will now connect to your Wii's files directly. Open a window in your file explorer from here.</li>
  <li>Use both Cyberduck and the window you just opened to do whatever dragging and dropping of files in and out of your SD card that you need to do. Note that because we are wirelessly transferring files here, files may take longer to transfer in and out of your system.</li>
  <li>Once finished, close out of Cyberduck. It may prompt you to pay money, in which case just click "Later". Cyberduck will always be free to you, and you paying money is only to support the developers.</li>
  <li>Back on your Wii, close out of FTPii.</li>
</ol>

### For Linux {#for-linux}

<ol start="8">
  <li>In your file explorer (in my case, Dolphin on my Steam Deck), right click on the file path at the top and make sure "Show file path" is selected.</li>
  <li>Click on the file path to open a textbox displaying the full file path.</li>
  <li>Press Ctrl+A to highlight the entire thing and then Backspace to delete it all.</li>
  <li>Enter the following into the file path bar: <code>ftp://(the ip address):(the port number)</code>. You should then almost instantly be able to access the files on your SD card.</li>
  <li>Open a new tab or window of Dolphin. Use both of these tabs/windows to do whatever dragging and dropping of files in and out of your SD card that you need to do. Note that because we are wirelessly transferring files here, files may take longer to transfer in and out of your system.</li>
  <li>Once finished, close out of the tab/window that contains your Wii's files and the other tab/window containing files on your Linux computer.</li>
  <li>Back on your Wii, close out of FTPii.</li>
</ol>

## Ordering Pizza??? {#ordering-pizza}

<p>Yes, you can order pizza through your Wii. I mean, this is seriously nothing more than a novelty that loses its charm once you even do it once, but it's cool that you can do this in the first place? This stems from a Japan exclusive Wii channel called "The Demae Channel" that let you order food from local restaurants through your Wii to your front door. You would pay through cash on delivery. Using WiiLink's services in 2025, <strong>which you should have set up if you followed the hacks guide</strong>, you can order pizza from Domino's if you are in either the US or Canada! I wouldn't really recommend it, but I'm not your parent so if you want I won't stop you...</p>
<div class="admonition warning">
  <p class="admonition-title">Assumptions Made!</p>
  <p><strong>This guide assumes you have already set up WiiLink on your Wii</strong>. The instructions should have been given to you through the Wii Hacks Guide, but you can find them again <a class="external" href="https://wiilink.ca/guide/wii/" rel="" target="_blank">here</a>. You should also have all the WiiLink patched channels on your Home Menu too.</p>
</div>
<ol>
  <li>On your computer, create a WiiLink account at <a class="external" href="http://accounts.wiilink.ca/" rel="" target="_blank">accounts.wiilink.ca</a>.</li>
  <li>Turn on your Wii.</li>
  <li>Open the Homebrew Channel.</li>
  <li>Open the Homebrew Browser.</li>
  <li>In the Utilities section, navigate to the WiiLink Account Linker app and install it.</li>
  <li>Once that's finished, close out of the Homebrew Browser. You should be back in the Homebrew Channel now.</li>
  <li>Open the WiiLink Account Linker.</li>
  <li>A code should be displayed on screen. Take a picture or mental note of that code, and input it at <a class="external" href="http://sso.riiconnect24.net/device" rel="" target="_blank">sso.riiconnect24.net/device</a> on your computer. This assumes you're still signed in.</li>
  <li>Once this is successful, go back to <a class="external" href="http://accounts.wiilink.ca/" rel="" target="_blank">accounts.wiilink.ca</a>. Click on Food Delivery Settings.</li>
  <li>In the dropdown box, select the number associated with your Wii.</li>
  <li>Click on "Enable Dominos Ordering". You should be done with your computer now.</li>
  <li>Back on your Wii, close out of the WiiLink Account Linker app, and then close out of the Homebrew Channel.</li>
  <li>On the Wii's Home Menu, open the Food Channel.</li>
  <li>If you have not previously set your address information, a prompt telling you to set it will appear. Press the <code>Address Info</code> button. Otherwise, select the <code>Change Address Information</code> button in the main menu.</li>
  <li>Now you are in the Address Information menu. Press the arrows to traverse screens. Here you will enter your data. Make sure this data is accurate!</li>
  <li>When you are finished, select the <code>Done</code> button and then <code>Demae</code>.</li>
  <li>Follow the on-screen instructions, then select <code>Order</code> in the main menu.</li>
  <li>You will now be prompted to select your region. Be sure to select your country correctly, as if not restaurants will fail to load. You will then be prompted to select your state/province, then city.</li>
  <li>Select the <code>Pizza</code> button. This will load all the restaurants in your area. The first restaurant in the list is the one closest to you.</li>
  <li>Select <code>See Menu</code> to list the different menu categories. Select the category you would like, then select a food item. In the item screen, you can add toppings and in/decrease quantity.</li>
  <li>After adding a food item, you will be brought to the basket. To add a food item, scroll to the bottom and select <code>Add Order</code>. To proceed to checkout, select <code>Next</code>.</li>
  <li>Double check your order before placing it. When you are ready, select the big green <code>Order</code> button.</li>
  <li>If no error appeared, your order was placed successfully! To track your order, simply visit the Domino’s Tracker for your region and enter the phone number you entered in the Address Information menu.</li>
</ol>
<p>Remember, this is cash on delivery only! Be sure to have some cash when the driver shows up at your doorstep. Additionally, I think ordering online through your smartphone is probably cheaper than doing this, but again I won't stop you...</p>
<p>If you'd like to order again, simply skip steps 1-12.</p>
