<article>
<div><h1 id="rip-bozotendo-3ds">RIP Bozotendo, 3DS</h1>
<div class="admonition warning">
<p class="admonition-title">Important Warning</p>
<p>Until I say it isn't, <strong>this megathread will continually be in a state of WIP</strong>! I am continually working to add things to here that may be pertinent to us. If you want information on something, please let me know. I will try my best to update this thread as needed or as I come along certain information.</p>
</div>
<h2 id="table-of-contents-you-are-here">Table of Contents (You are here)</h2>
<div class="toc">
<ol>
<li><a href="#table-of-contents-you-are-here">Table of Contents (You are here)</a></li>
<li><a href="#disclaimers">Disclaimers</a></li>
<li><a href="#formatting-your-sd-card-assuming-you-have-a-64-gb-sd-card">Formatting your SD Card (Assuming You Have a 64+ GB SD Card)</a><ol>
<li><a href="#windows">Windows</a></li>
<li><a href="#linux">Linux</a></li>
<li><a href="#macos">MacOS</a></li>
</ol>
</li>
<li><a href="#3ds-hacks-guide">3DS Hacks Guide</a></li>
<li><a href="#updating-luma3ds">Updating Luma3DS</a></li>
<li><a href="#pirating-gamesdlcupdatesofficial-themes">Pirating Games/DLC/Updates/(Official) Themes</a><ol>
<li><a href="#prerequisite-for-ds-games-installing-twilightmenu">(Prerequisite for DS Games) Installing TwiLightMenu++</a></li>
<li><a href="#through-hshop">Through hShop</a><ol>
<li><a href="#for-3ds-games">For 3DS Games</a></li>
<li><a href="#for-ds-games">For DS Games</a></li>
</ol>
</li>
<li><a href="#through-3hs">Through 3hs</a><ol>
<li><a href="#optional-theming-3hs">(Optional) Theming 3hs</a></li>
</ol>
</li>
<li><a href="#optional-making-ds-games-show-on-home-menu">(Optional) Making DS Games Show On Home Menu</a></li>
</ol>
</li>
<li><a href="#dumping-3ds-games">Dumping 3DS Games</a><ol>
<li><a href="#from-cartridge-to-home-menu">From Cartridge To Home Menu</a></li>
<li><a href="#to-rom-format">To ROM Format</a><ol>
<li><a href="#from-cartridge">From Cartridge</a></li>
<li><a href="#from-home-menu">From Home Menu</a></li>
</ol>
</li>
</ol>
</li>
<li><a href="#dumping-ds-cartridges">Dumping DS Cartridges</a></li>
<li><a href="#virtual-console-injects-for-retro-games">Virtual Console Injects (For Retro Games)</a><ol>
<li><a href="#other-ways-to-play-retro-games">Other Ways To Play Retro Games</a><ol>
<li><a href="#gameboy-color">GameBoy (Color)</a></li>
<li><a href="#gameboy-advance">GameBoy Advance</a></li>
<li><a href="#nintendo-entertainment-system-nes">Nintendo Entertainment System (NES)</a></li>
<li><a href="#super-nintendo-entertainment-system-snes">Super Nintendo Entertainment System (SNES)</a></li>
<li><a href="#sony-playstation">Sony PlayStation</a></li>
<li><a href="#nintendo-64">Nintendo 64</a></li>
<li><a href="#virtualboy">VirtualBoy</a></li>
</ol>
</li>
</ol>
</li>
<li><a href="#going-online-in-3ds-games">Going Online In 3DS Games</a></li>
<li><a href="#going-online-in-ds-games">Going Online In DS Games</a><ol>
<li><a href="#dsi-enhanced-games">DSi Enhanced Games</a></li>
<li><a href="#non-dsi-enhanced-games">Non-DSi Enhanced Games</a><ol>
<li><a href="#a-password-less-hotspot-from-an-android-phone">A Password-less Hotspot From An Android Phone</a></li>
<li><a href="#using-the-melonds-emulator">Using The melonDS Emulator</a></li>
<li><a href="#using-a-portable-router">Using A Portable Router</a></li>
</ol>
</li>
</ol>
</li>
<li><a href="#using-cheats">Using Cheats</a><ol>
<li><a href="#3ds-games">3DS Games</a></li>
<li><a href="#ds-games">DS Games</a></li>
</ol>
</li>
<li><a href="#installing-unofficial-themes">Installing Unofficial Themes</a><ol>
<li><a href="#optional-mix-matching-music">(Optional) Mix-Matching Music</a></li>
<li><a href="#optional-shuffling-themes">(Optional) Shuffling Themes</a></li>
</ol>
</li>
<li><a href="#installing-custom-badges">Installing Custom Badges</a></li>
<li><a href="#mods-generally-speaking">Mods (Generally Speaking)</a><ol>
<li><a href="#majoras-mask-3d-restoration-mod">Majora's Mask 3D Restoration Mod</a></li>
</ol>
</li>
<li><a href="#streaming-3ds-games-to-azahar-emulator">Streaming 3DS Games To Azahar Emulator</a></li>
<li><a href="#ftpd-file-transfer-over-internet">FTPD (File Transfer Over Internet)</a><ol>
<li><a href="#for-windowsmacos">For Windows/MacOS</a></li>
<li><a href="#for-linux">For Linux</a></li>
</ol>
</li>
<li><a href="#using-external-controllers">Using External Controllers</a></li>
<li><a href="#patching-dsi-firmware">Patching DS(i) Firmware</a></li>
</ol>
</div>
<h2 id="disclaimers">Disclaimers</h2>
<ul>
<li>Please know that there will be some proper terminology to understand! The word "root" may come up a lot in discussion regarding the file structure of your SD card, which means when you are currently not in any folder on your SD card. <ul>
<li>Additionally, you may see terms like "FBI" and "Universal Updater", which are apps installed after hacking your 3DS. This "3DS" chapter of this megathread is intended to be read sequentially, so you may come across terms you may not quite understand if you aren't reading in the proper order.</li>
</ul>
</li>
<li>Hopefully, your 3DS is of the "New" variety, because you'll get the most juice out of it. This seems like a no-brainer, but if you really care about stuff like PS1 emulation on the 3DS then it only runs on the "New" models.<ul>
<li>Additionally, if you have a "New" model 3DS, please know that they run on microSD cards. The "Old" model 3DS family runs on bigger sized SD cards. If you plan to buy a new SD card for this project (you should, as the stock SD card is too small), please plan accordingly. <strong>This megathread will from here on out refer to your storage card as an "SD card", regardless of how big or small your's is in physical size</strong>.</li>
</ul>
</li>
<li>As for SD card size, technically, the 3DS only supports SD cards up to 32 GB. HOWEVER, you can format your SD card on your computer so that it actually works with your system. The correct format is FAT32, and this megathread will get into how to format it to such in a bit.<ul>
<li>I would recommend either getting a 64 or 128 GB SD card, as that's all you'll realistically need and any more than that might just lag the system due to its limited strength.</li>
</ul>
</li>
<li>Everything that is mentioned here can also be applied to a 2DS variant model, but for simplicity's sake I will refer to both 3DS variants and 2DS variants as simply just the 3DS.</li>
</ul>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="formatting-your-sd-card-assuming-you-have-a-64-gb-sd-card">Formatting your SD Card (Assuming You Have a 64+ GB SD Card)</h2>
<h3 id="windows">Windows</h3>
<ol>
<li>Go to <a class="external" href="http://ridgecrop.co.uk/index.htm?guiformat.htm" rel="" target="_blank">this website</a>.</li>
<li>The website generally looks a bit old, but just click the giant image of the formatter and it will install guiformat.exe</li>
<li>Insert your old SD card into your computer, the one that's in your 3DS currently before upgrading it.<ul>
<li><em>Make sure your 3DS is turned off before taking it out of your system</em>!</li>
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
<li>Eject your new SD card from your computer and insert it into your 3DS.</li>
<li>Turn your 3DS on. If your system boots correctly, you may now throw away your old SD card. Otherwise, repeat this process from step 3 until it works.</li>
</ol>
<h3 id="linux">Linux</h3>
<ol>
<li>Using your distro's package manager (<code>apt-get</code>, <code>pacman</code>, or <code>flatpak</code>, to name a few), install GParted. This can be done by opening a Terminal window and installing as outlined by the distro's documentation.</li>
<li>Insert your old SD card into your computer, the one that's in your 3DS currently before upgrading it.<ul>
<li><em>Make sure your 3DS is turned off before taking it out of your system</em>!</li>
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
<li>Eject your new SD card from your computer and insert it into your 3DS.</li>
<li>Turn your 3DS on. If your system boots correctly, you may now throw away your old SD card. Otherwise, repeat this process from step 2 until it works.</li>
</ol>
<h3 id="macos">MacOS</h3>
<ol>
<li>Insert your old SD card into your computer, the one that's in your 3DS currently before upgrading it.<ul>
<li><em>Make sure your 3DS is turned off before taking it out of your system</em>!</li>
</ul>
</li>
<li>Take anything and everything in that SD card and put it somewhere on your computer you'd remember. This is <strong>CRUCIAL</strong> as formatting your SD card wipes everything. Make sure you also don't play around with the locations of every file inside the folders, alas it should just be dragging and dropping them somewhere.</li>
<li>Eject your old SD card from your computer. Do not throw it out just yet.</li>
<li>Insert your new SD card into your computer now.</li>
<li>Open a Terminal window on your Mac. </li>
<li>Enter <code>diskutil list</code>. A bunch of seemingly-gibberish will show up, however, your SD card will follow the format of <code>/dev/diskX</code> on the list of disks, along with the "name" of the SD card showing up somewhere in its respective section</li>
<li>Enter <code>sudo diskutil eraseDisk FAT32 (name) MBRFormat /dev/diskX</code>. Make sure you change X to the disk number you got earler, and change (name) with the name of your SD card. You will be prompted to enter your admin password, so please do so.</li>
<li>Once it is finished, drag and drop the contents of your old SD card into the newly formatted SD card.</li>
<li>Eject your new SD card from your computer and insert it into your 3DS.</li>
<li>Turn your 3DS on. If your system boots correctly, you may now throw away your old SD card. Otherwise, repeat this process from step 1 until it works.</li>
</ol>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="3ds-hacks-guide">3DS Hacks Guide</h2>
<div class="admonition info">
<p><a class="external" href="https://3ds.hacks.guide/" rel="" target="_blank">https://3ds.hacks.guide/</a></p>
</div>
<p>This website will continuously stay up to date with the latest information on how to hack your 3DS.</p>
<div class="admonition danger">
<p class="admonition-title">AVOID AT ALL COSTS</p>
<p>Do <strong>NOT</strong>  attempt to follow video guides on how to hack your 3DS! The written guide linked above is continuously being updated, and it could be even a matter of days until a video guide goes outdated as they all follow what they see on this exact guide. The instructions on the written guide are easy enough to follow along to!</p>
</div>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="updating-luma3ds">Updating Luma3DS</h2>
<div class="admonition info">
<p class="admonition-title">Please Read!</p>
<p>Luma3DS is the name of the custom OS you install on your 3DS after hacking it. However, it does not have anything to do with the system version that is displayed in your System Settings application. By updating Luma3DS, you are <strong>NOT</strong> updating your system's firmware. You are simply updating the tool that allows for unsigned homebrew to run on your system in the first place, allowing for less buggier experiences running homebrew. In fact, some newer homebrew require the use of an updated version of Luma3DS.</p>
</div>
<ol>
<li>Open Universal Updater from your Home Menu.</li>
<li>Search for "Luma3DS". It should look like a light blue Luma from Super Mario Galaxy.</li>
<li>Download the <code>boot.firm</code> file.</li>
</ol>
<div class="admonition danger">
<p>Do <strong><em>NOT</em></strong> download the nightly version unless you are willing to work around potential bugs! It may give you access to features early, but you'd have to update it every night and these nightly releases aren't exactly bug tested. It's best to avoid unless you know what you are doing!</p>
</div>
<ol start="4">
<li>Once that's finished, press Start to exit the Universal Updater.</li>
<li>Turn off your 3DS.</li>
<li>Turn your 3DS back on, but this time press and hold Select before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.</li>
<li>You should now see the Luma menu. Note that there is a version number at the top. It should be higher than what it originally was.</li>
<li>Press Start to resume the normal boot process.</li>
</ol>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="pirating-gamesdlcupdatesofficial-themes">Pirating Games/DLC/Updates/(Official) Themes</h2>
<div class="admonition info">
<p class="admonition-title">About hShop/3hs</p>
<p>hShop is an archive of most of all 3DS and (as of November 2026) DS content that was available. hShop provides their service for absolutely zero cost to the end user. They do provide a standalone app called 3hs, which eliminates the need for a computer when downloading their content. However, there are some drawbacks to that such as needing your 3DS to be on a stable internet connection when the 3DS just does not have proper Wi-Fi drivers compared to a proper computer in today's age (meaning slower download times from 3hs). This section of the megathread tells you how to download content from this archive irrespective of which method you prefer.</p>
</div>
<div class="admonition warning">
<p class="admonition-title">Branching Pathways</p>
<p>Due to the nature of the platform we will be using now following 2 respective worlds of content, the pathways below will branch out based on the kind of content you will be looking at. I have formatted the guide accordingly. <strong>HOWEVER</strong>, if you are pirating a DS game, you will need a tool called TwiLightMenu++ installed. I have also attached instructions for that here as well.</p>
</div>
<h3 id="prerequisite-for-ds-games-installing-twilightmenu">(Prerequisite for DS Games) Installing TwiLightMenu++</h3>
<div class="admonition info">
<p class="admonition-title">What Is This?</p>
<p>TwiLightMenu++ is a piece of homebrew that acts as a frontend launcher for another piece of homebrew called ndsBootstrap, which allows you to run ROMs of DS games on a (3)DS family system utilizing the native hardware rather than emulation. If you install the former, you will not need to install the latter, since it will bundle ndsBootstrap with the program. It tries to mimic the feel of the Home Menu of a DSi, so if you have/had one of those, you'll feel very familiar with it already! It should also go without saying that if you already have this installed, you will not need to reinstall it unless you want to update the program.</p>
</div>
<ol>
<li>Open Universal Updater from your Home Menu.</li>
<li>Search for "TwiLightMenu++". The icon should look like "TM" with 2 plusses below it.</li>
<li>Download <code>TwiLightMenu++</code>. If you'd like, you can also download any of the other addons the install provides, though it won't be necesary for this guide.</li>
</ol>
<div class="admonition danger">
<p>Do <em>NOT</em> install the nightly version, for the same reasons as you wouldn't install the nightly Luma3DS version. </p>
</div>
<div class="admonition warning">
<p>It may ask you to extract a <code>roms</code> folder. Since this is a first install, this is recommended for new users.</p>
</div>
<ol start="4">
<li>On your Home Menu, open TwiLightMenu++.</li>
<li>After some time (be patient), it will ask you for a language. Select the language you want.</li>
<li>Next, it will ask you for a region. Choose your region of choice.</li>
<li>Be patient as the application will now initialize everything. Once it's finished, you should see a bunch of folders.</li>
<li>Navigate to the <code>nds</code> folder and press A to select it</li>
<li>Exit out of TwiLightMenu++ by pressing the Home button and then A.</li>
</ol>
<h3 id="through-hshop">Through hShop</h3>
<p>Use this method if you can't connect your 3DS to the internet!</p>
<ol>
<li>Go to <a class="external" href="https://hshop.erista.me/" rel="" target="_blank">this website</a>.</li>
<li>Search for whatever you want on their website.</li>
<li>Click on "Direct Download (.cia)" or "Direct Download (.nds)".</li>
<li>Turn off your 3DS.</li>
<li>Take out its SD card and insert it into your computer.</li>
</ol>
<h4 id="for-3ds-games">For 3DS Games</h4>
<ol start="6">
<li>Take the <code>.cia</code> file that you downloaded from hShop and drag it into the <code>cias</code> folder that you should have made when hacking your 3DS.<ul>
<li>If this <code>cias</code> folder does not exist, please make one in the root of your SD card.</li>
</ul>
</li>
<li>Take your SD card out of your PC.</li>
</ol>
<div class="admonition warning">
<p>Make sure you do it safely by manually clicking eject on the file explorer, as we do not want to risk corrupting your game file!</p>
</div>
<ol start="8">
<li>Put your SD card back in your 3DS and turn it back on.</li>
<li>Open FBI from your Home Menu.</li>
<li>In FBI, select "SD".</li>
<li>Navigate to your <code>cias</code> folder.</li>
<li>Select "&lt;current directory&gt;".</li>
<li>Select "Install and delete all CIAs".</li>
<li>Once your game is finished installing, press B as much as you can to back out to FBI's main menu. Press Start after that.</li>
<li>Your game should now appear in the Home Menu as a "gift". Themes that you download will <em>not</em> automatically be installed, rather an installer will appear on the Home Menu which when ran once will uninstall itself while downloading the theme for use with Anemone3DS. This theme will now be "unofficial" to your system, at which point you can follow steps 7-10 of my section on installing unofficial themes found later in this megathread.</li>
</ol>
<div class="admonition warning">
<p class="admonition-title">Games Crashing?</p>
<p><strong>If your game works from here, you're done</strong>! However, some games (for example, Rhythm Heaven Megamix) may require you to download a seed for them to work otherwise the console will crash. hShop will tell you whether or not the seed is needed. The following steps will detail how to import that seed and for it to work with your 3DS. Do be warned, however, that if you've used 3hs before (outlined in the next section), you may not need to use these steps.</p>
</div>
<div class="admonition danger">
<p class="admonition-title">Make Sure To Do This!</p>
<p>If you are on Pretendo servers (instructions on how to do that are found later), make sure to switch back to Nintendo servers before doing this!</p>
</div>
<ol start="16">
<li>Back on your computer, re-open the page for the game you downloaded from hShop if it isn't open already.</li>
<li>Click on "Download seed for FBI".</li>
</ol>
<div class="admonition danger">
<p class="admonition-title">Do NOT!</p>
<p>Do <strong><em>NOT</em></strong> change the name of the file for the seed that you just downloaded! This will mess things up come time for use with your 3DS!</p>
</div>
<ol start="18">
<li>Turn off your 3DS.</li>
<li>Take out its SD card and insert it into your computer.</li>
<li>Take the <code>.dat</code> file that you downloaded from hShop and drag it into the <code>/fbi/seed</code> folder that you should have made when hacking your 3DS.<ul>
<li>If this <code>seed</code> folder does not exist, please make one in the <code>fbi</code> folder of your SD card.</li>
</ul>
</li>
<li>Take your SD card out of your PC.</li>
<li>Put your SD card back in your 3DS and turn it back on.</li>
<li>Open FBI from your Home Menu.</li>
<li>In FBI, select "Titles".</li>
<li>Navigate to the game you had installed prior and select it.</li>
<li>Navigate to "Import Seed" and select it.</li>
<li>Confirm the selection.</li>
<li>Press A once the importing has finished. This process is very quick!</li>
<li>Press B and then Start to exit out of FBI.</li>
<li>Launch your game!</li>
</ol>
<h4 id="for-ds-games">For DS Games</h4>
<ol start="6">
<li>Take the <code>.nds</code> file that you downloaded from hShop and drag it into the <code>/roms/nds</code> folder that you should have made when installing TwiLightMenu++.</li>
<li>Take your SD card out of your PC.</li>
</ol>
<div class="admonition warning">
<p>Make sure you do it safely by manually clicking eject on the file explorer, as we do not want to risk corrupting your game file!</p>
</div>
<ol start="8">
<li>Put your SD card back in your 3DS and turn it back on.</li>
<li>Open TwiLightMenu++ from your Home Menu.</li>
<li>Navigate to your game.</li>
<li>Launch your game!</li>
</ol>
<h3 id="through-3hs">Through 3hs</h3>
<p>Use this method as much as possible! That is, whenever your 3DS is connected to the internet.</p>
<ol>
<li>Go to <a class="external" href="https://hshop.erista.me/3hs" rel="" target="_blank">this website</a>.</li>
<li>Click "Direct Download (CIA)"</li>
<li>Turn off your 3DS.</li>
<li>Take out its SD card and insert it into your computer.</li>
<li>Take the <code>.cia</code> file that you downloaded from hShop and drag it into the <code>cias</code> folder that you should have made when hacking your 3DS.<ul>
<li>If this <code>cias</code> folder does not exist, please make one in the root of your SD card.</li>
</ul>
</li>
<li>Take your SD card out of your PC.</li>
<li>Put your SD card back in your 3DS and turn it back on.</li>
<li>Open FBI from your Home Menu.</li>
<li>In FBI, select "SD".</li>
<li>Navigate to your <code>cias</code> folder.</li>
<li>Select "&lt;current directory&gt;".</li>
<li>Select "Install and delete all CIAs".</li>
<li>Once 3hs is finished installing, press B as much as you can to back out to FBI's main menu. Press Start after that.</li>
<li>3hs should now appear in the Home Menu as a "gift".</li>
<li>Open 3hs.</li>
<li>Search for whatever content you want and hit "Install".</li>
<li>Wait for the game to finish installing.</li>
<li>Press Start once the game is done installing to exit to the Home Menu.<ul>
<li>If your game is a 3DS title or theme, it should now appear in the Home Menu as a "gift". Themes that you download will <em>not</em> automatically be installed, rather an installer will appear on the Home Menu which when ran once will uninstall itself while downloading the theme for use with Anemone3DS. This theme will now be "unofficial" to your system, at which point you can follow steps 7-10 of my section on installing unofficial themes found later in this megathread.</li>
<li>If your game is a DS title, do not panic if you don't see it on your Home Menu right away. It should have downloaded directly to your <code>/roms/nds</code> folder for use with TwiLightMenu++. As such, it won't appear on your Home Menu and you'll have to launch it through TwiLightMenu++.</li>
</ul>
</li>
</ol>
<div class="admonition info">
<p><strong>If you prefer the hShop method, know that to get a new game you have to start from step 1 every time</strong>. However, <strong>if you choose the 3hs method, 3hs is a one-time install, meaning that to get a new game you have to start at step 15</strong>.</p>
</div>
<h4 id="optional-theming-3hs">(Optional) Theming 3hs</h4>
<p>Tired of the bland look of 3hs with no music playing in the background? I've scoured a few obscure places on the internet for you so that you can properly theme the app like how I did. There are other options out there, but for the purpose of everyone's sanity deteriorating by doomscrolling forum boards I won't be posting/promoting them.</p>
<p>You're going to need proper music and theme files. More traditional audio formats like <code>.mp3</code>, <code>.flac</code>, or <code>.wav</code> do not work with the 3hs app. Additionally, theming the 3hs app's interface doesn't take traditional formats for pictures like <code>.jpg</code>, <code>.png</code>, or <code>.gif</code>. You'd need to make them from scratch and/or convert existing <code>.wav</code> files into their format. Frankly, I think that's a waste of time for everyone involved. </p>
<ol>
<li>Download a track and a theme from the sections below. You can do this by clicking on the link for them and following the instructions I've listed below for each.</li>
</ol>
<div class="admonition note">
<p class="admonition-title"><strong><span class="underline-markdown" style="text-decoration-line:underline; text-decoration-color:inherit; text-decoration-style:solid; text-decoration-line:underline; text-decoration-thickness:3px;">Music</span></strong></p>
<ul>
<li><a class="external" href="https://fileditchfiles.me/file.php?f=/s22/hXdFSJzNaVZeWVjbjFpi.hwav" rel="" target="_blank">nintendo 3ds eshop music but it's lofi</a> <em>Click on "Download", then rename when saving. You can (and should) rename it to "nintendo 3ds eshop music but it's lofi" since this is the name of the <a class="external" href="https://soundcloud.com/roldyduarte/nintendo-3ds-eshop-music-but-its-lofi" rel="" target="_blank">original SoundCloud track</a> I ripped this from.</em></li>
<li><a class="external" href="https://www.dropbox.com/scl/fo/vd35sx4s3gy0fix5t8fba/AFwPdq5s6eZ21H08HROjmbA/Nintendo%20eShop%20Music%20-%202011%20June.hwav?rlkey=xi1lekujj8wut5np75bfj6c51&amp;e=2&amp;dl=0" rel="" target="_blank">June 2011 eShop Music</a> <em>Click on "Download", then click on "Continue with Download Only". This is the official eShop theme from June 2011, aka the launch of the 3DS.</em></li>
</ul>
</div>
<div class="admonition note">
<p class="admonition-title"><strong><span class="underline-markdown" style="text-decoration-line:underline; text-decoration-color:inherit; text-decoration-style:solid; text-decoration-line:underline; text-decoration-thickness:3px;">Themes</span></strong></p>
<ul>
<li><a class="external" href="https://my.opendesktop.org/s/JHKJpSAkqrDYfge/download?path=%2F&amp;files=heShopGreenNewEra%2Bbag.hstx" rel="" target="_blank">Theme I Use</a> <em>Just click on this link.</em></li>
<li><a class="external" href="https://my.opendesktop.org/s/JHKJpSAkqrDYfge/download?path=%2F&amp;files=heShop%2Bbag.hstx" rel="" target="_blank">Orange Variant Of Above</a> <em>Just click on this link.</em></li>
</ul>
</div>
<ol start="2">
<li>Turn off your 3DS.</li>
<li>Take out its SD card and insert it into your computer.</li>
<li>Inside the <code>/3ds/3hs</code> folder of your SD card, create 2 folders if they don't already exist: <code>music</code> and <code>themes</code>. </li>
<li>Take the <code>.hwav</code> file you downloaded and put it in <code>/3ds/3hs/music</code>.</li>
<li>Take the <code>.hstx</code> file you downloaded and put it in <code>/3ds/3hs/themes</code>.</li>
<li>Take your SD card out of your PC.</li>
</ol>
<div class="admonition warning">
<p>Make sure you do it safely by manually clicking eject on the file explorer, as we do not want to risk corrupting your files!</p>
</div>
<ol start="8">
<li>Put your SD card back in your 3DS and turn it back on.</li>
<li>Open 3hs from your Home Menu.</li>
<li>On the touch screen, with one of your fingers or your stylus tap on the icon that looks like 3 lines.</li>
<li>Navigate to the "Themes" section and select it.</li>
<li>Navigate to the theme you extracted earlier and select it.</li>
<li>Press B.</li>
<li>Navigate to the "Audio" section and select it.</li>
<li>On the touch screen, with one of your fingers or your stylus tap on the checkbox for "Repeat playlists and songs".</li>
<li>On the touch screen, with one of your fingers or your stylus tap on the button for "Manage playlists".</li>
<li>Press A to add a new playlist.</li>
<li>Name this playlist whatever you want, as the name of this playlist is unimportant.</li>
<li>Press A to enter the tracklisting for the new playlist you just created.</li>
<li>Press A to add a file.</li>
<li>Press A to add the track you extracted earlier.</li>
<li>Press B twice.</li>
<li>On the touch screen, with one of your fingers or your stylus tap on the textbox for "Default playlist".</li>
<li>Press A to select the playlist we created earlier.</li>
<li>On the touch screen, with one of your fingers or your stylus tap on the button for "playlist" under the <code>Select...</code> section.</li>
<li>Press A to select the playlist we created earlier.</li>
<li>On the touch screen, with one of your fingers or your stylus tap on the button on the bottom right to "Save" the configuration.</li>
<li>Press B twice.</li>
<li>Happy hShopping!</li>
</ol>
<h3 id="optional-making-ds-games-show-on-home-menu">(Optional) Making DS Games Show On Home Menu</h3>
<p>Tired of having to open TwiLightMenu++ before being able to play a DS game? Why not make it show up on your Home Menu instead as if it was a normal 3DS title? Well, you can do that by just following the steps below! Do note, however, that if you pirate a new DS game you'll have to repeat these steps again.</p>
<ol>
<li>Open Universal Updater from your Home Menu.</li>
<li>Search for "ndsForwarder". The icon should look like smiling cartoon narwhal.</li>
<li>Download <code>ndsForwarder.3dsx</code>.</li>
<li>Press Start to exit out of the Universal Updater.</li>
<li>Open The Homebrew Launcher.</li>
<li>Navigate to <code>NDS Forwarder Generator</code> and select it.</li>
<li>In this piece of homebrew, navigate to <code>/roms/nds/</code>.</li>
<li>Select <code>&lt; Install All nds &gt;</code>. Hit "Yes" to confirm.</li>
<li>Once finished, press Start to back out into The Homebrew Launcher.</li>
<li>Press the Home button to exit out into the Home Menu.</li>
<li>Your DS games should now appear on the Home Menu!</li>
</ol>
<div class="admonition warning">
<p class="admonition-title">Title Limit</p>
<p>Nintendo was very restrictive in designing how the 3DS works in regards to how many titles one can have installed on their system at any given time. The 3DS can have at maximum 300 titles installed at once, 40 of which can be DSiWare. The forwarders created by homebrew count towards your 40 DSiWare title limit, meaning that <strong>you can only have up to 40 DS games show up on your Home Menu at a time. You will need to play the rest through TwiLightMenu++.</strong></p>
</div>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="dumping-3ds-games">Dumping 3DS Games</h2>
<h3 id="from-cartridge-to-home-menu">From Cartridge To Home Menu</h3>
<div class="admonition info">
<p class="admonition-title">Regarding Fresh Game Data</p>
<p>If you are dumping a brand new game and/or do not have any important save data, only follow steps 1, 2, 8-18, and 24.</p>
</div>
<ol>
<li>Insert your cartridge of choice and open the game just for a quick second.</li>
<li>Close your game after a few seconds or so by pressing the Home button and closing the software.</li>
</ol>
<div class="admonition danger">
<p>Do <strong>NOT</strong> take out your game cartridge at this point in time!!!</p>
</div>
<ol start="3">
<li>Open Checkpoint.</li>
<li>Find your game tied to your cartridge in the app. Checkpoint should tell you if the game is installed on the SD card or from a cartridge.</li>
<li>Select your game and press L to backup your save data. Press A to confirm.</li>
<li>Name this backup whatever you wish, as it's not important.</li>
<li>Once that's finished, press Start to exit out into the Home Menu.</li>
<li>Turn off your system.</li>
<li>Turn your 3DS back on, but this time press and hold Start before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.</li>
<li>You should now be greeted with GodMode9. It may ask you to reset the RTC datetime offset. Do not change the provided date, just mash A until you get to the menu.</li>
<li>Navigate to <code>[C:] GAMECART ()</code></li>
<li>Select the <code>[game title ID].trim.3ds</code> file and choose "NCSD Image Options".</li>
<li>Select "Install Game Image".</li>
<li>Press A to unlock.</li>
<li>Follow the on-screen D-pad prompts.</li>
<li>Wait for your game to install, however long that takes.</li>
<li>Once that's done, back out as much as you can with the B button and then press Start. This will reboot the system like normal.</li>
</ol>
<div class="admonition note">
<p>After the system is done rebooting, it's now safe to remove the cartridge from your system.</p>
</div>
<ol start="18">
<li>The game you see on your Home Menu will be a blank copy of your game. No save data, just raw game data. Open this so that Checkpoint will be able to recognize it.</li>
<li>Close the game after a few seconds or so by pressing the Home button and closing the software.</li>
<li>Open Checkpoint.</li>
<li>Find your game tied to your SD card in the app and select it.</li>
<li>You should have the option to restore the save since it's the same game. Restore it, obviously, by pressing R and selecting the name of the backup you made earlier.</li>
<li>Once that's done, close Checkpoint by pressing Start.</li>
<li>If you need to, reinstall updates using hShop/3hs.</li>
</ol>
<div class="admonition warning">
<p class="admonition-title">Title Limit</p>
<p>Nintendo was very restrictive in designing how the 3DS works in regards to how many titles one can have installed on their system at any given time. The 3DS can have at maximum 300 titles installed at once, 40 of which can be DSiWare. This means that <strong>you can only have up to 300 games show up on your Home Menu at a time. The rest of your 3DS library needs to be physical cartridges or emulated externally.</strong></p>
</div>
<div class="admonition note">
<p class="admonition-title">Emulators</p>
<p>These dumps are compatible with an emulator of your choice! More information on how to use these games with an emulator later.</p>
</div>
<h3 id="to-rom-format">To ROM Format</h3>
<h4 id="from-cartridge">From Cartridge</h4>
<div class="admonition info">
<p class="admonition-title">Regarding Fresh Game Data</p>
<p>If you are dumping a brand new game and/or do not have any important save data, skip steps 1-7 and step 25.</p>
</div>
<ol>
<li>Insert your cartridge of choice and open the game just for a quick second.</li>
<li>Close your game after a few seconds or so by pressing the Home button and closing the software.</li>
</ol>
<div class="admonition danger">
<p>Do <strong>NOT</strong> take out your game cartridge at this point in time!!!</p>
</div>
<ol start="3">
<li>Open Checkpoint.</li>
<li>Find your game tied to your cartridge in the app. Checkpoint should tell you if the game is installed on the SD card or from a cartridge.</li>
<li>Select your game and press L to backup your save data. Press A to confirm.</li>
<li>Name this backup whatever you wish, as it's not important.</li>
<li>Once that's finished, press Start to exit out into the Home Menu.</li>
<li>Turn off your system.</li>
<li>Turn your 3DS back on, but this time press and hold Start before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.</li>
<li>You should now be greeted with GodMode9. It may ask you to reset the RTC datetime offset. Do not change the provided date, just mash A until you get to the menu.</li>
<li>Navigate to <code>[C:] GAMECART ()</code></li>
<li>Select the <code>[game title ID].trim.3ds</code> file and choose "NCSD Image Options".</li>
<li>Wait for your ROM to properly dump.</li>
<li>Once that's done, press B to back out to the main menu.</li>
<li>Select <code>[0:] SDCARD</code>.</li>
<li>Navigate to <code>gm9</code> and select it.</li>
<li>Navigate to <code>out</code> and select it.</li>
<li>Navigate to the <code>.cia</code> file it built, and select it.</li>
<li>Select <code>CIA image options...</code>.</li>
<li>Select <code>Decrypt file (0:/gm9/out)</code>.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">Dual Paths</p>
<p>There may be a chance that your file is already decrypted. If that's the case, it will tell you "File is not encrypted". Skip step 21 by just pressing B if your ROM is already decrypted.</p>
</div>
<ol start="21">
<li>Wait for it to decrypt and then press A.</li>
<li>Press R + Start to shutdown your system.</li>
<li>Take out your SD card and insert it into your computer.</li>
<li>Your decrypted ROM is located in <code>/gm9/out/</code>. Copy your ROM to a location of your choice on your computer's hard drive.</li>
<li>Your save file is located in <code>/3ds/Checkpoint/saves/[game title ID] [game title name]/[backup name]/</code>. Copy your save file to a location of your choice on your computer's hard drive.</li>
<li>Take your SD card out of your PC.</li>
<li>Insert your SD card into your 3DS.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">Emulators</p>
<p>These dumps are compatible with an emulator of your choice!</p>
</div>
<h4 id="from-home-menu">From Home Menu</h4>
<div class="admonition info">
<p class="admonition-title">Regarding Fresh Game Data</p>
<p>If you are dumping a brand new game and/or do not have any important save data, skip steps 1-7 and step 28.</p>
</div>
<ol>
<li>Open the game of choice just for a quick second.</li>
<li>Close your game after a few seconds or so by pressing the Home button and closing the software.</li>
<li>Open Checkpoint.</li>
<li>Find your game tied to your cartridge in the app. Checkpoint should tell you if the game is installed on the SD card or from a cartridge.</li>
<li>Select your game and press L to backup your save data. Press A to confirm.</li>
<li>Name this backup whatever you wish, as it's not important.</li>
<li>Once that's finished, press Start to exit out into the Home Menu.</li>
<li>Turn off your system.</li>
<li>Turn your 3DS back on, but this time press and hold Start before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.</li>
<li>You should now be greeted with GodMode9. It may ask you to reset the RTC datetime offset. Do not change the provided date, just mash A until you get to the menu.</li>
<li>Press the Home button.</li>
<li>Navigate to <code>Title manager</code> and select it. </li>
<li>Navigate to <code>[A:] SD CARD</code> and select it. It will take a few seconds to load all the information regarding installed titles.</li>
<li>Navigate to your game of choice and choose <code>Manage Title...</code></li>
<li>Navigate to <code>Build CIA (standard)</code> and select it.</li>
<li>Wait for your ROM to properly dump.</li>
<li>Once that's done, press B to back out to the main menu.</li>
<li>Select <code>[0:] SDCARD</code>.</li>
<li>Navigate to <code>gm9</code> and select it.</li>
<li>Navigate to <code>out</code> and select it.</li>
<li>Navigate to the <code>.cia</code> file it built, and select it.</li>
<li>Select <code>CIA image options...</code>.</li>
<li>Select <code>Decrypt file (0:/gm9/out)</code>.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">Dual Paths</p>
<p>There may be a chance that your file is already decrypted. If that's the case, it will tell you "File is not encrypted". Skip step 24 by just pressing B if your ROM is already decrypted.</p>
</div>
<ol start="24">
<li>Wait for it to decrypt and then press A.</li>
<li>Press R + Start to shutdown your system.</li>
<li>Take out your SD card and insert it into your computer.</li>
<li>Your decrypted ROM is located in <code>/gm9/out/</code>. Copy your ROM to a location of your choice on your computer's hard drive.</li>
<li>Your save file is located in <code>/3ds/Checkpoint/saves/[game title ID] [game title name]/[backup name]/</code>. Copy your save file to a location of your choice on your computer's hard drive.</li>
<li>Take your SD card out of your PC.</li>
<li>Insert your SD card into your 3DS.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">Emulators</p>
<p>These dumps are compatible with an emulator of your choice!</p>
</div>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="dumping-ds-cartridges">Dumping DS Cartridges</h2>
<div class="admonition info">
<p class="admonition-title">Regarding Fresh Game Data</p>
<p>If you are dumping a brand new game and/or do not have any important save data, only follow steps 8-23, 30, 34-39.</p>
</div>
<ol>
<li>Insert your cartridge of choice and open the game just for a quick second.</li>
<li>Close your game after a few seconds or so by pressing the Home button and closing the software.</li>
</ol>
<div class="admonition danger">
<p>Do <strong>NOT</strong> take out your game cartridge at this point in time!!!</p>
</div>
<ol start="3">
<li>Open Checkpoint.</li>
<li>Find your game tied to your cartridge in the app. Checkpoint should tell you if the game is installed on the SD card or from a cartridge.</li>
<li>Select your game and press L to backup your save data. Press A to confirm.</li>
<li>Name this backup whatever you wish, as it's not important.</li>
<li>Once that's finished, press Start to exit out into the Home Menu.</li>
<li>Turn off your system.</li>
<li>Turn your 3DS back on, but this time press and hold Start before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.</li>
<li>You should now be greeted with GodMode9. It may ask you to reset the RTC datetime offset. Do not change the provided date, just mash A until you get to the menu.</li>
<li>Navigate to <code>[C:] GAMECART ()</code>.</li>
<li>Select the <code>[game title ID].nds</code> file and choose "Copy to 0:/gm9/out".</li>
</ol>
<div class="admonition warning">
<p class="admonition-title">About The <code>trim.nds</code> File</p>
<p>The <code>[game title ID].trim.nds</code> file is generally not recommended for DS games as there may arise playback issues. It's a good thing, however, that DS ROMs aren't that big in size anyway.</p>
</div>
<ol start="13">
<li>Wait for your game to copy, however long that takes.</li>
<li>Once that's done, back out as much as you can with the B button and then press Start. This will reboot the system like normal.</li>
</ol>
<div class="admonition note">
<p>After the system is done rebooting, it's now safe to remove the cartridge from your system.</p>
</div>
<ol start="15">
<li>Open FBI from your Home Menu.</li>
<li>Select "SD".</li>
<li>Navigate to <code>/gm9/out</code>.</li>
<li>Select your ROM file, and then select "Copy".</li>
<li>Press B twice to get to your SD card's root. From there, navigate to <code>/roms/nds/</code>.</li>
<li>Select <code>&lt;current directory&gt;</code>.</li>
<li>Select "Paste".</li>
</ol>
<div class="admonition note">
<p><strong>OPTIONAL</strong>: If you would like, you can rename your ROM to whatever you'd like. For example, maybe the game's name. To do this, navigate to the pasted ROM file, select it, and then select "Rename". <strong>Remember to keep its file extension of <code>.nds</code></strong>!</p>
</div>
<ol start="22">
<li>Press B twice to go back to your SD card's root. From there, navigate back to <code>/gm9/out/</code>.</li>
<li>If the original copy of your ROM is still located here, select it and press "Delete".</li>
<li>Press B twice to go back to your SD card's root. From there, navigate to <code>/3ds/Checkpoint/saves/[game title ID] [game title name]/[backup name]/</code>. This is where your save should be.</li>
<li>Select that save file and click "Copy".</li>
</ol>
<div class="admonition warning">
<p class="admonition-title">Save File Chicanery</p>
<p>I've seen cases where some games have multiple <code>.sav</code> files attached to them, which confuses the owners of those games. What I can gather is that the <code>.sav</code> with the biggest file size is the correct one. When hovering over a file in FBI, the top screen should tell you the file size. If that doesn't work at the end of step 32, come back to this step and redo the same step using the other <code>.sav</code> file instead of the bigger one. </p>
</div>
<ol start="26">
<li>Press B four times to go back to your SD card's root. From there, navigate to <code>/roms/nds/saves/</code>.</li>
<li>Select <code>&lt;current directory&gt;</code>.</li>
<li>Select "Paste".</li>
<li>In the same folder, navigate to your save file. Select it and then select "Rename". It needs to be named the same as the game it's tied to. For example, "Pokémon White Version.nds" in <code>/roms/nds/</code> is tied to "Pokémon White Version.sav" in <code>/roms/nds/saves/</code>.</li>
<li>Press B four times to go back to FBI's main menu. From there, press Start to exit out to the Home Menu.</li>
<li>Open TwiLightMenu++.</li>
<li>Navigate to <code>/roms/nds/</code> and select your ROM. This is a check to see if your save file loaded up properly.</li>
<li>Close out of the game by pressing the Home button and then pressing A.</li>
<li>Open The Homebrew Launcher.</li>
<li>Navigate to NDS Forwarder Generator.</li>
<li>n this piece of homebrew, navigate to <code>/roms/nds/</code>.</li>
<li>Select <code>&lt; Install All nds &gt;</code>. Hit "Yes" to confirm.</li>
<li>Once finished, press Start to back out into The Homebrew Launcher.</li>
<li>Press the Home button to exit out into the Home Menu.</li>
</ol>
<div class="admonition warning">
<p class="admonition-title">Title Limit</p>
<p>As stated earlier, <strong>you can only have up to 40 DS games show up on your Home Menu at a time. You will need to play the rest through TwiLightMenu++.</strong></p>
</div>
<div class="admonition note">
<p class="admonition-title">Emulators</p>
<p>These dumps are compatible with an emulator of your choice, should you choose to export these files to use with one! More info on this later.</p>
</div>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="virtual-console-injects-for-retro-games">Virtual Console Injects (For Retro Games)</h2>
<div class="admonition note">
<p class="admonition-title">Personal Preferences</p>
<p>Steps 7-9 include art aspects that are personal preferences. When following along with these steps, you may use your own discretion if you like them or not.</p>
</div>
<ol>
<li>Open <a class="external" href="https://www.dropbox.com/scl/fi/hxvfg8cwrebi5gxeikokr/Debug.zip?rlkey=crc9u3oenpvqf5pwnuff166f4&amp;e=1&amp;dl=0" rel="" target="_blank">this Dropbox link</a> and click on the Download icon at the top right. Do not sign in if you do not want to; just click "Or continue with download only".</li>
<li>Extract the <code>.zip</code> file you just downloaded using an unarchiving application of your choice (i.e. WinRar, 7-Zip).</li>
<li>Open the <code>.exe</code> version of the program.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">Spanish?</p>
<p>If when you open the application and the text is in Spanish, click the tiny gear icon at the top below the file menu and change the language to English. From there, close and reopen the app.</p>
</div>
<ol start="4">
<li>Click "File -&gt; New -&gt; (Console Name) CIA".</li>
<li>Click "Project -&gt; Load ROM".</li>
<li>The program might inform you that it was unable to download game information. This is normal. After that, it'll prompt you to search through their database for game information. Choose the right one. If you can't find it, just write any information into the program.</li>
<li>As for game icon, find an image of the game's box art on Google or SteamGridDB, and load it into the icon by choosing "Load image from file".</li>
<li>In the CIA banner section, in the dropdown menu change it to "3D Frame with Color".</li>
<li>Right below it, click "Load image from file". This time, find an image of the game's title screen on Google and load it in there.</li>
<li>Once you've finished, click "Project -&gt; Export CIA".</li>
<li>Turn off your system.</li>
<li>Take out its SD card and insert it into your computer.</li>
<li>Drag and drop that new <code>.cia</code> file to the <code>/cias/</code> folder on your SD card.</li>
<li>Take your SD card out of your PC.</li>
<li>Insert your SD card back into your 3DS.</li>
<li>Turn your system back on.</li>
<li>Open FBI.</li>
<li>Select "SD".</li>
<li>Navigate to <code>cias</code>.</li>
<li>Select <code>&lt;current directory&gt;</code>.</li>
<li>Select "Install and delete all CIAs".</li>
<li>Once your game is finished installing, press B as much as you can to back out to FBI's main menu. Press Start after that.</li>
<li>Your game should now appear in the Home Menu as a "gift".</li>
</ol>
<div class="admonition warning">
<p>If you just want a fresh copy of the game, stop reading here. However, if you have an  save you want to put into your VC inject that you just created, continue on.</p>
</div>
<ol start="24">
<li>Turn off your system.</li>
<li>Take out its SD card and insert it into your computer.</li>
<li>Drop your save for your game somewhere on the SD card. It doesn't really matter where, but for convenience put it on the root.</li>
<li>Take your SD card out of your PC.</li>
<li>Insert your SD card back into your 3DS.</li>
<li>Turn on your system.</li>
<li>Open your new Virtual Console inject. </li>
<li>Close this game after a few seconds. This stores into memory that you were playing this Virtual Console game last.</li>
<li>Turn off your 3DS.</li>
<li>Turn your 3DS back on, but this time press and hold Start before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.</li>
<li>You should now be greeted with GodMode9. It may ask you to reset the RTC datetime offset. Do not change the provided date, just mash A until you get to the menu.</li>
<li>Navigate to <code>[0:] SDCARD</code> and select it.</li>
<li>Navigate to the location of your save file, and press Y when hovering on your save file. This copies it to the clipboard.</li>
<li>Press B as much as you need to to get back to the GodMode9 main menu.</li>
<li>Navigate to "[S:] SYSNAND VIRTUAL" and select it.</li>
<li>Navigate to <code>agbsave.bin</code> and select it.</li>
<li>Select "AGBSAVE Options" from the menu on the bottom screen.</li>
<li>Navigate to 'Inject GBA VC" and select it.</li>
<li>Back out as much as you can once it's injected.</li>
<li>Press Start to reboot the system.</li>
<li>Whenever you play that VC inject, from now on you can pick up where you previously left off.</li>
</ol>
<h3 id="other-ways-to-play-retro-games">Other Ways To Play Retro Games</h3>
<h4 id="gameboy-color">GameBoy (Color)</h4>
<p>Just use a VC inject.</p>
<h4 id="gameboy-advance">GameBoy Advance</h4>
<div class="admonition info">
<p class="admonition-title">3DS Native GBA Playback</p>
<p>Everyone knows that the 3DS has backwards compatibility with DS games due to it having DSi hardware baked into it, but did you know that that DSi has GBA hardware built into it as well? This means that the DSi and the 3DS families of systems can all play GBA games, they just lacked the GBA port to do that. The 3DS does put that GBA hardware to use, however, in the form of its Virtual Console service.</p>
</div>
<p><strong>open_agb_firm</strong> is a tool that allows for use of the 3DS' native GBA hardware to play your GBA ROM collection.</p>
<ol>
<li>Open Universal Updater from your Home Menu.</li>
<li>Search for "open_agb_firm". The icon looks... very indiscriminate.</li>
<li>Download "open_agb_firm.firm".</li>
<li>Press Start to exit the Universal Updater.</li>
<li>Turn off your system.</li>
<li>Take out its SD card and insert it into your computer.</li>
<li>In a file explorer of your choice, navigate to the <code>/roms/</code> folder.</li>
<li>If a <code>gba</code> folder doesn't exist in it, create one.</li>
<li>Drag and drop any GBA ROMs you'd like into this <code>gba</code> folder.</li>
</ol>
<div class="admonition info">
<p class="admonition-title">Regarding ROMs</p>
<p>In our lovely Discord server, I have made it so our fantastic bot can give you access to a library of ROMs for various systems. For our case, whenever the bot is online please type "!w emulation gba" (without the quotes) in one of the command's permitted channels for a library of GBA ROMs.</p>
</div>
<ol start="10">
<li>Take your SD card out of your PC.</li>
</ol>
<div class="admonition warning">
<p>Make sure you do it safely by manually clicking eject on the file explorer, as we do not want to risk corrupting your game file!</p>
</div>
<ol start="11">
<li>Insert your SD card back into your 3DS.</li>
<li>Turn your 3DS back on, but this time press and hold Select before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.</li>
<li>You should now see the Luma menu. In the Luma menu, make sure <code>Enable loading external FIRMS and modules</code> is enabled.</li>
<li>Press Start to reboot the system.</li>
<li>Turn off your 3DS immediately afterwards.</li>
<li>Turn your 3DS back on, but this time press and hold Start before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.</li>
<li>You should now be greeted with the Luma Chainloader. Select "open_agb_firm".</li>
<li>Navigate to <code>/roms/gba/</code>.</li>
<li>Select the ROM of the game you'd like to play.</li>
<li>When you are finished playing, simply hit the Power button. </li>
</ol>
<div class="admonition info">
<p class="admonition-title">Regarding Saves</p>
<p>If you do not have any save files you would like to import, stop reading here. Otherwise, continue.</p>
</div>
<ol start="21">
<li>Take out its SD card and insert it into your computer.</li>
<li>Drop any of your saves for your games in <code>/3ds/open_agb_firm/saves/</code>. Make sure your save file has the same name as your ROM. For example, "The Minish Cap.gba" in <code>/roms/gba/</code> is tied to "The Minish Cap.sav" in <code>/3ds/open_agb_firm/saves/</code>.</li>
<li>Take your SD card out of your PC.</li>
<li>Insert your SD card back into your 3DS.</li>
<li>Turn your 3DS back on, but this time press and hold Start before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.</li>
<li>You should now be greeted with the Luma Chainloader. Select "open_agb_firm".</li>
<li>Navigate to <code>/roms/gba/</code>.</li>
<li>Select the ROM of the game you'd like to play. Your save should now be imported properly.</li>
</ol>
<h4 id="nintendo-entertainment-system-nes">Nintendo Entertainment System (NES)</h4>
<p>Just use a VC inject.</p>
<h4 id="super-nintendo-entertainment-system-snes">Super Nintendo Entertainment System (SNES)</h4>
<div class="admonition info">
<p class="admonition-title">3DS SNES Virtual Console</p>
<p>Back in the day, Nintendo said the the "Old" variant of the 3DS systems simply could not handle SNES Virtual Console titles and that that luxury was relegeated to "New" variant of the 3DS systems. Everyone knew that was a load of crap coming out of Nintendo, so homebrew developers took it upon themselves to stick it to Nintendo's face in terms of SNES emulation.</p>
</div>
<p><strong>snes_9x</strong> is a very popular SNES emulator, that now has an updated fork for the 3DS.</p>
<ol>
<li>Open Universal Updater from your Home Menu.</li>
<li>Search for "Snes9x (updated fork)". The icon looks... very corporate.</li>
<li>Download "snes9x_3ds.cia".</li>
</ol>
<div class="admonition note">
<p>If you would like, you may choose to install the <code>.3dsx</code> version to launch through The Homebrew Launcher. However, for the sake of the tutorial we will be sticking with the <code>.cia</code> version.</p>
</div>
<ol start="4">
<li>Press Start to exit the Universal Updater.</li>
<li>Turn off your system.</li>
<li>Take out its SD card and insert it into your computer.</li>
<li>In a file explorer of your choice, navigate to the <code>/roms/</code> folder.</li>
<li>If a <code>snes</code> folder doesn't exist in it, create one.</li>
<li>Drag and drop any SNES ROMs you'd like into this <code>snes</code> folder.</li>
</ol>
<div class="admonition info">
<p class="admonition-title">Regarding ROMs</p>
<p>In our lovely Discord server, I have made it so our fantastic bot can give you access to a library of ROMs for various systems. For our case, whenever the bot is online please type "!w emulation snes" (without the quotes) in one of the command's permitted channels for a library of SNES ROMs.</p>
</div>
<ol start="10">
<li>Take your SD card out of your PC.</li>
</ol>
<div class="admonition warning">
<p>Make sure you do it safely by manually clicking eject on the file explorer, as we do not want to risk corrupting your game file!</p>
</div>
<ol start="11">
<li>Insert your SD card back into your 3DS.</li>
<li>Turn your 3DS back on.</li>
<li>Open Snes9x. It should appear as a "present" on the Home Menu.</li>
<li>Navigate to <code>/roms/snes/</code>.</li>
<li>Select the ROM of the game you'd like to play.</li>
<li>When you are finished playing, simply hit the Power button. </li>
</ol>
<div class="admonition info">
<p class="admonition-title">Regarding Saves</p>
<p>If you do not have any save files you would like to import, stop reading here. Otherwise, continue.</p>
</div>
<ol start="17">
<li>Take out its SD card and insert it into your computer.</li>
<li>Drop any of your saves for your games in <code>/3ds/snes_9x/saves/</code>. Make sure your save file has the same name as your ROM. For example, "Final Fantasy III.sfc" in <code>/roms/snes/</code> is tied to "Final Fantasy III.srm" in <code>/3ds/snes_9x/saves/</code>.</li>
<li>Take your SD card out of your PC.</li>
<li>Insert your SD card back into your 3DS.</li>
<li>Turn your 3DS back on.</li>
<li>Open Snes9x.</li>
<li>Navigate to <code>/roms/snes/</code>.</li>
<li>Select the ROM of the game you'd like to play. Your save should now be imported properly.</li>
</ol>
<h4 id="sony-playstation">Sony PlayStation</h4>
<div class="admonition warning">
<p class="admonition-title">New 3DS Only!</p>
<p>Only the "New" variant of 3DS systems can emulate PlayStation games. If you do not have one of those, you're out of luck...</p>
</div>
<p><strong>RetroArch</strong> can be used to emulate PS1 games through its <em>PCSX-ReARMed</em> core.</p>
<ol>
<li>Go to <a class="external" href="https://www.retroarch.com/?page=platforms" rel="" target="_blank">this website</a>.</li>
<li>Navigate to the Download section for the "3DS / 2DS Family". Click on "Download (cia)". </li>
<li>Extract that <code>.7z</code> archive you just downloaded using an unarchiving application of your choice. (i.e. WinRar, 7-Zip)</li>
<li>Navigate to <code>/retroarch_cia/retroarch/cores</code>.</li>
<li>Delete all cores in <code>.cia</code> format in this folder except for <code>pcsx_rearmed_libretro.cia</code>. This is our PS1 emulator.</li>
<li>Go back one folder, so now our current working directory is <code>/retroarch_cia/retroarch/</code>.</li>
<li>Turn off your 3DS.</li>
<li>Take out its SD card and insert it into your computer.</li>
<li>Drag and drop the <code>retroarch</code> folder inside the <code>retroarch_cia</code> folder onto the root of your SD card.</li>
<li>Drag and drop the <code>retroarch_3ds.cia</code> file inside <code>/retroarch_cia/cia</code> insides your 3DS' <code>cias</code> folder.</li>
<li>Take your SD card out of your PC.</li>
<li>Insert your SD card back into your 3DS.</li>
<li>Turn your 3DS back on.</li>
<li>Open FBI.</li>
<li>In FBI, select "SD".</li>
<li>Navigate to your <code>cias</code> folder.</li>
<li>Select "&lt;current directory&gt;".</li>
<li>Select "Install and delete all CIAs".</li>
<li>Once RetroArch is finished installing, press B as much as you can to back out to FBI's main menu. Press Start after that.</li>
<li>RetroArch should now appear in the Home Menu as a "gift".</li>
<li>Open RetroArch. It should try to initialize all the information with your system. Give it it's time. It will close out on its own once complete.</li>
<li>On your Home Menu, you may see that RetroArch installed an unnecessary core to your Home Menu. Ignore it for now. Open the main RetroArch app again.</li>
<li>Navigate to "Load core" and select it.</li>
<li>Navigate to <code>/retroarch/cores/pcsx_rearmed_libretro.cia</code> and select it. In the background, it will install the PS1 emulator directly to your Home Menu and then immediately send you to the PS1 emulator app.</li>
<li>Once you've loaded the emulator, close out of it by pressing the Home button and closing out of it.</li>
<li>Open the System Settings app.</li>
<li>Navigate through Data Management -&gt; 3DS -&gt; Software.</li>
<li>Find both the main RetroArch app and (if applicable) that random unnecessary core.</li>
<li>Exit out of the System Settings application.</li>
<li>Turn off your 3DS.</li>
<li>Take out its SD card and insert it into your computer.</li>
<li>In a file explorer of your choice, navigate to the <code>/roms/</code> folder.</li>
<li>If a <code>psx</code> folder doesn't exist in it, create one.</li>
<li>Drag and drop any PS1 ROMs you'd like into this <code>psx</code> folder.</li>
</ol>
<div class="admonition info">
<p class="admonition-title">Regarding ROMs</p>
<p>In our lovely Discord server, I have made it so our fantastic bot can give you access to a library of ROMs for various systems. For our case, whenever the bot is online please type "!w emulation ps1" (without the quotes) in one of the command's permitted channels for a library of PS1 ROMs. Additionally, the bot also gives instructions on how to properly compress your PS1 ROMs, so give that a shot as well.</p>
</div>
<ol start="34">
<li>Take your SD card out of your PC.</li>
</ol>
<div class="admonition warning">
<p>Make sure you do it safely by manually clicking eject on the file explorer, as we do not want to risk corrupting your game file!</p>
</div>
<ol start="35">
<li>Insert your SD card back into your 3DS.</li>
<li>Turn your 3DS back on.</li>
<li>Open PCSX_ReARMed.</li>
<li>Select "Load Content" and navigate to your PS1 ROM.</li>
<li>When finished playing, tap the bottom screen and navigate to close content. Then, close out of the application.</li>
</ol>
<div class="admonition info">
<p class="admonition-title">Regarding Saves</p>
<p>If you do not have any save files you would like to import, stop reading here. Otherwise, continue.</p>
</div>
<ol start="40">
<li>Take out its SD card and insert it into your computer.</li>
<li>Drop any of your saves for your games in <code>/retroarch/cores/savefiles/</code>. Make sure your save file has the same name as your ROM. For example, "Crash Bandicoot.chd" in <code>/roms/psx/</code> is tied to "Crash Bandicoot.srm" in <code>/retroarch/cores/savefiles/</code>.</li>
<li>Take your SD card out of your PC.</li>
<li>Insert your SD card back into your 3DS.</li>
<li>Turn your 3DS back on.</li>
<li>Open PCSX_ReARMed.</li>
<li>Navigate to <code>/roms/psx/</code>.</li>
<li>Select the ROM of the game you'd like to play. Your save should now be imported properly.</li>
</ol>
<h4 id="nintendo-64">Nintendo 64</h4>
<div class="admonition warning">
<p class="admonition-title">New 3DS Only!</p>
<p>Only the "New" variant of 3DS systems can emulate PlayStation games. If you do not have one of those, you're out of luck...</p>
</div>
<p>Although it, for some reason, is advertised as doable, I've seen more reports that other people can never get it to work. And even if they can it's not in a very playable state. Therefore, I would advise against trying this.</p>
<h4 id="virtualboy">VirtualBoy</h4>
<p>Yes, it's possible. Somehow. <strong>There is a VirtualBoy emulator for the 3DS called Red-Viper</strong>. It has the ability to utilize the 3DS' stereoscopic 3D effects to emulate what would have been the VirtualBoy's fields of depth.</p>
<ol>
<li>Open Universal Updater from your Home Menu.</li>
<li>Search for "red-viper". The icon looks... very unintuitive.</li>
<li>Download "red_viper.3dsx".</li>
<li>Press Start to exit the Universal Updater.</li>
<li>Turn off your system.</li>
<li>Take out its SD card and insert it into your computer.</li>
<li>In a file explorer of your choice, navigate to the <code>/roms/</code> folder.</li>
<li>If a <code>vb</code> folder doesn't exist in it, create one.</li>
<li>Drag and drop any VirtualBoy ROMs you'd like into this <code>vb</code> folder.</li>
</ol>
<div class="admonition info">
<p class="admonition-title">Regarding ROMs</p>
<p>Unfortunately, our bot does not supply VirtualBoy ROMs. You must scout those for yourself until I add support for that to the bot. Sorry!</p>
</div>
<ol start="10">
<li>Take your SD card out of your PC.</li>
</ol>
<div class="admonition warning">
<p>Make sure you do it safely by manually clicking eject on the file explorer, as we do not want to risk corrupting your game file!</p>
</div>
<ol start="11">
<li>Insert your SD card back into your 3DS.</li>
<li>Turn your 3DS back on.</li>
<li>Open The Homebrew Launcher.</li>
<li>Navigate to <code>red-viper.3dsx</code> and select it.</li>
<li>Navigate to <code>/roms/vb/</code>.</li>
<li>Select the ROM of the game you'd like to play.</li>
<li>When you are finished playing, simply hit the Home button and close out of the application.</li>
</ol>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="going-online-in-3ds-games">Going Online In 3DS Games</h2>
<div class="admonition info">
<p class="admonition-title">About Online Services</p>
<p>On April 8th, 2024 5 PM PDT, Nintendo shut down the Nintendo Network. Nintendo Network was the one way the 3DS and Wii U went online in games. However, Pretendo is a WIP open source replacement of Nintendo Network functionality. With Pretendo, you can go online with your 3DS post-Nintendo Network shutdown, along with gaining access a new (and improved) version of Miiverse among other cool things.</p>
</div>
<div class="admonition warning">
<p class="admonition-title">Your Friends List</p>
<p>Setting up Pretendo does <strong>NOT</strong> carry over your Friends List. Pretendo has stated that while they think a potential NNID -&gt; PNID account transfer is possible, it is outside the scope of the project on top of potential lawsuits from Nintendo that may arise from handling NNID data from them.</p>
</div>
<ol>
<li>Open Universal Updater from your Home Menu.</li>
<li>Search for "Nimbus". The icon looks like a purple lowercase N.</li>
<li>You can choose whether you want to install the <code>.3dsx</code> version or the <code>.cia</code> version. Keep in mind, the <code>.3dsx</code> version is meant to be launched through The Homebrew Launcher, while the <code>.cia</code> version is meant to be launched through the Home Menu.</li>
</ol>
<div class="admonition note">
<p>For the sake of this guide, we will be installing the <code>.3dsx</code> version. Though, instructions shouldn't vary by much if you choose to go the other route. Only by means of how to access the Nimbus application.</p>
</div>
<ol start="4">
<li>Press Start to exit out of the Universal Updater once it's finished installing.</li>
<li>Turn off your system.</li>
<li>Turn your 3DS back on, but this time press and hold Select before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.</li>
<li>You should now see the Luma menu. In the Luma menu, make sure both <code>Enable loading external FIRMS and modules</code> and <code>Enable game patching</code> are enabled.</li>
<li>Press Start to reboot the system.</li>
<li>Open The Homebrew Launcher.</li>
<li>Navigate to Nimbus and select it.</li>
<li>Select "Pretendo" on the bottom screen.</li>
<li>Once the system finishes reloading, press the Home button to suspend The Homebrew Launcher. Close out of it.</li>
<li>Put your 3DS aside for now, but leave it on. Ideally, you can put it in Sleep Mode.</li>
<li>Go to <a class="external" href="https://pretendo.network/" rel="" target="_blank">Pretendo's website</a> on a computer. Set up an account with them (A "PNID").</li>
</ol>
<div class="admonition danger">
<p class="admonition-title">About Account Names</p>
<p>You may <strong>NOT</strong> use the same account name as your old NNID! For example, if I had registered an NNID with Nintendo with the ID name of "JohnDoe", you can create a PNID with the ID name of "JohnDoe" but your 3DS will not be able to sign into that PNID. As such, try to find a new ID name for your PNID. (i.e. "JohnDoe" uses "DohnJoe" instead). </p>
</div>
<ol start="15">
<li>Once you've set up your account with them, open the System Settings application on your 3DS.</li>
<li>Open the "Nintendo Network ID Settings" applet.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">Potential Confusion</p>
<p>Even if we are connected to Pretendo's servers, there is no reference to a "Pretendo" in the 3DS' UI. Therefore, please just remember that you are connected to Pretendo servers when trying to access "Nintendo" Network stuff.</p>
</div>
<ol start="17">
<li>Log into your PNID as if it were an NNID. Choose "Link existing ID" when signing in. Remember to select the option to use the Mii that's registered with your system as the face of your PNID instead of the default one.</li>
<li>Once you're done with that, you should immediately get booted back into the System Settings application. Just close out of it.</li>
<li>You're done! This is only a one time set up!</li>
</ol>
<div class="admonition note">
<p>If you wish to verify that you are finished with the set up process, try opening the Friends List applet. If you are able to go online and you have an empty list of friends, you are good to go. If not, there are people who can try helping in <a class="external" href="https://invite.gg/pretendo" rel="" target="_blank">their Discord server</a>.</p>
</div>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="going-online-in-ds-games">Going Online In DS Games</h2>
<div class="admonition info">
<p class="admonition-title">About Wiimmfi</p>
<p>Nintendo Wi-Fi Connection (Nintendo WFC) was a service that the DS and the Wii used to go connect your games online. It was shut down on May 20th, 2014, due to the outsourced company that was hosting Nintendo's servers being shut down. However, over the course of the years afterwards, dedicated fans were able to revive these servers for Wii and DS games through Wiimmfi! In some cases, it can be as easy as simply entering a DNS code to route your network information to!</p>
</div>
<div class="admonition info">
<p class="admonition-title">What Kind Of Game Do You Have?</p>
<p>The original DS from 2004 could only connect to Wi-Fi networks with either no security whatsoever that don't have a web based sign in (something like an airport's or a Starbucks Wi-Fi), or ones using the outdated WEP security protocol, which had been cracked by 2001 and was officially deprecated in favor of WPA2 in 2004. The DSi offered enhanced Wi-Fi capabilities, including support for WPA and WPA2 security protocols. This is important for games like the Gen 5 Pokémon games, which are 'DSi Enhanced' and can take advantage of these newer security standards when played on a DSi or 3DS. Thus, it's important to note whether the game you want to go online in is DSi Enhanced or not. <a class="external" href="https://gamicus.fandom.com/wiki/List_of_DSi_enhanced_video_games" rel="" target="_blank">This list</a> may tell you. Chances are the game you want to play isn't, however.</p>
</div>
<h3 id="dsi-enhanced-games">DSi Enhanced Games</h3>
<ol>
<li>Open the System Settings app on your 3DS' Home Menu.</li>
<li>Select "Internet Settings".</li>
<li>Select "Connection Settings".</li>
<li>Select the number associated with your Wi-Fi connection. For example, "Connection 1".</li>
<li>Select "Change Settings".</li>
<li>Tap the right arrow on the right of the bottom screen just once.</li>
<li>Select "DNS".</li>
<li>Select "No" under the section for "Auto-Obtain DNS".</li>
<li>Select "Detailed Setup".</li>
<li>Make sure the Primary and Secondary DNS numbers are the same as the ones listed <a class="external" href="https://wiilink.ca/guide/wii/#connecting-to-dns" rel="" target="_blank">here</a>. If not, configure that. Don't get thrown off by the fact that WiiLink's guide tells you how to set up this DNS with a Wii, as this DNS also works with the DS and should you have been following along this whole time you wouldn't need to follow their steps. Just find and use the DNS numbers on this page.</li>
<li>Select "OK".</li>
<li>Select "Save" then "OK".</li>
<li>It will ask you to do a connection test. This doesn't really matter, but to be on the safe side, select "Test".</li>
<li>Once your connection test is successful, back out 3 times by tapping "Back" on the bottom screen thrice.</li>
<li>Press X to close out of the System Settings app.</li>
<li>Load up your DSi Enhanced game. It may be either through a cartridge or through a dump that you had situated on your 3DS.</li>
</ol>
<h3 id="non-dsi-enhanced-games">Non-DSi Enhanced Games</h3>
<div class="admonition note">
<p class="admonition-title">The Modern Day</p>
<p>Chances are that nowadays, your Wi-Fi router at home does not support WEP security. Additionally, it is also common practice for your home internet to have a password attached to it, meaning it has to fall under some other security protocol. As of late 2024, that protocol will likely be WPA3, which obviously is not WEP. This leaves us with a few options... </p>
</div>
<h5 id="a-password-less-hotspot-from-an-android-phone">A Password-less Hotspot From An Android Phone</h5>
<div class="admonition warning">
<p class="admonition-title">"Why Not iPhones As Well"?</p>
<p>This is simply because of software restrictions that Apple has set on their iOS. iOS will simply not allow you to create a password-less hotspot from your phone; an iPhone's hotspot must have some form of encryption to it. By modern standards, the encryption that iOS hotspots are allowed to use are not WEP, which means they cannot be detected by the Nintendo DS.</p>
</div>
<ol>
<li>Open the hotspot settings on your Android phone. Instructions on how to do this varies between Android versions and the manufacturers of your phone, so you may need to look up how to do that for your make and model.</li>
<li>Configure your hotspot to however you like (i.e. the name/SSID of your hotspot), just make sure that the security parameter is set to "None" and that the speed/bandwidth is set to 2.4 GHz. This means your hotspot will have no password attached to it and can be read at a frequency that your 3DS can read.</li>
<li>Save whatever configurations you made.</li>
<li>Turn on your hotspot and put your Android phone aside for now. Leave it on the hotspot menu however.</li>
<li>Turn on your 3DS.</li>
<li>Open the System Settings app on your 3DS' Home Menu.</li>
<li>Select "Internet Settings".</li>
<li>Select "Connection Settings".</li>
<li>Select "Nintendo DS Connections" and then "OK". This will bring you to the DS Wi-Fi settings in built into the 3DS' DSi firmware after a quick automatic reboot.</li>
<li>Select "Nintendo Wi-Fi Connection Settings".</li>
<li>Select an empty connection number.</li>
<li>Select "Manual Setup".</li>
<li>Enter the SSID of your hotspot into the box for SSID on your "DS".</li>
<li>Select "No" under the section for "Auto-Obtain DNS".</li>
<li>Make sure the Primary and Secondary DNS numbers are the same as the ones listed <a class="external" href="https://wiilink.ca/guide/wii/#connecting-to-dns" rel="" target="_blank">here</a>. If not, configure that. Don't get thrown off by the fact that WiiLink's guide tells you how to set up this DNS with a Wii, as this DNS also works with the DS and should you have been following along this whole time you wouldn't need to follow their steps. Just find and use the DNS numbers on this page.</li>
<li>Select "Save Settings".</li>
<li>Select the number of the connection you just configured.</li>
<li>Select "Test Connection".</li>
<li>Once your connection is successful, press the B button 4 times to have your system automatically reboot back into the 3DS' Connection Settings.</li>
<li>Select "Back".</li>
<li>Press X to close out of the System Settings application.</li>
<li>Open a Non-DSi Enhanced Game of your choice. It may be either through a cartridge or through a dump that you had situated on your 3DS.</li>
</ol>
<div class="admonition warning">
<p class="admonition-title">Data Usage</p>
<p>This method will consume a LOT of your monthly allowance for cellular data, if you have such an allowance. Please be cautious with how long you are going online with your game if this is the case. Alternatively, you can also follow the second or third options listed right below.</p>
</div>
<h4 id="using-the-melonds-emulator">Using The melonDS Emulator</h4>
<ol>
<li>Either dump your Non-DSi Enhanced DS game, or scavenge for its ROM online. Instructions for both methods are listed above. If it is already backed up, ignore this step.</li>
<li>Turn off your system.</li>
<li>Take out its SD card and insert it into your computer.</li>
<li>In our Discord server, in any of the command's permitted channels, enter <code>!w emulation ds</code>.</li>
<li>Follow step 1 and steps 4-6 on the guide provided. Just remember, when following step 4 set your "Save files path" to <code>/roms/nds/saves</code> that is on your SD card. This way, it will directly read and write from the save you had extracted and placed properly on your system. Also, when following step 6 locate to your game's ROM in <code>/roms/nds</code>.</li>
<li>In your game, enter the Wi-Fi settings. For example, in "Mario Kart DS" this can be done by selecting "Nintendo WFC" in the game's title screen and then by selecting "Nintendo WFC Settings".</li>
<li>Select "Nintendo Wi-Fi Connection Settings".</li>
<li>Select Connection 1. You should see that the SSID is "melonAP".</li>
<li>Select "No" under the section for "Auto-Obtain DNS".</li>
<li>Make sure the Primary and Secondary DNS numbers are the same as the ones listed <a class="external" href="https://wiilink.ca/guide/wii/#connecting-to-dns" rel="" target="_blank">here</a>. If not, configure that. Don't get thrown off by the fact that WiiLink's guide tells you how to set up this DNS with a Wii, as this DNS also works with the DS and should you have been following along this whole time you wouldn't need to follow their steps. Just find and use the DNS numbers on this page.</li>
<li>Select "Save Settings".</li>
<li>Select the number of the connection you just configured.</li>
<li>Select "Test Connection".</li>
<li>Once your connection is successful, press the B button thrice to have your system automatically go back to your game.</li>
<li>Once finished with the game's online features and/or are finished playing the game, select "System -&gt; Stop" from the menu at the top.</li>
<li>Close out of melonDS.</li>
<li>Take your SD card out of your PC.</li>
<li>Insert your SD card back into your 3DS.</li>
</ol>
<div class="admonition warning">
<p class="admonition-title">Locking Down</p>
<p>This method requires the use of a computer with a (micro)SD card slot to insert your card into. Additionally, you would then be tied to using your game with melonDS to go online, as Nintendo WFC configurations from back in the day treated a game and a console as one tied-together unit. If this doesn't seem like something you'd want to do, but have a spare bit of money on you, you could try setting up a network hotspot in your house following the steps listed below.</p>
</div>
<h4 id="using-a-portable-router">Using A Portable Router</h4>
<p>You can buy a cheap "travel" router from tech junk stores or the internet for relatively cheap. <a class="external" href="https://www.tp-link.com/us/home-networking/wifi-router/tl-wr802n/" rel="" target="_blank">The router I have</a> fits in my pocket, and is so small people aren't even going to notice it's there unless they <em>really</em> looked. You may even forget you have this router once this setup is done! (Please don't.).</p>
<div class="admonition warning">
<p class="admonition-title">Assumptions Made!</p>
<p><strong>This guide assumes that you're using the router I linked above!</strong> This is just so that there is parity with instructions and your setup process.</p>
</div>
<div class="admonition note">
<p class="admonition-title">Keep Track</p>
<p>Remember, if at any point during the set up of this router (steps 1-36) you ever get disconnected from the router's network that you need to reconnect it in order to continue on to the next step.</p>
</div>
<ol>
<li>Buy the router I linked above.</li>
<li>Wait however long for that to arrive at your door.</li>
<li>Unbox the router. You will get a sticker with the default SSID and password configuration printed on it. Save this for later.</li>
<li>The router comes with an included USB to microUSB cable and a power brick. Plug in your router to an outlet accordingly.</li>
<li>Wait about 30 seconds to 1 minute to let the router configure itself.</li>
<li>On your PC, connect to the default Wi-Fi configuration from that sticker earlier from your PC's Wi-Fi settings.</li>
<li>On your PC's web browser, go to <code>http://192.168.0.1/</code>. This is the webpage for your router's configuration settings. Your browser may complain that you're accessing an unsecure site (as we are accessing a <code>http</code> site versus a <code>https</code> site, so make sure you work around this. This process varies depending on browser, so I cannot help you.</li>
<li>It will prompt you to set a password. This password is to make sure that no one except for whoever knows it can configure your router, thus, <strong>make sure this password is secure!</strong> You will then be sent to the Quick Setup section.</li>
<li>Click on "Next".</li>
<li>Click on the box for "WISP" mode, and then click Next.</li>
<li>Click on the box for "Dynamic IP (Most common option)" mode, and then click Next.</li>
<li>The router will scan for all nearby Access Points (APs). Click on "Connect" in the row and column for your desired Wi-Fi network. You may see several options for the same network. Choose the row which has the highest "Signal strength".</li>
<li>In the box for "Wireless password", enter the password for the Wi-Fi network you selected earlier.</li>
<li>In the box for "Local Network SSID", enter a new SSID if you wish. This is the name of the Wi-Fi network you see, so if you don't want to see the default name change it to something more meaningful to you.</li>
<li>Click on the box for "Disable Wireless Security". <strong>THIS IS IMPORTANT!</strong> We will soon be working to make sure very little other people can connect to this network, if they can even find it, so don't freak out quite yet. Your DS-mode 3DS and your PC will only be able to connect to this open network by the end of this set up.</li>
<li>Click on the box that says "Next".</li>
<li>The screen will show your configuration just for you to double check. Click on "Finish".</li>
<li>The router will now restart. Wait for this progress bar to finish, and then wait another 30 seconds to 1 minute. You will need to reconnect to the new SSID you set earlier.</li>
<li>Once done, in the Wireless tab of the configuration page, click on the subsection for "Basic settings".</li>
<li>Uncheck the box for "Enable SSID Broadcast".</li>
<li>Click on "Save".</li>
<li>In the Wireless tab of the configuration page, click on the subsection for "Wireless MAC Filtering".</li>
<li>Get your PC's MAC Address. This is necessary so that if you ever need to make changes to the router configuration, your PC can be a base for that. On Windows, read <a class="external" href="https://kb.ucdavis.edu/?id=00209" rel="" target="_blank">this guide</a> to figure out how. On MacOS or Linux, open a terminal of choice and enter <code>ifconfig en0 | grep ether</code>.</li>
<li>Click on the "Add New" button on the router configuration page.</li>
<li>Enter the MAC Address you got earlier into the respective textbox. Capitalize any letters you see in that address.</li>
<li>In the textbox for description, make a quick one-liner to let you know this is your PC. For example, "My PC".</li>
<li>Click on "Save".</li>
<li>Click on the "Add New" button again.</li>
<li>In the textbox for description, make a quick one-liner to let you know this is your 3DS. For example, "My 3DS".</li>
<li>Turn on your 3DS.</li>
<li>Open the System Settings application.</li>
<li>Navigate through Internet Settings -&gt; Other Information -&gt; Confirm MAC Address. You should then be able to see your 3DS' MAC address.</li>
<li>In the textbox for the MAC Address, enter the MAC Address you see on your 3DS' touch screen. Replace any dashes (-) with colons (:).</li>
<li>Click on "Save".</li>
<li>Click on the box for "Allow the stations specified by any enabled entries in the list to access.".</li>
<li>Finally, you can click on the giant "Enable" button at the top of this page.</li>
<li>We're done with all network configurations. Close out of the router configuration settings tab in your browser. We won't be needing a PC anymore.</li>
<li>On your 3DS, tap on "Back" twice.</li>
<li>Tap on "Nintendo DS Connections".</li>
<li>Tap on "OK". This will reboot the system into DS mode.</li>
</ol>
<div class="admonition warning">
<p class="admonition-title">Holding Start or Select?</p>
<p>If you didn't already know, when booting into DS mode for whatever reason (most times, loading a DS game), you can hold the Start or Select button while the DS software is booting so that it displays at a 4:3 resolution that the original DS used instead of a 5:3 resolution like the 3DS uses when playing DS games. This can be helpful because the 5:3 resolution can really wash out some colors and stretch the image a bit too much. Accessing DS Wi-Fi settings like this is no exception to this, but there's a catch. Due to the nature of this set up you can connect to a network like this without the need to mod your 3DS, but since this megathread is about things you can do with a modded system this is made under the assumption that your 3DS is modded. In which case, holding Start in this segment will open GodMode9 (or the Luma3DS chainloader if you have open_agb_firm installed as well), whereas holding Select in this segment will open the Luma3DS menu. Pressing Start afterward will <em>not</em> reboot you back into 3DS mode, but into DS mode. So in case you get thrown off by this, don't be. :)</p>
</div>
<ol start="41">
<li>Select "Nintendo Wi-Fi" Connection Settings.</li>
<li>On any of the three available connections, select the box that says "None" for that open connection.</li>
<li>Navigate to "Manual Setup" and select it.</li>
<li>Select "Edit" in the SSID section.</li>
<li>Enter the SSID you created earlier and then select OK. Confirm it from there.</li>
<li>Navigate to the "Auto-obtain DNS" section and select "No".</li>
<li>Make sure the Primary and Secondary DNS numbers are the same as the ones listed <a class="external" href="https://wiilink.ca/guide/wii/#connecting-to-dns" rel="" target="_blank">here</a>. If not, configure that. Don't get thrown off by the fact that WiiLink's guide tells you how to set up this DNS with a Wii, as this DNS also works with the DS and should you have been following along this whole time you wouldn't need to follow their steps. Just find and use the DNS numbers on this page.</li>
<li>Select "Save Settings".</li>
<li>Select the number of the connection you just configured.</li>
<li>Select "Test Connection".</li>
<li>Once your connection is successful, press the B button thrice to have your system automatically go back to the 3DS Internet Settings.</li>
<li>Tap on "Back".</li>
<li>Tap on "Close" or press X.</li>
<li>Open your Non-DSi Enhanced game.</li>
<li>Happy netplay!</li>
</ol>
<p>From now on, your 3DS will automatically connect to this small router when playing a Non-DSi Enhanced game online. No need to reconfigure your router again afterwards. Just let it sit.</p>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="using-cheats">Using Cheats</h2>
<div class="admonition danger">
<p class="admonition-title">Be A Good Samaritan!</p>
<p>Please do <strong>NOT</strong> use game-breaking cheats online in your games! Not only can you get banned from using certain online services, it also ruins the fun for other people playing with you!</p>
</div>
<h3 id="3ds-games">3DS Games</h3>
<ol>
<li>Open the game of choice just for a quick second.</li>
<li>Close your game after a few seconds or so by pressing the Home button and closing the software.</li>
<li>Open Checkpoint.</li>
<li>Find your game in the app. Select it.</li>
<li>Using the touchscreen, select "Cheats" below the "Restore" option.</li>
<li>Select the cheats you'd like to enable from the list.</li>
<li>Press B once finished selecting your cheats.</li>
<li>Press A to save.</li>
<li>Press Start to exit Checkpoint.</li>
<li>Open your game of choice.</li>
<li>Press L + D-Pad Down + Select.</li>
<li>Navigate to "Cheats..." and select it</li>
<li>Select the cheats you want to use.</li>
<li>Go wild!</li>
</ol>
<h3 id="ds-games">DS Games</h3>
<div class="admonition warning">
<p class="admonition-title">Assumption Made!</p>
<p><strong>This guide assumes that you have dumped a ROM of a game or have it set up through TwiLight Menu++</strong>! If you haven't done that already, please do so! Instructions are above.</p>
</div>
<div class="admonition info">
<p class="admonition-title">Regarding The Cheats Database</p>
<p>If you already have this file installed, skip to step 5.</p>
</div>
<ol>
<li>Open the Universal Updater.</li>
<li>Search for "NDS(i) Cheat Databases". The logo looks like the Action Replay DS logo.</li>
<li>Download the <code>[twlmenu] usrcheat.dat</code> file.</li>
<li>Press Start to exit out of the Universal Updater.</li>
<li>Open TwiLightMenu++ from the Home Menu.</li>
<li>Navigate to a game of your choice.</li>
<li>Press Y and then X to open the cheats menu.</li>
<li>Select whatever cheats you want.</li>
<li>Press X to save the cheat information.</li>
<li>Press B.</li>
<li>Press A to launch your game.</li>
<li>Use your cheats!</li>
</ol>
<div class="admonition note">
<p class="admonition-title">Regarding Forwarded Games</p>
<p>If your game is forwarded to the Home Menu, these same cheats will still apply!</p>
</div>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="installing-unofficial-themes">Installing Unofficial Themes</h2>
<ol>
<li>On your computer, open <a class="external" href="https://themeplaza.art/themes" rel="" target="_blank">this website</a>.</li>
<li>Search for a general topic for a theme you'd like.</li>
<li>Hover your mouse over the picture of a theme you like, and a QR code should appear on screen. Keep your mouse still.</li>
<li>Turn on your 3DS and open the Anemone app.</li>
<li>Press R for "Scan QR Code".</li>
<li>With your 3DS' exterior cameras, scan the QR code that shows over your mouse.</li>
<li>After it is finished installing, navigate to your new theme.</li>
<li>While holding the A button, press and hold Up on the D-pad. Release your hold on the A button while still holding down Up on the D-pad.</li>
<li>Once the theme has finished loading, press Start and turn off the system.</li>
<li>Upon reboot, your new theme should be applied to your system.</li>
</ol>
<h3 id="optional-mix-matching-music">(Optional) Mix-Matching Music</h3>
<p>You can have music from other themes play on an entirely different theme if you'd like! The process isn't all that much harder either, you just need 2 themes downloaded into Anemone.</p>
<ol>
<li>Open Anemone on your 3DS.</li>
<li>Navigate to the theme you'd want displayed. We'll call it the presentor theme.</li>
<li>While holding the A button, press and hold Up on the D-pad. Release your hold on the A button while still holding down Up on the D-pad.</li>
<li>Once the presentor has finishing loading, press Start and turn off the system.</li>
<li>Upon reboot, the presentor should be displaying but we're not done yet. Open Anemone.</li>
<li>Navigate to the theme you'd want the music of to be playing. We'll call it the donor theme.</li>
<li>While holding the A button, press and hold Left on the D-pad. Release your hold on the A button while still holding down Left on the D-pad.</li>
<li>Once the donor has finished loading, press Start and turn off the system.</li>
<li>Upon reboot, the presentor should be displaying while the donor's theme music is playing.</li>
</ol>
<h3 id="optional-shuffling-themes">(Optional) Shuffling Themes</h3>
<p>You can have it so that whenever you enter the Home Menu of your 3DS, a different theme shows up. This can be through a variety of methods, including but not limited to entering/exiting Sleep Mode or suspending games/apps. Make sure to already have a few themes downloaded!</p>
<ol>
<li>Open Anemone on your 3DS.</li>
<li>Scroll through the list of themes you have downloaded. If you want that theme to be included in the shuffle press B when hovering over the theme.</li>
<li>When finished with deciding what themes you want to shuffle, hold down on the A button. While holding the A button, press and hold Down on the D-pad. Release your hold on the A button while still holding down Down on the D-pad.</li>
<li>Once the themes have finished loading, press Start and turn off the system.</li>
<li>Upon reboot, the shuffle should be activated.</li>
</ol>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="installing-custom-badges">Installing Custom Badges</h2>
<ol>
<li>Open Universal Updater from your Home Menu.</li>
<li>Search for "GYTB". What stands out to me in its icon is a pixel art ladybug.</li>
<li>Download the <code>gytb.cia</code> file.</li>
</ol>
<div class="admonition warning">
<p>Looking through the program's GitHub repository, it seems that the <code>.3dsx</code> homebrew version is meant for 3DS systems that were hacked through a VERY outdated method. Therefore, please avoid it as it by extension is also outdated.</p>
</div>
<div class="admonition note">
<p class="admonition-title">Important</p>
<p>If you had already played Nintendo Badge Arcade way back when, skip steps 4-6. It is imperative if you know if you did or didn't, but that's easily checked by if your system allows you to select badges from the Home Menu. Alternatively, you'll know if you have by the <code>badges</code> folder on the root of your SD card is already populated by files for badges.</p>
</div>
<ol start="4">
<li>Press Start to exit out of the Universal Updater.</li>
<li>Go to hShop/3hs (whichever method you prefer) and download Nintendo Badge Arcade. </li>
<li>Play through its tutorial.</li>
<li>Once done, exit out of the application by pressing the Home button and closing out of the app.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">Important</p>
<p>By this point, everyone reading this guide should have now used Nintendo Badge Arcade at least once. However, there may be a subsection of you that have used it in the past and deleted it. If you are one of those people, skip steps 8-11.</p>
</div>
<ol start="8">
<li>Open the System Settings application.</li>
<li>Navigate through Data Management -&gt; 3DS -&gt; Software.</li>
<li>Find Nintendo Badge Arcade and delete it.</li>
<li>Exit out of the System Settings application.</li>
<li>Run GYTB from your Home Menu. It should appear as a "gift".</li>
<li>GYTB should now register the custom badges it came with. Once that's done, press any button to exit the application.</li>
<li>Turn off your system.</li>
<li>Take out your SD card and insert it into your computer.</li>
<li>Go to <a class="external" href="https://themeplaza.art/badges" rel="" target="_blank">this website</a>.</li>
<li>Search for and/or find a sheet of badges you'd like. Click on it.<ul>
<li>I am not exactly sure why it shows a QR code when hovering over a sheet, but my guess is that it's because this is the same website that manages themes.</li>
</ul>
</li>
<li>Click on "Download" to download a ZIP archive of all the badges in that sheet.</li>
<li>Extract that ZIP archive using an unarchiving application of your choice. (i.e. WinRar, 7-Zip)</li>
<li>Take all the <code>.png</code> files from the extraction and drag them into the <code>badges</code> folder of your 3DS' SD card.</li>
<li>Eject your SD card and insert it back into your 3DS.</li>
<li>Turn on your 3DS.</li>
<li>Open the GYTB application from the Home Menu.</li>
<li>GYTB will now re-register its own custom badges on top of the ones you inserted into the badges folder.</li>
</ol>
<div class="admonition info">
<p>If you choose to add more badges after doing this once, GYTB is a one-time setup, meaning that to get more badges <strong>you have to start at step 14 the next time</strong>.</p>
</div>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="mods-generally-speaking">Mods (Generally Speaking)</h2>
<ol>
<li>Go to <a class="external" href="https://gamebanana.com/" rel="" target="_blank">GameBanana</a>, as they tend to have a lot of mods/texture packs for your game of choice.</li>
<li>Once you find the mod of your choice, make sure you click on it to see whether or not the developer of it said that it works on a real 3DS. a lot of the time, the mods they make may only work on Citra or other 3DS emulators. Another quick way to check if it only works on Citra is if the texture pack you downloaded is comprised of image files (such as <code>.png</code>), which don't work on a 3DS. </li>
<li>Turn on your system.</li>
<li>Open FBI.</li>
<li>Select "Titles".</li>
<li>Navigate to your game of choice, and note down the title ID the top screen should display. It will be important for later.</li>
<li>Press B to get to FBI's main menu.</li>
<li>Press Start to exit out of FBI.</li>
<li>Turn off your system.</li>
<li>Take out its SD card and insert it into your computer.</li>
<li>In a file explorer of your choice, navigate to the <code>/luma/</code> folder.</li>
<li>If a <code>titles</code> folder doesn't exist in it, create one.</li>
<li>Inside the new <code>titles</code> folder, create a folder titled with the title ID you noted down somewhere.</li>
<li>Inside the title id folder, create a folder called <code>RomFS</code>.</li>
<li>Place your mod files in this new <code>RomFS</code> folder.</li>
<li>Take your SD card out of your PC.</li>
<li>Insert your SD card back into your 3DS.</li>
<li>Turn your 3DS back on, but this time press and hold Select before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.</li>
<li>You should now see the Luma menu. In the Luma menu, make sure <code>Enable game patching</code> is enabled.</li>
<li>Press Start to reboot the system.</li>
<li>Whenever you boot up your game of choice, from now on it should be modded.</li>
</ol>
<h3 id="majoras-mask-3d-restoration-mod">Majora's Mask 3D Restoration Mod</h3>
<ol>
<li>Go to <a class="external" href="https://restoration.zora.re/" rel="" target="_blank">this website</a>.</li>
<li>Click the "Download for 3DS or Citra" button.</li>
<li>Click the "Download Project Restoration (the latest version)" button.</li>
<li>Use an unarchiving application of your choice (i.e. WinRar, 7-Zip) to extract the <code>.7z</code> file that you downloaded.</li>
<li>Turn on your system.</li>
<li>Open FBI.</li>
<li>Select "Titles".</li>
<li>Navigate to <em>Majora's Mask 3D</em>, and note down the title ID the top screen should display. It will be important for later.</li>
<li>Press B to get to FBI's main menu.</li>
<li>Press Start to exit out of FBI.</li>
<li>Turn off your system.</li>
<li>Take out its SD card and insert it into your computer.</li>
<li>In a file explorer of your choice, navigate to the <code>/luma/</code> folder.</li>
<li>If a <code>titles</code> folder doesn't exist in it, create one.</li>
<li>Inside the new <code>titles</code> folder, create a folder titled with the title ID you noted down somewhere.</li>
<li>When you extracted the <code>.7z</code> file, there should have been 3 folders called <code>v100</code>, <code>v101</code>, and <code>v110</code>. Start off with the <code>3ds</code> folder inside the <code>v100</code> folder. drag the <code>code.bps</code> and <code>exheader.bin</code> files from that folder and drop them in the title ID folder you just made.</li>
</ol>
<div class="admonition note">
<p><strong>OPTIONAL</strong>: If you would like, you can instead drag the <code>code_faster_aim.bps</code> file along with the <code>exheader.bin</code> file and drop that in the title ID folder. When it is dropped, however, make sure to rename it to <code>code.bps</code> within your SD card. This file will give you slightly faster aim when aiming with the Circle Pad.</p>
</div>
<div class="admonition warning">
<p class="admonition-title">Trial And Error</p>
<p>For this next few steps, you may see yourself repeatedly coming back to step 16 but instead of <code>/v100/3ds/</code> you would be using <code>/v101/3ds/</code> or <code>/v110/3ds/</code>. It's unfortunately just how it is. Some systems react to things differently.</p>
</div>
<ol start="17">
<li>Take your SD card out of your PC.</li>
<li>Insert your SD card back into your 3DS.</li>
<li>Turn your 3DS back on, but this time press and hold Select before pressing the power button, along with continuing to hold it after you've pressed the power button until you see something flash on screen.</li>
<li>You should now see the Luma menu. In the Luma menu, make sure <code>Enable game patching</code> is enabled.</li>
<li>Press Start to reboot the system.</li>
<li>Whenever you boot up <em>MM3D</em>, you will know that the game is modded if there's a sound that plays immediately after opening the application.</li>
</ol>
<div class="admonition note">
<p>If you do not hear that sound, look through the "Trial And Error" warning and start from there.</p>
</div>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="streaming-3ds-games-to-azahar-emulator">Streaming 3DS Games To Azahar Emulator</h2>
<div class="admonition info">
<p class="admonition-title">What This Means</p>
<p>Your 3DS will store information about the games you play to its internal storage. An emulator acts as a middleman, making your computer behave like the old console so that the games run as if you were playing them on the original system. There should be no reason why an emulator cannot access storage data the same way an actual 3DS can, since an emulator is already trying to fool your computer into thinking it is a 3DS. This is where Artic Base comes in. It allows you to send game information from your 3DS over the internet to your computer for it to be used in an emulator, which in this case is Azahar, as it is currently the best 3DS emulator for PCs and Android devices.</p>
</div>
<div class="admonition warning">
<p class="admonition-title">Ups And Downs</p>
<p>There are many up sides to using Artic Base. You can essentially use your 3DS like a Nintendo Switch in the sense that you can play handheld at a lower fidelity and performance, and then use Artic Base to connect to your computer to play at a better fidelity and performance right where you left off. Or vice versa. The big downside to this, however, is that when connected to an emulator through Artic Base, loading times for games can range from 2-5 times longer. Additionally, if you have certain mods installed on your 3DS they may or may not work. This can only be checked through trial and error, since I can't seem to find good documentation on this issue.</p>
</div>
<ol>
<li>Open Universal Updater from your Home Menu.</li>
<li>Search for "Artic Base". The icon looks like an igloo.</li>
<li>You can choose whether you want to install the <code>.3dsx</code> version or the <code>.cia</code> version. Keep in mind, the <code>.3dsx</code> version is meant to be launched through The Homebrew Launcher, while the <code>.cia</code> version is meant to be launched through the Home Menu.</li>
</ol>
<div class="admonition note">
<p>For the sake of this guide, we will be installing the <code>.3dsx</code> version. Though, instructions shouldn't vary by much if you choose to go the other route. Only by means of how to access the Artic Base Server application.</p>
</div>
<ol start="4">
<li>Press Start to exit out of the Universal Updater once it's finished installing.</li>
<li>Go to your PC if you aren't there already while reading this.</li>
<li>Download the latest release of Azahar <a class="external" href="https://azahar-emu.org/pages/download/" rel="" target="_blank">here</a>. If on Windows, the differences between MSVC and MSYS2 aren't something the average person would understand, so just trust me when I say download the MSVC version.</li>
<li>Once Azahar is downloaded, extract the archive the download should've come in. You should see a folder emerge from that archive.</li>
<li>Inside this folder, you should see an Azahar application. The other stuff is irrelevant. Just drag and drop that application binary to wherever you see fit. Note that when I say "binary", this can mean a <code>.exe</code> file or a <code>.app</code> file or a <code>.AppImage</code> file depending on your operating system.</li>
<li>Download the <code>.3dsx</code> file from the latest release of <a class="external" href="https://github.com/azahar-emu/ArticSetupTool/releases/latest" rel="" target="_blank">this GitHub repository</a>.</li>
<li>Turn off your 3DS.</li>
<li>Take out its SD card and insert it into your computer.</li>
<li>Drag and drop that <code>.3dsx</code> file you just downloaded into your <code>3ds</code> folder.</li>
<li>Take your SD card out of your PC.</li>
</ol>
<div class="admonition warning">
<p>Make sure you do it safely by manually clicking eject on the file explorer, as we do not want to risk corrupting your files!</p>
</div>
<ol start="14">
<li>Turn on your 3DS</li>
<li>Open The Homebrew Launcher.</li>
<li>Navigate to Azahar Artic Setup Tool and select it.</li>
<li>Press A and wait for a few seconds. The top screen will now display an IP address with a port next to it. (Format: <a class="external" href="http://xxx.xxx.xxx.xxx/" rel="" target="_blank">XXX.XXX.XXX.XXX</a>:PORT).</li>
<li>Open the Azahar application binary. Set it up as you'd like.</li>
</ol>
<div class="admonition info">
<p class="admonition-title">Regarding Emulators</p>
<p>in our lovely Discord server, I have made it so our fantastic bot can give you a detailed tutorial on how to set up a multitude of emulators. For our case, whenever the bot is online please type "!w emulation 3ds" (without the quotes) in one of the command's permitted channels for information on how to set up the preferred 3DS emulator on a computer.</p>
</div>
<ol start="19">
<li>Click on "File &gt; Set Up System Files..."</li>
<li>Enter in that IP address you see on your top screen.</li>
<li>Press "OK". Give it a minute, as Azahar is transferring information from your console to your PC over the internet.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">In Case Of Curiousity</p>
<p>The information being transferred here is actually the unique files your 3DS stores within its NAND that identify it among others. Essentially, what Nintendo would think we're doing here is cloning your 3DS. Pretty neat! Normally, you'd need something like a System Transfer to use the same credentials and whatnot for your NNID, but since those identifiers are now doubled and in 2 separate places your 3DS has now effectively been cloned. Note that your Friend Code and your friends list would not carry over.</p>
</div>
<ol start="22">
<li>You will eventually see the System Settings application open. This is normal. It will prompt you to update your system version; please do so. </li>
<li>Wait for this update to finish. Once finished you should be booted back into the main Azahar UI.</li>
<li>On your 3DS, press Start. You will be booted back into the Home Menu.</li>
<li>Re-open The Homebrew Launcher.</li>
<li>Navigate to Artic Base and select it.</li>
<li>Press A and wait a few seconds.</li>
<li>Once the system finishes reloading, press the Home button to suspend The Homebrew Launcher. Close out of it.</li>
<li>Open a 3DS game of your choice. You should see that as the Nintendo 3DS splash screen shows up, a small flash of blue should appear on screen.</li>
<li>The top screen will now display an IP address with a port next to it. (Format: <a class="external" href="http://xxx.xxx.xxx.xxx/" rel="" target="_blank">XXX.XXX.XXX.XXX</a>:PORT).</li>
<li>Back on your PC, click on File -&gt; Connect to Artic Base.</li>
<li>Enter your IP address and port number exactly as you see it on your 3DS' top screen into the emulator's textbox.</li>
<li>Give it some time, and your game will now be streamed to your emulator. To exit out, just press Start on your 3DS.</li>
</ol>
<p>"This is kind of tedious!" you might say. And you'd be right. Which is why once you've set up everything and if you'd like to stream a game to Azahar again, you can start from step 25.</p>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="ftpd-file-transfer-over-internet">FTPD (File Transfer Over Internet)</h2>
<div class="admonition info">
<p class="admonition-title">What Is FTPD?</p>
<p>The "New" variant of 3DS systems can wirelessly transfer files between a Windows computer running Windows 7 or later from the System Settings application -&gt; Data Management -&gt; microSD Management. Once you start up the instance following the on screen prompts, you could access your 3DS' files from the Windows file explorer in its Network section. But what if you don't have a "New" variant system and/or don't have a Windows device, yet you want to wirelessly transfer files between your computer and 3DS? This is where FTPD comes in. It allows you to do exactly that.</p>
</div>
<div class="admonition warning">
<p class="admonition-title">Take Into Consideration</p>
<p>From my understanding, as of 1/21/2025 or maybe some time before as well, the FTPD application now comes bundled with the process of modding your system. If you're modding your system since then, you can skip steps 1-4.</p>
</div>
<ol>
<li>Open Universal Updater from your Home Menu.</li>
<li>Search for "FTPD". The icon looks like a black square that says "FTPD" in giant green text.</li>
<li>You can choose whether you want to install the <code>.3dsx</code> version or the <code>.cia</code> version. Keep in mind, the <code>.3dsx</code> version is meant to be launched through The Homebrew Launcher, while the <code>.cia</code> version is meant to be launched through the Home Menu.</li>
</ol>
<div class="admonition note">
<p>For the sake of this guide, we will be installing the <code>.cia</code> version. Though, instructions shouldn't vary by much if you choose to go the other route. Only by means of how to access the FTPD application.</p>
</div>
<ol start="4">
<li>Once it's finished installing, press Start to close out of the Universal Updater.</li>
<li>Open the FTPD application from your Home Menu.</li>
<li>The top screen should have an IP address and port number at the top. This will be in the format of <a class="external" href="http://xxx.xxx.xxx.xxx/" rel="" target="_blank">XXX.XXX.XXX.XXX</a>:(PORT). Keep note of it.</li>
<li>Put your 3DS aside for now but leave it on with the screens opened.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">Divergence</p>
<p>This section will now divide into 2 sections for instructions depending on your operating sytem.</p>
</div>
<h3 id="for-windowsmacos">For Windows/MacOS</h3>
<ol start="8">
<li>Go to <a class="external" href="https://cyberduck.io/download/" rel="" target="_blank">this website</a>.</li>
<li>Download for your operating system.</li>
<li>On Windows, run through the installer for the program and then open Cyberduck. On MacOS, unarchive the <code>.zip</code> file you downloaded using an unarchiver of your choice (the MacOS default one works just fine), drag and drop <code>Cyberduck.app</code> into your Applications pin in Finder, go to the Applications pin, right click on <code>Cyberduck.app</code>, select "Open", then confirm that you want to open the application.</li>
<li>In Cyberduck, click "Open Connection" at the top.</li>
<li>At the dropdown on the top, make sure "FTP (File Transfer Protocol)" is selected.</li>
<li>In the text box for "Server", enter the IP address on your 3DS.</li>
<li>In the box for "Port", enter the port number on your 3DS.</li>
<li>Cyberduck will now connect to your 3DS' files directly. Open a window in your file explorer from here.</li>
<li>Use both Cyberduck and the window you just opened to do whatever dragging and dropping of files in and out of your SD card that you need to do. Note that because we are wirelessly transferring files here, files may take longer to transfer in and out of your system.</li>
<li>Once finished, close out of Cyberduck. It may prompt you to pay money, in which case just click "Later". Cyberduck will always be free to you, and you paying money is only to support the developers.</li>
<li>Back on your 3DS, press Start to exit out of FTPD.</li>
</ol>
<h3 id="for-linux">For Linux</h3>
<ol start="8">
<li>In your file explorer (in my case, Dolphin on my Steam Deck), right click on the file path at the top and make sure "Show file path" is selected.</li>
<li>Click on the file path to open a textbox displaying the full file path.</li>
<li>Press Ctrl+A to highlight the entire thing and then Backspace to delete it all.</li>
<li>Enter the following into the file path bar: <code>ftp://(the ip address):(the port number)</code>. You should then almost instantly be able to access the files on your SD card.</li>
<li>Open a new tab or window of Dolphin. Use both of these tabs/windows to do whatever dragging and dropping of files in and out of your SD card that you need to do. Note that because we are wirelessly transferring files here, files may take longer to transfer in and out of your system.</li>
<li>Once finished, close out of the tab/window that contains your 3DS' files and the other tab/window containing files on your Linux computer.</li>
<li>Back on your 3DS, press Start to exit out of FTPD. </li>
</ol>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="using-external-controllers">Using External Controllers</h2>
<div class="admonition warning">
<p class="admonition-title">Assumptions Made!</p>
<ul>
<li><strong>This guide assumes that you have a Windows PC</strong>! The software that you will need is Windows dependant, using .dll and .exe files. I'm not sure if you can run these programs under a compatability layer like Proton on Linux or Whisky on MacOS, but for the sake of working 100% of the time please use a Windows PC for this.</li>
<li><strong>This guide assumes that you are going to be using an Xbox controller</strong>! This works with a tool called XInput, which comes with Xbox controllers. If you do not have an Xbox controller, you can use a tool like <a class="external" href="https://github.com/x360ce/x360ce/releases/" rel="" target="_blank">x360ce</a> to remap your buttons accordingly, or open the software outlined below as a Non-Steam Game to utilize Steam Input. This guide will not go over either of these processes.</li>
</ul>
</div>
<div class="admonition info">
<p class="admonition-title">You Can Use One?</p>
<p>Luma3DS allows for interoperability between it and a 3rd-party application called InputRedirection. This process will allow you to connect your 3DS to your PC over your local internet connection, at which point you can connect your controller to your PC and operate your 3DS from there. You may then use your external controller for use on your 3DS. This can be for accessibility reasons (ie. if your hands cramp up after long sessions of play), or for better use with games that have wonkier control schemes (ie. Smash Bros, Kid Icarus Uprising, MH4U/G).</p>
</div>
<ol>
<li>Connect your controller to your PC. This can be done either via Bluetooth or through a wired connection.</li>
<li>Download the latest <code>.zip</code> file of the required application from <a class="external" href="https://github.com/TuxSH/InputRedirectionClient-Qt/releases/" rel="" target="_blank">here</a>. You are looking for the <code>.zip</code> file that is NOT the source code; look for the keyword "QT" in the<code>.zip</code> file you would download.</li>
<li>Extract this <code>.zip</code> file to a location of your choice on your PC.</li>
<li>Open <code>InputRedirectionClient-QT.exe</code>.</li>
<li>Turn on your 3DS.</li>
<li>Once it boots up, press L + D-Pad Down + Select.</li>
<li>Navigate to "Miscellaneous options..." and select it.</li>
<li>Navigate to "Start InputRedirection" and select it.</li>
<li>You will see that on the top right corner of your touch screen, there will be an IP address. Type this into the box for the IP address in the <code>.exe</code> file you opened in step 4.</li>
<li>If you do not like how some of the controls are laid out, you can remap them in the "Settings" of the <code>.exe</code> application.</li>
<li>You are free to game on your controller!</li>
</ol>
<p>If you'd like to stop InputRedirection when finished playing, simply repeat steps 6-8.</p>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="patching-dsi-firmware">Patching DS(i) Firmware</h2>
<div class="admonition info">
<p class="admonition-title">How "DS(i) Mode" Works</p>
<p>The layman approach of explaining how the 3DS is able to play DS games is that "it contains DS hardware inside of it". This is mostly true, but not entirely. While it's not literally a DS motherboard soldered inside, the 3DS does contain hardware that's capable of natively running DS software. Specifically, it includes processors that are compatible with the ARM9 and ARM7 chips used in the original DS. When you boot a DS game, the 3DS essentially powers down its "modern" firmware and enters a firmware called "DS(i) Mode", which closely mimics the DS (and DSi) environment using that hardware-level compatibility.</p>
</div>
<div class="admonition info">
<p class="admonition-title">How DS(i) Mode Renders Games</p>
<p>In DS(i) mode, the 3DS behaves as if it were a DS or DSi, with most of the newer system's features disabled. Things like wireless, screen brightness controls, and even some SD card access are limited or rerouted through legacy systems. However, DS(i) Mode does take a few liberties when rendering games. For example, even though you have access to the Circle Pad on a 3DS, it’s essentially useless for DS games, as it just maps to the D-pad’s inputs. Thus, you’ll still be using the D-pad to control movement. One "crime" I find particularly egregious is that DS(i) Mode tries to take advantage of the 3DS' larger screens and resolution when playing DS games. It upscales the original DS resolution (256x192) to a 5:3 ratio (400x240) for the 3DS' displays. This upscaling can lead to a lot of blur and distortion, especially on XL variants of the 3DS. While Nintendo did provide an option to fix this (by holding Start or Select as the system boots into DS(i) Mode) which would force the game to render at the original 4:3 resolution, many people didn’t know about it as Nintendo either didn’t market the feature well or left it as a hidden option. <strong>This guide will focus on how to make it so that DS(i) Mode will automatically render games at the original resolution</strong>. Please keep in mind, however, that if you'd like you can mess around with the homebrew we will be installing.</p>
</div>
<ol>
<li>Open Universal Updater from your Home Menu.</li>
<li>Search for "TWPatch". The icon looks like Mario standing next to a purple brick with "TWL" in big blue text right above them.</li>
<li>Download "TWPatch.3dsx".</li>
</ol>
<div class="admonition note">
<p>If you would like, you may choose to install the <code>.cia</code> version to launch through the Home Menu. However, for the sake of the tutorial we will be sticking with the <code>.3dsx</code> version.</p>
</div>
<ol start="4">
<li>Press Start to exit the Universal Updater.</li>
<li>Open The Homebrew Launcher.</li>
<li>Navigate to <code>TWPatch.3dsx</code> and select it.</li>
<li>Press Y + B once the application opens.</li>
<li>Press A to toggle on "Invert START+SELECT function".</li>
<li>Press B.</li>
<li>Hold Start to begin the patch process. This may take a few minutes, so get a quick drink of water! :)</li>
<li>Once the patching is finished, hold Select to exit out to The Homebrew Launcher.</li>
<li>Press the Home button to exit out to the Home Menu.</li>
<li>Open up your DS game of choice.</li>
<li>Enjoy better clarity! </li>
</ol>
<p><a href="../3ds/">Back to Top</a><br/>
<a href="../">Back to Base</a></p></div>
</article>