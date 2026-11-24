<article>
<div><h1 id="rip-bozotendo-steam-deck">RIP Bozotendo, Steam Deck</h1>
<div class="admonition warning">
<p class="admonition-title">Important Warning</p>
<p>Until I say it isn't, <strong>this megathread will continually be in a state of WIP</strong>! I am continually working to add things to here that may be pertinent to us. If you want information on something, please let me know. I will try my best to update this thread as needed or as I come along certain information.</p>
</div>
<h2 id="table-of-contents-you-are-here">Table of Contents (You are here)</h2>
<div class="toc">
<ol>
<li><a href="#table-of-contents-you-are-here">Table of Contents (You are here)</a></li>
<li><a href="#disclaimers">Disclaimers</a></li>
<li><a href="#recommended-settings-tweaks">Recommended Settings Tweaks</a></li>
<li><a href="#decky-loader">Decky Loader</a><ol>
<li><a href="#recommended-decky-plugins-store">Recommended Decky Plugins (Store)</a><ol>
<li><a href="#protondb-badges">ProtonDB Badges</a></li>
<li><a href="#powertools">PowerTools</a></li>
<li><a href="#steamgriddb">SteamGridDB</a></li>
<li><a href="#css-loader">CSS Loader</a><ol>
<li><a href="#simpledeck">"SimpleDeck"</a></li>
</ol>
</li>
<li><a href="#audio-loader">Audio Loader</a></li>
<li><a href="#tabmaster">TabMaster</a></li>
</ol>
</li>
<li><a href="#recommended-decky-plugins-non-store">Recommended Decky Plugins (Non-Store)</a><ol>
<li><a href="#prerequisite-turning-on-developer-mode-in-decky-settings">(Prerequisite) Turning on Developer Mode in Decky Settings</a></li>
<li><a href="#decky-multiframegen-wip">Decky MultiFramegen (WIP)</a></li>
<li><a href="#game-theme-music">Game Theme Music</a></li>
<li><a href="#anyaspectratio-wip">AnyAspectRatio (WIP)</a></li>
</ol>
</li>
</ol>
</li>
<li><a href="#vesktop-discord">Vesktop (Discord)</a></li>
<li><a href="#emudeck">EmuDeck</a><ol>
<li><a href="#onboardinginitial-setup">Onboarding/Initial Setup</a></li>
<li><a href="#gyroscopedsu">GyroscopeDSU</a></li>
<li><a href="#emudecky">EmuDecky</a></li>
<li><a href="#emudeck-compressor">EmuDeck Compressor</a></li>
<li><a href="#cloud-services">Cloud Services</a></li>
<li><a href="#once-finished-with-rom-compression-andor-cloud-services">Once Finished With ROM Compression And/Or Cloud Services</a></li>
</ol>
</li>
<li><a href="#unofficial-versions-of-proton">Unofficial Versions of Proton</a><ol>
<li><a href="#method-1-wine-cellar">Method 1 (Wine Cellar)</a></li>
<li><a href="#method-2-protonup-qt">Method 2 (ProtonUp-QT)</a></li>
</ol>
</li>
<li><a href="#epicgogprime-games-on-deck">Epic/GOG/Prime Games On Deck</a><ol>
<li><a href="#method-1-unifideck">Method 1 (Unifideck)</a></li>
<li><a href="#method-2-heroic-games-launcher">Method 2 (Heroic Games Launcher)</a></li>
</ol>
</li>
<li><a href="#chiaki-ng-playstation-remote-play">chiaki-ng (PlayStation Remote Play)</a></li>
<li><a href="#kde-connect-wireless-file-transfer">KDE Connect (Wireless File Transfer)</a></li>
<li><a href="#using-cheats-in-pc-games">Using Cheats In PC Games</a></li>
<li><a href="#protontricks">Protontricks</a></li>
<li><a href="#vortex-mod-manager">Vortex Mod Manager</a></li>
<li><a href="#achievement-manager">Achievement Manager</a></li>
</ol>
</div>
<h2 id="disclaimers">Disclaimers</h2>
<ul>
<li>The Steam Deck runs a "distro" of Linux called SteamOS. I know that to a new person, Linux seems scary. But SteamOS is very beginner friendly to work with. You'll have a hang of it just by following this guide (which is meant to be read sequentially).<ul>
<li>This comes at a downside where some games that require the use of an anti-cheat, such as Valorant, will <strong>NOT</strong> work on the Steam Deck. While the developers of these games can simply just "flip a switch" to allow Linux gamers to play these games, they do not allow it for the time being. If you wanted to play these games on your Deck, I'm so sorry. Don't fret, however, since there is <a class="external" href="https://areweanticheatyet.com/" rel="" target="_blank">this website</a> that tells you whether an anti-cheat game will work on Linux!</li>
</ul>
</li>
<li><strong>The Steam Deck's Desktop Mode is your friend!</strong> We will be using it frequently to install tools needed to maximize your Steam Deck's potential.</li>
<li>The Steam Deck doesn't have a "proper" process for hacking one like, say, a Wii or 3DS has, where it has a sort of indescribable hacker-man feel to it. But, you can do some pretty cool stuff outside of what Valve normally would let you do with a Steam Deck.<ul>
<li>Just know that since we will be doing things in Desktop Mode, while everything is doable without a mouse and keyboard it is recommended that you use one for navigating it. This can be done by docking your Steam Deck into a dock, or by using Steam Link to stream your Steam Deck's display to your PC.<ul>
<li>Should you choose not to utilize a mouse and keyboard, the Steam deck gives you functionality within the device's hardware. The way clicking works is kind of counterintuitive but in your hands it will make sense.<ol>
<li>Left click is by either pressing down on the right track pad or by pressing R2. </li>
<li>Right click is by pressing L2.</li>
<li>Your mouse is controlled by either the right track pad or the right joystick. Alternatively, you can try using the touchscreen to interact with things on screen.</li>
<li>The scroll wheel is controlled by the left track pad and the left joystick.</li>
<li>To invoke the on-screen keyboard, press Steam + X on your Deck.</li>
</ol>
</li>
</ul>
</li>
</ul>
</li>
<li>Fun fact: In Desktop Mode, if you right click on an application's icon in either Dolphin (the file explorer) or in the start menu, you can add that application to Steam as a Non-Steam game. This will allow you to access that application back in Gaming Mode. A good use case for this may be for adding applications like Discord (Vesktop, as the more commonly utilized Discord client for Deck users is called. More on this later.) or Firefox to Steam so that you can quickly navigate to them from Gaming Mode instead of having to manually go to Desktop Mode every time.</li>
<li>You may see reference to something called "Proton" in this part of the megathread. Proton is an open source tool created by Valve which allows for Linux to create Windows environments for your Windows Steam games to run underneath Linux. Because of its open source nature, other people have taken it upon themselves to create their own versions of Proton so that these new versions of Proton can do what Valve's doesn't. More on this later.<ul>
<li>Speaking of Proton, the way it works is that the Steam Deck will create fake Windows <code>C:\</code> drives for your each of your individual games to work in, which can take up anywhere between 255 MB to ~1.5 GB of storage. Additionally, games will also install compiling their own individual shader caches, which can take up more storage in a range of between a few kilobytes to upwards of 15 GIGABYTES. In lieu of this, <strong>I would advise against buying a 64 GB Steam Deck unless you plan on upgrading the SSD</strong>! Additionally, to play it safe I'd always caution <strong>not to fill up the storage on your Steam Deck and always leave around 10-15 GB free AT ALL TIMES</strong>!<ul>
<li>If you'd like to learn how to upgrade the SSD on your Steam Deck I will not be going over it on this Rentry, but you can <a class="external" href="https://youtu.be/YF2Dy7Ol_Ew" rel="" target="_blank">watch this YouTube video</a>. If you're going this route I'd recommend getting <strong>at least a 1 TB SSD</strong> to go with your Deck, but <strong>no more than 2 TB</strong>!</li>
</ul>
</li>
</ul>
</li>
</ul>
<p><a href="../steam-deck/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="recommended-settings-tweaks">Recommended Settings Tweaks</h2>
<p>Here's some settings you should tweak on your Deck to make it more seamless and console-like!</p>
<ol>
<li>While in the Steam UI, press the Steam button.</li>
<li>Navigate to "Settings" and select it.</li>
<li>Navigate to "Display".</li>
<li>In the Display settings, navigate to "Automatically Scale User Interface" and make sure it is toggled on. This scales the UI to your TV when docked.</li>
<li>If you'd like to reduce blue light emission when playing at night, navigate to "Schedule Night Mode" and make sure it is toggled on. Use the drop downs below to schedule times in which Night Mode is active.</li>
<li>Navigate to Maximum Game Resolution. In the drop down, set the resolution to "Native". This auto-adjusts game resolution when docked.</li>
<li>Press B.</li>
<li>Navigate to "Power" and select it. You should have your cursor over "Battery Percentage". Make sure it is toggled on.</li>
<li>Right below that toggle, make sure "Enable battery charging limit" is toggled on. This can be helpful if you're frequently docking your Steam Deck to an external display or if you play a lot while the Deck is charging as to not degrade the battery's health over time. Use the slider below to set the charge limit; I recommend 80%. <em>Note: it may take some getting used to seeing that 80% as "fully charged".</em></li>
<li>Navigate to "When plugged in, dim after" and select 20 minutes from the drop down.</li>
<li>Navigate to "On battery power, dim after" and select 5 minutes from the drop down.</li>
<li>Navigate to "When plugged in, sleep after" and select "Disabled" from the drop down.</li>
<li>Navigate to "On battery power, sleep after" and select 20 minutes from the drop down.</li>
<li>Press B.</li>
<li>Navigate to "Downloads" and select it.</li>
<li>Navigate to "Limit download speed" and make sure it is toggled on.</li>
<li>In the box below, set the limit to <code>10000000</code> Kbps. This gets rid of Steam's internal bandwidth cap for game downloads!</li>
<li>Navigate to "Allow downloads during gameplay" and make sure it is toggled on. <em>Note: for more intensive games, having downloads going in the background while playing may hinder performance.</em></li>
<li>Press B.</li>
<li>Navigate to "Game Recording" and select it.</li>
<li>From the three choices below, choose "Record Manually". Now, you can press Steam + A to start/stop recordings in game. If you'd like you can navigate further down to "Record Microphone" and toggle that on in case you want to record your voice as well.</li>
<li>Press B twice.</li>
</ol>
<h2 id="decky-loader">Decky Loader</h2>
<div class="admonition info">
<p class="admonition-title">About Decky Loader</p>
<p>Decky Loader is a plugin loader directly for your Steam Deck when it is in Gaming Mode. It can do a whole range of things, such as giving you a range of tools to fine tune how the hardware works or changing how Gaming Mode looks like to you. Highly customizable with a very simply set up process.</p>
</div>
<ol>
<li>While in the Steam UI, press and hold down on the Power button until you see a menu appear.</li>
<li>Navigate to "Switch to Desktop" and select it. Go through any set up stuff that appears on screen about KDE Plasma (the name for the desktop environment) if you've never been in Desktop Mode.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">Wallet Information</p>
<p>If you unplug your Deck from the charger while in Desktop Mode, it may ask you to set up wallet information. No, it won't ask you for credit card information. Just click the option for the "classic file".</p>
</div>
<ol start="3">
<li>Click on the Firefox icon in the Dock. Go through the setup process. Firefox is the default browser on your Deck.</li>
<li>Go to <a class="external" href="https://decky.xyz/" rel="" target="_blank">https://decky.xyz/</a>.</li>
<li>Right click the "Download" button at the top right of the page and left click "Save Link As...".</li>
<li>In the file explorer, select the Desktop. Do NOT save yet!</li>
<li>Get rid of the <code>.download</code> extension in the file name bar. (<code>decky_installer.desktop.download</code> should now become <code>decky_installer.desktop</code>).</li>
<li>Once that's done, click "Save".</li>
<li>Close out of Firefox.</li>
<li>In the desktop, double click the "Install Decky" icon. Press "Continue" or "Execute" after that if prompted.</li>
<li>It may ask you to temporarily set your sudo password to "Decky!". Your "sudo" password is the password running tasks in what is the equivalent of running as administrator on Windows. (<strong>S</strong>uper <strong>U</strong>ser <strong>DO</strong>). Let it.</li>
<li>Ask it to install the "release" version. You won't need the "prerelease" version unless you know what you're doing.</li>
<li>Once it's finished installing, close out of the Konsole window the script was running in.</li>
<li>Double click on "Return to Gaming Mode" in the desktop.</li>
<li>In Gaming Mode, press the 3dots button ("Quick Access Menu", as it'll be called here after). You should see an icon that looks like a wall plug. Navigate to it.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">Decky Icon Not Showing?</p>
<p>If you don't see that wall plug icon, give it a bit. And if still not, press and hold the power button and restart the device.</p>
</div>
<ol start="16">
<li>You should see a store icon at the top right. Navigate to it and select it.</li>
<li>Install whatever plugins you'd like from their store.</li>
</ol>
<h3 id="recommended-decky-plugins-store">Recommended Decky Plugins (Store)</h3>
<h4 id="protondb-badges">ProtonDB Badges</h4>
<p>Sometimes, whatever Valve says is Deck "Verified" or Deck "Playable" or Deck "Unsupported" is incorrect. Adding this badge to the game's Gaming Mode start page allows you to click navigate and select it to gain Linux gaming community insight on how to properly configure the game of your choice to work with your Linux device.</p>
<p>It has been helpful to me at least where a game in my Library is marked as Deck "Unsupported" by Valve. However, ProtonDB was able to tell me to get a custom version of Proton to get this game working with my Deck. (More on custom versions of Proton later).</p>
<h4 id="powertools">PowerTools</h4>
<p>If you know what you are doing, you can directly monitor CPU and GPU usage through this plugin to optimize performance in certain situations. </p>
<h4 id="steamgriddb">SteamGridDB</h4>
<p>This tool is for adding artwork for whatever game/program you have listed on Steam, be they official or unofficial.</p>
<ol>
<li>Hover a title in your Library or Home and press the Options button (looks like 3 lines on top of each other next to Y).</li>
<li>Select "Change Artwork". If it doesn't appear, press B and then press Options while hovering over the title again.</li>
<li>Choose whatever artwork you'd like. </li>
<li>Restart after you're done as prompted.</li>
</ol>
<h4 id="css-loader">CSS Loader</h4>
<p>This one is probably the most intricate plugin on its own. It allows you to completely customize the look of your Gaming Mode UI. It has its own plugins to extend to this plugin.</p>
<ol>
<li>In the Decky plugin menu from the Quick Access Menu, navigate to "CSS Loader" and select it.</li>
<li>Navigate to the Download icon at the top right and select it.</li>
<li>Install whatever CSS theme you want.</li>
<li>Once that's finished, select the gear icon next to the "Reinstall" button.</li>
<li>Enable the theme you just downloaded by simply pressing A.</li>
</ol>
<h5 id="simpledeck">"SimpleDeck"</h5>
<p>Do you want a quick way to install as many themes as possible? I've got the right thing for you!</p>
<ol>
<li>In the Decky plugin menu from the Quick Access Menu, navigate to "CSS Loader" and select it.</li>
<li>Navigate to the Download icon at the top right and select it.</li>
<li>Set the filter to "Profile".</li>
<li>Select "SimpleDeck". It should be by me, obviously. :)</li>
<li>Select "Install".</li>
<li>Once that's finished, select the gear icon next to the "Reinstall" button.</li>
<li>Enable the profile you just downloaded by simply pressing A.</li>
</ol>
<h4 id="audio-loader">Audio Loader</h4>
<p>This plugin lets you change the UI sounds of Gaming Mode along with add background music to Gaming Mode in case you ever feel bored of there being no music. This plugin is made by the same people who made CSS Loader. </p>
<ol>
<li>In the Decky plugin menu from the Quick Access Menu, navigate to "Audio Loader" and select it.</li>
<li>Navigate to the Download icon at the top right and select it.</li>
<li>Navigate to "Manage Packs" and select it.</li>
<li>Set the filter to whatever you are looking for. If you are looking for UI SFX, select "Audio". If you are looking for background music, select "Music".</li>
<li>Find some audio you might like and select it.</li>
<li>Select "Install". A vinyl should start spinning to indicate it is installing.</li>
<li>Once the vinyl stops spinning, press B twice to back out of the Audio Loader store.</li>
<li>Go back to the Decky plugin menu from the Quick Access Menu, navigate to "Audio Loader" and select it.</li>
<li>Select the respective packs of audio you just downloaded from the correct dropdowns.</li>
<li>Press B twice to back out of the Quick Access Menu.</li>
<li>Press the button to access the Quick Access Menu.</li>
<li>Navigate to the Decky plugin menu.</li>
<li>Navigate to "Audio Loader" and select it.</li>
<li>Navigate to "Enable Legacy Features" and select it.</li>
<li>From both dropdowns, select whichever sounds you downloaded.</li>
<li>Close out of the Quick Access Menu.</li>
</ol>
<p>If you want some recommendations, I have my Deck set to have "Dreamy SFX" and "Dreamy Ambience" for the UI sounds and the background music respectfully. Though, I do sometimes change it up to have "azure sounds" and "azure tides" as the respective audio playing in the background. Do note, however, that he reason why background music is considered a "Legacy Feature" is that the implementation is buggy and the developers of the plugin simply do not want to fix that. One such bug is that <strong>if you wake up your Deck from Sleep Mode the background music will NOT immediately start playing!</strong> <em>This can be fixed, however,</em> by simply repeating steps 11-16 but only retoggling the dropdown for background music. Alternatively, you can set up the Game Theme Music plugin (detailed further on) and a login PIN through the Settings, in order to then pre-emptively set your Deck to Sleep Mode as it is in the info page for a game in order for this music to play once you simply press B to exit out.</p>
<h4 id="tabmaster">TabMaster</h4>
<p>This plugin lets you customize what tabs in your library you will see in the Library section of the Deck's UI.</p>
<ol>
<li>In the Library section of your Deck's UI, navigate to the top bar where all of the tabs are.</li>
<li>Press the Menu button.</li>
<li>Customize as you'd like!</li>
</ol>
<h3 id="recommended-decky-plugins-non-store">Recommended Decky Plugins (Non-Store)</h3>
<div class="admonition info">
<p class="admonition-title">What Does This Mean?</p>
<p>There are tons of Decky plugins out there that are not on their official store. It takes time for a proper review process from the Decky team that people don't want to go through, or these plugins don't fit under guidelines proposed by the Loader team. Could be one reason or another. Here are a few plugins I think are worth looking at that are past the store. I've also included the respective GitHub links to downloading these plugins. From Desktop Mode, you will need to download them to a folder of your choice. (Most likely, the downloads folder).</p>
</div>
<h4 id="prerequisite-turning-on-developer-mode-in-decky-settings">(Prerequisite) Turning on Developer Mode in Decky Settings</h4>
<div class="admonition info">
<p class="admonition-title">Developer Mode</p>
<p>This allows you to install a plugin from a <code>.zip</code> file from outside the Store. Don't worry, we won't actually be "developing" anything. The intention behind this is so that people who <em>do</em> make plugins can quickly test their builds of it before going through the review process, but this feature is available to anyone who wants to install 3rd-party plugins.</p>
</div>
<ol>
<li>In Gaming Mode, press the Quick Access Menu button. You should see an icon that looks like a wall plug. Navigate to it.</li>
<li>You should see a cog icon at the top right. Navigate to it and select it.</li>
<li>In the General tab of the settings, navigate to the toggle for "Developer mode" and toggle it on.</li>
</ol>
<p>There should now be a tab in the settings called "Developer", where the first option is "Install Plugin from ZIP File". This is how you will be installing these plugins. The first time you select the "Browse..." button there will be a 5 second cooldown on a warning that these plugins would be "use at your own risk" before moving forward, but after those initial 5 seconds that popup just becomes a warning from then on out. All plugins below will assume that from the GitHub links for them, you downloaded these plugins and "Browse"d to install them.</p>
<h4 id="decky-multiframegen-wip">Decky MultiFramegen (WIP)</h4>
<p>If you are playing a heavy AAA game (for example, <em>Clair Obscur: Expedition 33</em>), you'll quickly notice that the Steam Deck may in fact be underpowered to handle the game at a usable frame rate while still looking good. Upscaling technology has been around for a while now as a tool PC gamers use to squeeze more performance out of their hardware. The way it usually works is by having the game render at a lower resolution (say, 480p), while an upscaling algorithm reconstructs the image at a higher resolution (for the Deck, it's 800p). This can usually increase your frame rates in-game without sacrificing too much visual quality.</p>
<p>Natively, the Steam Deck supports certain upscalers that games provide, such as AMD's FSR or Intel's XeSS. However, NVIDIA's DLSS normally requires NVIDIA hardware, and not every game supports the latest upscaling models. Thankfully, this plugin solves a lot of these issues. It lets you hijack the upscaling <code>.dll</code> files that certain games come installed with (particularly DirectX 12 games that support DLSS) and tell the game to use a different upscaling model instead, while it thinks it's still using the original one. This can potentially give you sharper visuals, better performance, or both.</p>
<p>Additionally, you may notice that even with better upscaling, the game may still not run at a high FPS. For example, when I tried running <em>Expedition 33</em> after playing around with upscaler models, I was only getting around a smooth 30 FPS. Not unplayable, but a smooth 60 FPS or higher would be nicer. This Decky plugin also allows you to use something called <strong>MAKO FrameGen</strong>, which generates artificial frames between real ones to give the illusion of getting a 2x, 3x, or even 4x multiplier to your FPS. There is a slight trade-off in input latency and occasional visual glitches, and it won't feel quite as responsive as a genuine higher frame rate, but it can make games look significantly smoother. "Download more FPS", if you want to keep it more layman-friendly.</p>
<div class="admonition info">
<p><a class="external" href="https://github.com/MWGIH/DeckyMultiFrameGen/releases/latest" rel="" target="_blank">https://github.com/MWGIH/DeckyMultiFrameGen/releases/latest</a></p>
</div>
<div class="admonition warning">
<p class="admonition-title">AI Disclosure</p>
<p>This plugin has an extensively documented use of how Claude and other AI agents are used during the development of this plugin. However, the person behind the plugin is also a seasoned developer with extensive credentials and coding knowledge that exceeds mine. As such, I would refrain from calling this plugin "vibe coded", but I think it is also fair to disclose that AI was used in the development of this plugin.</p>
</div>
<p><strong><em>WIP</em></strong> </p>
<h4 id="game-theme-music">Game Theme Music</h4>
<p>Do you remember how on the Wii, when you selected a channel from its UI it would play music before you launched the game? Well, with this plugin you can set music to play in your Steam game's page ("launch page" as I'll call them from here on) that opens up in order to launch a game! You know, that one page where you can see your activity and achievements with the giant Play button on it? That one. Do note that this also works with the launch pages for your Non-Steam games as well. This plugin should (partially) be made by me! :)</p>
<div class="admonition info">
<p><a class="external" href="https://github.com/MegalonVII/SDH-GameThemeMusic/releases/latest" rel="" target="_blank">https://github.com/MegalonVII/SDH-GameThemeMusic/releases/latest</a></p>
</div>
<div class="admonition warning">
<p class="admonition-title">About Store Version</p>
<p>I have this plugin on the official Decky store, but that version is <strong>outdated</strong>. Please use the GitHub one for now while I work to get that update on the store as well!</p>
</div>
<ol>
<li>Navigate to any game in your Library and select it. Do <em>NOT</em> select Play to launch it.</li>
<li>Navigate to the gear icon and select it.</li>
<li>Navigate to "Change Theme Music..." and select it.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">Not Appearing?</p>
<p>If you are attempting this after just waking up your Deck from Sleep Mode or anything relating to a power cycle, do note that this option will not appear in that settings menu you just pulled up. To remedy this, just press B and then A again.</p>
</div>
<ol start="4">
<li>You'll see a list of YouTube videos to choose from slowly populate the UI, though if you'd like to fine tune this selection you can edit the search parameter by simply pressing A. The onscreen keyboard will open up, so use that to search for something more specific. The default search parameter will be "(game title) Theme Music".</li>
<li>Navigate to a video you think is fitting. You can select "Play" to preview the video's audio just to hear how it sounds.</li>
<li>If you've found an audio you like, navigate to Download and select it. This can take a few short seconds to a few minutes, depending on how long the video is and how fast your internet speeds are.</li>
<li>Press B to go back to the game's launch page. You should now be able to hear the song you downloaded!</li>
</ol>
<h4 id="anyaspectratio-wip">AnyAspectRatio (WIP)</h4>
<p><strong><em>WIP</em></strong></p>
<p><a href="../steam-deck/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="vesktop-discord">Vesktop (Discord)</h2>
<div class="admonition info">
<p class="admonition-title">What Is Vesktop? Why Install?</p>
<p>Discord's main client is available for Linux, but it is very under supported. This is where Vesktop comes in. It is a modified Discord client with the Vencord mod already pre-installed. Vesktop allows you to add plugins to your Discord experience to enhance it infinitely. The main reason to install this is because of being able to join Discord voice chats while playing games on your Deck.</p>
</div>
<ol>
<li>While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.</li>
<li>Navigate to "Switch to Desktop" and select it.</li>
<li>On the Dock, open Firefox to this exact guide.</li>
<li>Copy the following script made by yours truly:<br/>
<code>curl -fsSL https://gist.githubusercontent.com/MegalonVII/cc69d04c666a3fd420ebce010cab36b8/raw/steamdeck-vesktop-appimage-install.sh | bash</code></li>
<li>Press on L5 on your Deck. This is the bottom most back button on the left side of your Deck. This will open up the Start Menu. Additionally, you can just tap on it from the Dock.</li>
<li>Go to the "System" section of the Start Menu.</li>
<li>Open Konsole.</li>
<li>Click on "Paste" at the top right of the window.</li>
<li>Press A.</li>
<li>Once the script is done, close out of the Konsole window. You should see an icon for Vesktop on the Desktop, but we will not be utilizing this for now. This is just for future use.</li>
<li>Press on L5 on your Deck to open the Start Menu again.</li>
<li>Go to the "Internet" section of the Start Menu.</li>
<li>Navigate to the icon for Vesktop. Right click on it.</li>
<li>Left click on "Add to Steam". This will be helpful for later, as now this program is in our Steam Library as a Non-Steam game.</li>
<li>Once it's done loading, left click on Vesktop.</li>
<li>Sign into Discord like normal.</li>
<li>Once signed in, close out of Vesktop.</li>
<li>Double click on "Return to Gaming Mode" from the Desktop.</li>
<li>Once in Gaming Mode, press the Steam button and select Library.</li>
<li>Navigate to the Non-Steam section.</li>
<li>Find Vesktop, and hover over its Library page.</li>
<li>Press the Options key over Vesktop.</li>
<li>Navigate to "Properties" and select it.</li>
<li>Rename "Vesktop" to "Discord".</li>
<li>Back out of the Properties section.</li>
<li>Launch "Discord" from your Library.</li>
<li>Vesktop will prompt you to enable their Steam Deck configuration. Enable it.</li>
<li>Press the Steam button to open the "game's" Steam menu.</li>
<li>Exit out of the "game".</li>
</ol>
<div class="admonition warning">
<p class="admonition-title">Artwork</p>
<p>If you had installed the SteamGridDB Decky plugin, now is a good time to add artwork for your Non-Steam game!</p>
</div>
<p>Now, you can access Discord calls and content and participate directly from your Steam Deck. Additionally, in Gaming Mode, you can leave Discord running in the background while another game is running, meaning you can participate in voice chat while playing another game.</p>
<p><a href="../steam-deck/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="emudeck">EmuDeck</h2>
<div class="admonition info">
<p class="admonition-title">What Is EmuDeck?</p>
<p>Emulators are a big part of PC gaming. However, with how the Steam Deck's OS is divided into 2 parts it's hard to manage all the games you are emulating. EmuDeck entirely removes this problem from you. It works to simplify the process of setting up emulators for your Steam Deck as much as possible and adding your ROMs as Non-Steam games to your Library. As such, it's really only a one-time setup unless you add more ROMs to your collection.</p>
</div>
<h3 id="onboardinginitial-setup">Onboarding/Initial Setup</h3>
<ol>
<li>While in the Steam UI, press and hold down on the Power button until you see a menu appear.</li>
<li>Navigate to "Switch to Desktop" and select it. Go through any set up stuff that appears on screen about KDE Plasma (the name for the desktop environment) if you've never been in Desktop Mode.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">Wallet Information</p>
<p>If you unplug your Deck from the charger while in Desktop Mode, it may ask you to set up wallet information. No, it won't ask you for credit card information. Just click the option for the "classic file".</p>
</div>
<ol start="3">
<li>Click on the Firefox icon in the Dock. Go through the setup process. Firefox is the default browser on your Deck.</li>
<li>Go to <a class="external" href="https://emudeck.com/" rel="" target="_blank">https://emudeck.com/</a>.</li>
<li>Click the "Download button. It should take you to the section for your operating system. Click "SteamOS". A pop up will appear comparing the early access version to the free version. Click "Download for free".</li>
<li>In the file explorer, select the Desktop. Do NOT save yet!</li>
<li>Get rid of the <code>.download</code> extension in the file name bar. (<code>EmuDeck.desktop.download</code> should now become <code>EmuDeck.desktop</code>).</li>
<li>Once that's done, click "Save".</li>
<li>Close out of Firefox.</li>
<li>In the desktop, double click the "Install EmuDeck" icon. Press "Continue" or "Execute" after that if prompted.</li>
<li>Wait for it to finish doing a quick install of necessary background tools.</li>
<li>Once it's finished, it should open the proper setup page in the EmuDeck application. You should see 2 options, an "Easy Mode" or a "Custom Mode". Easy Mode alleviates all set up struggle but installs everything it can. Custom Mode allows for you to fine tune what you actually need. We will be selecting Custom Mode for our set up. Press "Next".</li>
<li>Select your appropriate ROM directory (in my case, my internal storage), and then select "Next". This is where all your ROMs and BIOS files will go for later. If you chose the internal storage, once everything is done you should see an <code>Emulation</code> folder in your Home folder in the file explorer. If you chose an SD card, that same <code>Emulation</code> folder will be on the root of your SD card. We will ignore the "Custom Directory" option.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">EmuDeck Error</p>
<p>You may see that EmuDeck may throw an error at you which tells you to restart EmuDeck. Just ignore this. Do not be worried. My Steam Deck does not have an SD card in it, and when I clicked the option to choose SD Card, the error popped up again. My guess is it is just panicking over not finding an SD card in your Deck.</p>
</div>
<ol start="14">
<li>Select your device. In our case, the Steam Deck. Press "Next".</li>
<li>Choose the option for "Highest" integration. This means that your ROMs will show up in your Steam Library once this whole process is done, so that you can launch them directly from Gaming Mode.</li>
<li>Select the emulators you'll need for your own tastes and then select "Next". Here's a rundown of every emulator you should see.<ul>
<li><strong>Azahar</strong>: A 3DS emulator. It is a merger of PabloMK7's old Citra fork and Lime3DS, both of which are now discontinued.</li>
<li><strong>BigPEmu</strong>: An Atari Jaguar emulator. I don't think this is pertinent to anyone in our server.</li>
<li><strong>Cemu</strong>: A Wii U emulator.</li>
<li><strong>Dolphin</strong>: A GameCube and Wii emulator.</li>
<li><strong>DuckStation</strong>: A PlayStation emulator.</li>
<li><strong>Flycast</strong>: A multiplatform Sega Dreamcast, Naomi, Naomi 2 and Atomiswave emulator. I don't think this is pertinent to anyone in our server.</li>
<li><strong>MAME</strong>: It stands for "Multiple Arcade Machine Emulator". I don't think this is pertinent to anyone in our server.</li>
<li><strong>melonDS</strong>: A DS emulator.</li>
<li><strong>mGBA</strong>: A GameBoy Advance emulator.</li>
<li><strong>Model2</strong>: A Sega Model 2 emulator. I don't think this is pertinent to anyone in our server.</li>
<li><strong>PCSX2</strong>: A PlayStation 2 emulator.</li>
<li><strong>PPSSPP</strong>: A PlayStation Portable emulator.</li>
<li><strong>PrimeHack</strong>: A mod for the Dolphin emulator which aims to tune the controls of <em>Metroid Prime Trilogy</em> into something more inline with a modern FPS game. This means bringing proper mouse and keyboard functionality and/or dual analogue stick functionality. I don't think this is pertinent to anyone in our server.</li>
<li><strong>RetroArch</strong>: A core based frontend for as many emulators as you can think of. Often times, these cores are not as updated as their standalone versions, (think <code>mGBA.exe</code> vs. its RetroArch counterpart), but it is very functional for all of its use cases. I'd only use this if you want to emulate a console that isn't on this list, or if you only want to use just one emulator for (mostly) everything.</li>
<li><strong>Rosalie's Mupen GUI</strong>: A GUI frontend for a Nintendo 64 emulator.</li>
<li><strong>RPCS3</strong>: A PlayStation 3 emulator.</li>
<li><strong>Ryujinx</strong>: A Nintendo Switch emulator.</li>
<li><strong>ScummVM</strong>: It stands for "Script Creation Utility for Maniac Mansion Virtual Machine". It is like a special translator that helps old video games run on modern computers. Many classic games from the late 80s and 90s were designed for older computers or consoles that don’t exist anymore. These games were often made using specific engines (like SCUMM, hence the name). ScummVM steps in by emulating those old environments. I don't think this is pertinent to anyone in our server.</li>
<li><strong>ShadPS4</strong>: A PlayStation 4 emulator.</li>
<li><strong>Supermodel</strong>: A Sega Model 3 emulator. I don't think this is pertinent to anyone in our server.</li>
<li><strong>Vita3k</strong>: A PlayStation Vita emulator.</li>
<li><strong>Xemu</strong>: An original Xbox emulator. Use case for this is very fringe, as most of the time you'll be able to run the same games on PCSX2, however, if any of you are into Halo this may be worth a look.</li>
<li><strong>Xenia</strong>: An Xbox 360 emulator. Use case for this is very fringe, as most of the time you'll be able to run the same games on PCSX2, however, if any of you are into Halo or one of the other few Xbox exclusives this may be worth a look.</li>
</ul>
</li>
</ol>
<div class="admonition note">
<p class="admonition-title">"What About Yuzu, Citron, and Eden?"</p>
<p>You may notice that I left out sections in this guide for Yuzu, Citron, and Eden. This is intentional on my behalf. For anyone familiar with the emulation scene, you may know that Yuzu was a Nintendo Switch emulator that Nintendo themselves had settled with the devs to take down from the internet. However, due to Yuzu's open source nature, this didn't stop other community members from forking the repository's codebase for their own and building on top of that as the original project was being shut down. Citron was one such Yuzu fork, while Eden is a fork of Citron due to some developers having a falling out with the other Citron devs. EmuDeck <em>only</em> provides <em>configurations</em> (ie, setting up controls and adding your games to your Steam library) for your <em>own</em> backups of Yuzu builds, meaning you'd need to scour the internet for a working backup of Yuzu before the project was shut down and place it in the <code>Applications</code> tab in your Dolphin file explorer. They will NOT provide support for it, meaning if you run into a problem using Yuzu they won't help you. This same BYO principle applies to Citron and Eden as well. Thus, I would recommend not bothering with them for the time being. You won't see further mention of them throughout the rest of this megathread.</p>
</div>
<ol start="17">
<li>Select your "Emulator and Tool Configurations" and press "Next". It should automatically select the emulators you had selected in the previous step. Additionally, it may select 2 options at the bottom of the list after scrolling: "EmulationStationDE" and "Pegasus". Deselect them, as we are working towards getting our ROMs to appear in our Steam library.</li>
<li>Configure Auto Saves if you'd like and press "Next". I normally leave this <strong>OFF</strong> but it is up to you. This feature creates save states every time you close out of a game in an applicable emulator so that when you reopen it later you pick up right where you left off.</li>
<li>Sign into your RetroAchievements account from here. If you don't have one, create one on their website and then come back to the EmuDeck set up process to sign into it from there. Press "Next" once finished.</li>
</ol>
<div class="admonition info">
<p class="admonition-title">About RetroAchievements</p>
<p>RetroAchievements is a nifty thing which allows you to earn community made achievements in your retro collection of emulated games. You will simply sign into your account through the settings of your emulator if it supports RetroAchievements, and you're good to go! Note that EmuDeck configures RetroAchievements for DuckStation, PCSX2, PPSSPP, and RetroArch.</p>
</div>
<div class="admonition warning">
<p class="admonition-title">Regarding RetroAchievements on RetroArch</p>
<p>This is just a thing with me, and may not be applicable to you, but RetroAchievements does not want to properly load up responses on my Steam Deck. This means I cannot use it on my Deck. If this happens to you once this whole process is finished...</p>
<ol>
<li>Open the RetroArch app from the start menu</li>
<li>Navigate to Settings -&gt; Achievements</li>
<li>Turn them off.</li>
<li>Back out to Main Menu. Navigate to Main Menu -&gt; Configuration File</li>
<li>"Save Current Configuration".</li>
<li>Back out and then navigate to Main Menu -&gt; Quit.</li>
</ol>
</div>
<ol start="19">
<li>Configure game bezel if you'd like and press "Next". I normally leave this <strong>ON</strong> but it is up to you. This feature adds borders that look like the console you're emulating if using an applicable emulator.</li>
<li>Configure Aspect Ratio for Classic Sega Systems if you'd like and press "Next". Not applicable to me, but I'd leave it as <strong>4:3</strong>.</li>
<li>Configure Aspect Ratio for Classic Nintendo if you'd like and press "Next". I leave this as <strong>4:3</strong>.</li>
<li>Configure Aspect Ratio for Classic 3D Games if you'd like and press "Next". I leave this as <strong>16:9</strong> usually <strong>but in some cases I revert back to 4:3</strong>.</li>
<li>Configure Aspect Ratio for GameCube Games if you'd like and press "Next". I leave this as <strong>16:9</strong>.</li>
<li>Configure LCD Shader for Handheld Systems if you'd like and press "Next". I leave this <strong>OFF</strong> but it is up to you.</li>
<li>Configure CRT Shader for Classic 2D Games if you'd like and press "Next". I leave this <strong>OFF</strong> but it is up to you.</li>
<li>Configure CRT Shader for Classic 3D Games if you'd like and press "Next". I leave this <strong>OFF</strong> but it is up to you.</li>
<li>Configure Controller Layout if you'd like and press "Next". I leave this as <strong>A=A</strong> or <strong>"Controller Layout Match"</strong> but it is up to you.</li>
<li>You'll see a final summary of what you're setting up on the screen. Read over it and if you're okay with it press "Finish". If not, press "Back" and reconfigure whatever you need to.</li>
<li>Wait for the installation to finish. It is installing your emulators and whatever other configurations you'll need. This will take a while, so grab a coffee or something. It may throw up a popup or 2, just accept them all.</li>
<li>Once this is done, it will throw on the success screen. Press "Next".</li>
<li>It will ask you to import games from here. Press "Manual Copy".</li>
<li>Press "Open Emulation Folder". It will open your file explorer in your installed and fully configured <code>Emulation</code> folder.</li>
<li>You'll see a <code>bios</code> folder and a <code>roms</code> folder. Both of which have folders inside of them which are very important. Here's a guide on how to get started with each of EmuDeck's emulators.<ul>
<li><strong>Azahar</strong><ul>
<li>Place your ROMs in <code>Emulation/roms/3ds</code> or <code>Emulation/roms/n3ds</code>.</li>
</ul>
</li>
<li><strong>BigPEmu</strong><ul>
<li>Place your Jaguar ROMs in <code>Emulation/roms/atarijaguar</code>.</li>
<li>Place your Jaguar CD ROMs in <code>Emulation/roms/atarijaguarcd</code>.</li>
</ul>
</li>
<li><strong>Cemu</strong><ul>
<li>Place your ROMs in <code>Emulation/roms/wiiu</code>.</li>
</ul>
</li>
<li><strong>Dolphin</strong><ul>
<li>Place your GameCube ROMs in <code>Emulation/roms/gc</code> or <code>Emulation/roms/gamecube</code>.</li>
<li>Place your Wii ROMs in <code>Emulation/roms/wii</code>.</li>
</ul>
</li>
<li><strong>DuckStation</strong><ul>
<li>Place your ROMs in <code>Emulation/roms/psx</code>.</li>
<li>Place your BIOS file(s) in <code>Emulation/bios</code>. BIOS is <strong>REQUIRED</strong>.</li>
</ul>
</li>
<li><strong>Flycast</strong><ul>
<li>Place your Dreamcast ROMs in <code>Emulation/roms/dreamcast</code>.</li>
<li>Place your Atomiswave ROMs in <code>Emulation/roms/atomiswave</code>.</li>
<li>Place your NAOMI ROMs in <code>Emulation/roms/naomi</code>.</li>
<li>Place your NAOMI 2 ROMS in <code>Emulation/roms/naomi2</code>.</li>
</ul>
</li>
<li><strong>MAME</strong><ul>
<li>Place your MAME ROMs in <code>Emulation/roms/mame</code>.</li>
<li>Place your MAME BIOS file(s) in <code>Emulation/roms/mame</code>. BIOS is <strong>REQUIRED</strong>.</li>
</ul>
</li>
<li><strong>melonDS</strong><ul>
<li>Place your ROMs in <code>Emulation/roms/ds</code>.</li>
</ul>
</li>
<li><strong>mGBA</strong><ul>
<li>Place your GBA ROMs in <code>Emulation/roms/gba</code>.</li>
<li>Place your GBC ROMs in <code>Emulation/roms/gbc</code>.</li>
<li>Place your GB ROMs in <code>Emulation/roms/gb</code>.</li>
</ul>
</li>
<li><strong>Model 2</strong><ul>
<li>Place your ROMs in <code>Emulation/roms/model2/roms</code>.</li>
</ul>
</li>
<li><strong>PCSX2</strong><ul>
<li>Place your ROMs in <code>Emulation/roms/ps2</code>.</li>
<li>Place your BIOS file(s) in <code>Emulation/bios</code>. BIOS is <strong>REQUIRED</strong>.</li>
</ul>
</li>
<li><strong>PPSSPP</strong><ul>
<li>Place your ROMs in <code>Emulation/roms/psp</code>.</li>
</ul>
</li>
<li><strong>Primehack</strong><ul>
<li>Place your ROM of <em>Metroid Prime Trilogy</em> in <code>Emulation/roms/primehacks/</code>.</li>
</ul>
</li>
<li><strong>RetroArch</strong><ul>
<li>Place your ROMs for various system in the folders listed in this little table. If your system of relevance is not listed in this table, I'd imagine the EmuDeck folder structure is pretty intuitive. (i.e. NES ROMs go in <code>Emulation/roms/nes</code>, SNES ROMs go in <code>Emulation/roms/snes</code>, etc.).</li>
</ul>
</li>
<li><strong>Rosalie's Mupen GUI</strong><ul>
<li>Place your N64 ROMs in <code>Emulation/roms/n64</code>.</li>
<li>Place your N64DD ROMs in <code>Emulation/roms/n64dd</code>.</li>
<li>Place your N64DD BIOS file(s) in <code>Emulation/bios</code>. BIOS is <strong>REQUIRED</strong> for N64DD.</li>
</ul>
</li>
<li><strong>RPCS3</strong><ul>
<li>Place your ROMs in <code>Emulation/roms/ps3</code>.</li>
<li>Install your <strong>(REQUIRED)</strong> BIOS directly through RPCS3 by...<ul>
<li>Opening the application from the Start menu.</li>
<li>Pressing on <code>File -\&gt; Install Firmware</code>.</li>
<li>Navigating to where your firmware file is downloaded and selecting it.</li>
<li>Closing out of RPCS3.</li>
</ul>
</li>
</ul>
</li>
<li><strong>Ryujinx</strong><ul>
<li>Place your ROMs in <code>Emulation/roms/switch</code>.</li>
<li>Place your <code>.keys</code> files in <code>Emulation/bios/ryujinx/keys</code>. Keys are <strong>REQUIRED</strong>.</li>
<li>Install your <strong>(REQUIRED)</strong>  BIOS directly through Ryujinx by...<ul>
<li>Opening the application from the Start menu.</li>
<li>Pressing on <code>Tools -\&gt; Install Firmware -\&gt; Install a firmware from XCI or ZIP</code>.</li>
<li>Navigating to where your firmware archive is downloaded and selecting it.</li>
<li>Closing out of Ryujinx.</li>
</ul>
</li>
</ul>
</li>
<li><strong>ScummVM</strong><ul>
<li>Place your ROMs in <code>Emulation/roms/scummvm</code>.</li>
</ul>
</li>
<li><strong>ShadPS4</strong><ul>
<li>Place your ROMs in <code>Emulation/roms/ps4</code>.</li>
</ul>
</li>
<li><strong>Supermodel</strong><ul>
<li>Place your ROMs in <code>Emulation/roms/model3</code>.</li>
</ul>
</li>
<li><strong>Vita3k</strong><ul>
<li>Place your ROMs in <code>Emulation/roms/psvita/InstalledGames</code>.</li>
<li>Install your <strong>(REQUIRED)</strong> BIOS directly through Vita3k by...<ul>
<li>Opening the application from the Start menu.</li>
<li>Pressing on <code>File -\&gt; Install Firmware</code>.</li>
<li>Navigating to where your firmware archive is downloaded and selecting it. This can be directly downloaded from Sony from <a class="external" href="https://www.playstation.com/en-us/support/hardware/psvita/system-software/" rel="" target="_blank">here</a>. Make sure once it's finished installing, select <code>Delete Archive?</code> if it shows up.</li>
<li>Navigating to where your system fonts file is downloaded and selecting it. This can be directly downloaded from Sony from <a class="external" href="http://dus01.psp2.update.playstation.net/update/psp2/image/2022_0209/sd_59dcf059d3328fb67be7e51f8aa33418/PSP2UPDAT.PUP?dest=us" rel="" target="_blank">here</a>. Make sure once it's finished installing, select <code>Delete Archive?</code> if it shows up.</li>
<li>Closing out of Vita3k.</li>
</ul>
</li>
</ul>
</li>
<li><strong>Xemu</strong><ul>
<li>Place your ROMs in <code>Emulation/roms/xbox</code>.</li>
<li>Place your BIOS files in <code>Emulation/bios</code>. BIOS is <strong>REQUIRED</strong>.<ul>
<li>Rename your MCPX Boot ROM Image to <code>mcpx_1.0.bin</code>.</li>
<li>Rename your Flash ROM Image to <code>Complex_4627v1.03.bin</code>.</li>
</ul>
</li>
</ul>
</li>
<li><strong>Xenia</strong><ul>
<li>Place your Xbox 360 ROMs in <code>Emulation/roms/xbox360/roms</code>.</li>
<li>Place your Xbox Live Arcade ROMs in <code>Emulation/roms/xbla/roms</code>.</li>
</ul>
</li>
</ul>
</li>
</ol>
<div class="admonition info">
<p class="admonition-title">Regarding ROMs And BIOS</p>
<p>In our lovely Discord server, I have made it so our fantastic bot can give you access to a library of ROMs and BIOS for various systems. For our case, whenever the bot is online please type "!w emulation" (without the quotes) in one of the command's permitted channels for a library of these files. Do note that it does not have everything listed here.</p>
</div>
<ol start="34">
<li>Once you've configured all your necessary files, close out of the file explorer.</li>
<li>Press "Close" and then "Next" on the EmuDeck application interface.</li>
<li>Click on "Launch Steam ROM Manager". Press "OK" on the prompt to enter Gecko Mode. Do note that if you are doing without a mouse and keyboard, you will no longer be able to use the right stick for controlling the mouse and must use R2 as left click.</li>
<li>Click on "Choose". Select your Steam profile and select "Save". Advance from there.</li>
<li>Turn off the toggle for all parsers.</li>
<li>Scroll through all the parsers and select which ones that are necessary for you.</li>
</ol>
<div class="admonition danger">
<p class="admonition-title">Regarding Cemu.</p>
<p>Do <strong><em>NOT</em></strong> use the Proton builds of Cemu! It is recommended to just use the Native versions. Additionally, if you are following our bot's emulation wiki (in our case, you should only be following steps 2-5 and then placing the ROM in the correct folder on your Deck listed above), please select your ROM format as <code>.wua</code>!</p>
</div>
<ol start="40">
<li>Once finished, click on "Add Games" and then "Parse".</li>
<li>If you'd like, configure the artwork as needed.</li>
<li>Once you have the artwork you want, press "Save to Steam". Wait for that to finish.</li>
<li>Close out of Steam ROM Manager. Press "Next" on the EmuDeck application interface.</li>
<li>Read over the Emulation Hotkeys, and then click on "Finish".</li>
<li>Click on "Manage Emulators".</li>
<li>Click on "Update Configurations". This will take a short bit. Just wait. Once it's done, click "Close".</li>
<li>Click on "Update" below "Update your Emulators".</li>
<li>Click on "Update Flatpaks". Then, click OK on the popup behind the Konsole window. Wait for the Flatpaks to update, and then press OK.</li>
<li>In the EmuDeck UI, click on "Update AppImages, Binaries, and Windows Executables". Then, click OK on the popup behind the Konsole window. Wait for everything to update, and then press OK.</li>
<li>In the EmuDeck UI, click on "Back".</li>
</ol>
<div class="admonition note">
<p class="admonition-title">If SRM Failed...</p>
<p>At this point, if Steam ROM Manager failed for you, you can follow steps 37-43 from here by simply clicking on the Steam ROM Manager button in the UI.</p>
</div>
<div class="admonition note">
<p class="admonition-title">If You'd Like...</p>
<p>At this point, if all you care about is retro gaming, you're done. Just close out of the EmuDeck application and return to Gaming Mode from the Desktop. Your ROMs should be populated in your Steam Library. However, the next few sections are dedicated to optional things that EmuDeck can do.</p>
</div>
<div class="admonition danger">
<p class="admonition-title">DO NOT!</p>
<p>Do <strong><em>NOT</em></strong> add the EmuDeck desktop app to Steam from the right click menu! I just never really got this to work, and the EmuDecky plugin should be more than enough to satisfy your needs for this app while in Gaming Mode. (More on this later).</p>
</div>
<h3 id="gyroscopedsu">GyroscopeDSU</h3>
<div class="admonition info">
<p class="admonition-title">What Is This?</p>
<p>GyroscopeDSU is a tool that allows you to use the Steam Deck's gyroscope features with Wii, 3DS, Wii U, and Switch games. If you plan on emulating these games, please follow these instructions!</p>
</div>
<ol>
<li>While still in the EmuDeck desktop application, scroll down the side menu until you see "Gyroscope". Click on it.</li>
<li>Click "Install".</li>
<li>A Konsole window should appear, installing it.</li>
<li>Once finished, press any key to exit the Konsole. Or just close out of it.</li>
<li>Click on the Start menu and select "Restart".</li>
<li>Confirm the selection. Once finished restarting, your Deck should now boot into Gaming Mode. </li>
</ol>
<div class="admonition note">
<p class="admonition-title">Why Restart?</p>
<p>You may have noticed that I said to restart the Deck instead of selecting the option in your Desktop to "Return to Gaming Mode". This is because clicking on that icon does <strong>NOT</strong> actually restart your Deck despite it looking like it does. We need to restart our Deck as GyroscopeDSU has now become core functionality of our Deck.</p>
</div>
<ol start="7">
<li>Assuming you've already added your games to your Steam library, select a game that may require gyro functionality.</li>
<li>Open the Controller Settings by selecting on the game pad icon.</li>
<li>Set the "Gyro Behavior" to "Directional Pad".</li>
<li>Calibrate the gyrometer by scrolling down to the "Gyro Calibration" section and selecting "Calibrate".</li>
<li>Place your Deck on a flat surface within 4 seconds of pressing the "Calibrate" button.</li>
<li>You should know if the Deck has finished calibrating the gyro if it says "Calibration Succeeded". Once it does, grab your Deck again and press the B button.</li>
<li>Press B again to exit back into the game's selection page.</li>
</ol>
<div class="admonition warning">
<p class="admonition-title">About Gyro Calibration</p>
<p>You will need to repeat steps 7-13 for <strong>EVERY</strong> game that may require gyro support in your Steam library!</p>
</div>
<h3 id="emudecky">EmuDecky</h3>
<div class="admonition info">
<p class="admonition-title">What Is EmuDecky?</p>
<p>EmuDecky is a Decky Loader plugin that...</p>
<ul>
<li>Lets you quickly see all the hotkeys configured by EmuDeck for your games. (i.e. For Wii U games, pressing L5 or R5 switches between the game screen and what would be the Gamepad's screen).</li>
<li>Lets you configure quick settings like bezels, shaders, etc.</li>
<li>Lets you configure aspect ratios for your games.</li>
<li>Lets you update your emulators from Gaming Mode.</li>
</ul>
<p>... with more features to come!</p>
</div>
<div class="admonition warning">
<p class="admonition-title">Please Do This!</p>
<p>If you haven't already, please follow my instructions on how to install Decky Loader and some or all of my recommended plugins!</p>
</div>
<ol>
<li>While still in the EmuDeck desktop application, scroll down the side menu until you see "EmuDecky". Click on it.</li>
<li>Click "Install EmuDecky".</li>
<li>You're done!</li>
</ol>
<h3 id="emudeck-compressor">EmuDeck Compressor</h3>
<div class="admonition info">
<p class="admonition-title">What Is This?</p>
<p>ROMs of games from later generations like PlayStation 3 or Nintendo Switch can be massive in size. Some ROMs can be as big as tens of gigabytes in size! This is where the EmuDeck Compression Tool comes in. At the cost of ever so slightly longer loading times in your games (in most cases so small it's almost unnoticeable), your ROM collection can be compressed to, in some cases, half its size!</p>
</div>
<ol>
<li>While still in the EmuDeck desktop application, scroll down the side menu until you see "EmuDeck Compressor". Click on it.</li>
<li>Read the information on screen about formats the compressor compresses to.</li>
<li>Scroll down until you see a button that says "Run the Compression Tool". Click on it.</li>
<li>A Konsole window and a little GUI (graphical user interface) should pop up on screen. Focus on the GUI.</li>
<li>Click on "Bulk Compression" and then click "Select".</li>
<li>It will now scan your <code>roms</code> folder and the folders inside of it for uncompressed ROMs. Check all the consoles that show up on screen and then click "Select".</li>
</ol>
<div class="admonition info">
<p class="admonition-title">Regarding PSP ROMs</p>
<p>If you are compressing PSP ROMs, it will prompt you to choose between a CSO or CHD format. CHD format compresses a bit more but only works in emulators, while CSO format works with real modded PSPs and real modded PSVitas at a slightly more bloated file size. Choose which format you'd like.</p>
</div>
<ol start="7">
<li>Once it finishes, close out of the tool. It should close the GUI and the Konsole window. You should now be back in the EmuDeck desktop app.</li>
</ol>
<h3 id="cloud-services">Cloud Services</h3>
<div class="admonition info">
<p class="admonition-title">What Do You Mean By This?</p>
<p>EmuDeck also allows you to, directly from Gaming Mode, access certain browser-based applications for watching movies/TV shows/YouTube, listening to music/podcasts, and browsing social media. That is, if you configure these services to work with EmuDeck.</p>
</div>
<ol>
<li>While still in the EmuDeck desktop application, scroll down the side menu until you see "Cloud Services". Click on it.</li>
<li>A popup will appear here with a few options. Click on the bubble next to the first option which says "Manage Cloud Services".</li>
</ol>
<div class="admonition note">
<p class="admonition-title">What About The Other Options?</p>
<p>There are a lot of other options here, but in this guide we will be ignoring them. These options are for remote play clients for PlayStation or streaming to/from another PC, or are other general applications. They aren't really pertinent to media to access directly from your Deck.</p>
</div>
<ol start="3">
<li>Click "Select".</li>
<li>Tick off whichever options are relevant to you for streaming services. In my case, I selected <code>Spotify.sh</code>, <code>Twitter.sh</code>, and  <code>YouTube.sh</code>.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">Discord?</p>
<p>There is an option for <code>Discord.sh</code> in this list. Ignore it. We already installed a better version of Discord earlier. :P</p>
</div>
<ol start="5">
<li>Once finished, click "OK".</li>
<li>It will then prompt you to use Steam ROM Manager for your changes to take effect. This is exactly what we'll be doing in the next subsection.</li>
</ol>
<h3 id="once-finished-with-rom-compression-andor-cloud-services">Once Finished With ROM Compression And/Or Cloud Services</h3>
<ol>
<li>Open Steam ROM Manager from the EmuDeck side menu. Remember that you'd have to use Gecko Mode if it's applicable to you.</li>
<li>Toggle off all parsers by clicking on and off the slider at the top right.</li>
<li>Select the parsers for the consoles that you had compressed earlier and/or the parser for "Cloud Services".</li>
</ol>
<div class="admonition danger">
<p class="admonition-title">Regarding Cemu.</p>
<p>Do <strong><em>NOT</em></strong> use the Proton builds of Cemu! It is recommended to just use the Native versions. Additionally, if you are following our bot's emulation wiki (in our case, you should only be following steps 2-5 and then placing the ROM in the correct folder on your Deck listed above), please select your ROM format as <code>.wua</code>!</p>
</div>
<ol start="4">
<li>Click on "Add Games" on the menu at the bottom.</li>
<li>Click "Parse".</li>
<li>Click "Remove from Steam". Now that the ROM(s) with the old format(s) are gone, this step is necessary to remove the link between the emulator(s) and the old ROM(s). Additionally, if you had previous cloud services installed doing this step will update the list to include the ones you chose.</li>
<li>Click "Parse" again.</li>
<li>Click "Add to Steam". Wait for it to finish.</li>
<li>Close out of Steam ROM Manager.</li>
<li>Close out of EmuDeck.</li>
<li>Return to Gaming Mode from the Desktop by double click on its icon.</li>
<li>Get back to emulating and consuming other content!</li>
</ol>
<p><a href="../steam-deck/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="unofficial-versions-of-proton">Unofficial Versions of Proton</h2>
<div class="admonition info">
<p class="admonition-title">Why Do I Need One?</p>
<p>As mentioned earlier, Proton is an open source tool created by Valve which allows for Linux to create Windows environments for your Windows Steam games to run underneath Linux. Because of its open source nature, other people have taken it upon themselves to create their own versions of Proton so that these new versions of Proton can do what Valve's doesn't. In fact, some games work underneath Linux exclusively with other versions of Proton as opposed to Valve's version. If you look through ProtonDB, a community driven forum of people listing their experience on how to configure a game to work under Proton, you may see that one of your own games on Steam runs only under custom versions of Proton.</p>
</div>
<p>Currently, there are two methods to get unofficial versions of Proton installed and configured on your Deck. I will be going over both methods.</p>
<h3 id="method-1-wine-cellar">Method 1 (Wine Cellar)</h3>
<div class="admonition info">
<p class="admonition-title">What Is Wine Cellar?</p>
<p>Wine Cellar is a Decky Loader plugin that streamline the process of installing custom versions of Proton. It is meant to be used within either Gaming Mode or Big Picture while using the Steam application in Desktop Mode.</p>
</div>
<div class="admonition warning">
<p class="admonition-title">Please Do This!</p>
<p>If you haven't already, please follow my instructions on how to install Decky Loader and some or all of my recommended plugins!</p>
</div>
<ol>
<li>While in the Gaming Mode UI, press the button to access the Quick Access Menu.</li>
<li>In the Decky plugin section, you should see a store icon at the top right. Navigate to it and select it.</li>
<li>Navigate to Wine Cellar and select "Install". This plugin should be at the bottom of the store, since it is sorted alphabetically.</li>
<li>Confirm the installation and wait for that installation to finish.</li>
<li>The Decky menu should open now. Navigate to the "Wine Cellar" tab and select it.</li>
<li>Navigate to "Manage" and select it.</li>
<li>Navigate to some 3rd-party compatibility tool, but in most cases you'll want to use "ProtonGE".<br/>
!!!  note About ProtonGE<br/>
    ProtonGE is a fork of Proton by a community member who goes by the name GloriousEggroll. He does a lot of unofficial Proton fixes with his versions that Valve probably won't do because of licensing agreements that he is not tied to.</li>
<li>Navigate to the latest version and select it. When selecting it, you could be selecting a button with 3 dots on it.</li>
<li>Select "Install" and wait for the download to finish.</li>
<li>Press and hold the Power button.</li>
<li>Navigate to "Restart" and select it.</li>
<li>Navigate to your game that only works under a custom version of Proton. Press the Options key once your cursor is over it.</li>
<li>Select "Properties".</li>
<li>Scroll down to the "Compatibility" section.</li>
<li>Check on the box that says "Force the use of a specific Steam Play compatibility tool". This should give you access to a new dropdown menu.</li>
<li>From the dropdown, select your custom version of Proton.</li>
<li>Press the B button twice.</li>
<li>Launch the game.</li>
<li>Happy gaming!</li>
</ol>
<h3 id="method-2-protonup-qt">Method 2 (ProtonUp-QT)</h3>
<div class="admonition info">
<p class="admonition-title">What Is ProtonUp-QT?</p>
<p>ProtonUp-QT is a simple GUI-based application to streamline the process of installing custom versions of Proton. It is meant to be used within Desktop Mode, as the process for using it requires the restart of Steam.</p>
</div>
<ol>
<li>While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.</li>
<li>Navigate to "Switch to Desktop" and select it. Go through any set up stuff that appears on screen about KDE Plasma (the name for the desktop environment) if you've never been in Desktop Mode.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">Wallet Information</p>
<p>If you unplug your Deck from the charger while in Desktop Mode, it may ask you to set up wallet information. No, it won't ask you for credit card information. Just click the option for the "classic file".</p>
</div>
<ol start="3">
<li>In the Dock, click on the Discover Store icon. It looks like a shopping bag.</li>
<li>Search for "ProtonUp-QT".</li>
<li>Install it. The icon for ProtonUp-QT looks like a green arrow in a white circle that says "PUPGUI" on it.</li>
<li>Exit out of the Discover Store.</li>
<li>Press on L5 on your Deck. This is the bottom most back button on the left side of your Deck. This will open up the Start Menu. Additionally, you can just tap on it from the Dock.</li>
<li>Go to the "Utilities" section of the Start Menu.</li>
<li>Navigate to ProtonUp-QT. Left click on it to open it.</li>
</ol>
<div class="admonition danger">
<p class="admonition-title">DO NOT!</p>
<p>Do <strong><em>NOT</em></strong> add this app to Steam from the right click menu! It is optimally used whenever Steam is closed and then reopened, and that happens when you go from Desktop Mode back to Gaming Mode.</p>
</div>
<ol start="10">
<li>Left click on "Add version".</li>
<li>Select a "Compatibility tool" from the dropdown. In most use cases this will be GE-Proton.</li>
<li>Select a "Version" (preferably the latest) from the dropdown.</li>
<li>Left click on "Install".</li>
<li>Once it's finished installing, close out of the application.</li>
<li>Double click on "Return to Gaming Mode" from the Desktop.</li>
<li>Navigate to your game that only works under a custom version of Proton. Press the Options key once your cursor is over it.</li>
<li>Select "Properties".</li>
<li>Scroll down to the "Compatibility" section.</li>
<li>Check on the box that says "Force the use of a specific Steam Play compatibility tool". This should give you access to a new dropdown menu.</li>
<li>From the dropdown, select your custom version of Proton.</li>
<li>Press the B button twice.</li>
<li>Launch the game.</li>
<li>Happy gaming!</li>
</ol>
<p><a href="../steam-deck/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="epicgogprime-games-on-deck">Epic/GOG/Prime Games On Deck</h2>
<h3 id="method-1-unifideck">Method 1 (Unifideck)</h3>
<div class="admonition info">
<p class="admonition-title">About Unifideck</p>
<p>Unifideck is a Decky Loader plugin which seamlessly integrates the games you have on Epic Games and all sorts of 3rd-party launchers with your Steam library in Gaming Mode. No need to go to Desktop Mode. It allows you to sign in to all the other extra storefronts and launchers from one single place and seamlessly integrate those games directly into the Steam Big Picture Mode experience.</p>
</div>
<div class="admonition warning">
<p class="admonition-title">Please Do This!</p>
<p>If you haven't already, please follow my instructions on how to install Decky Loader and some or all of my recommended plugins! Please be advised, however, that TabMaster configurations may conflict with this plugin. Please react accordingly!</p>
</div>
<div class="admonition warning">
<p class="admonition-title">Assumptions Made!</p>
<p><strong>This guide assumes you know how to install 3rd-party Decky plugins!</strong> You can find instructions on how to do this earlier in this repository in the section for my recommended Decky plugins.</p>
</div>
<div class="admonition warning">
<p class="admonition-title">AI Disclosure</p>
<p>This plugin does not have much documentation on how AI is used behind it. However, Claude and GitHub Copilot do show up as contributors to the project, with Claude having contributed a decent amount of code to the project. This doesn't mean the plugin itself is "vibe coded", though, since the majority of contributions to the plugin have come from humans within the Decky plugin dev community. The best way to describe the development of this plugin would be "AI assisted".</p>
</div>
<div class="admonition info">
<p><a class="external" href="https://github.com/mubaraknumann/unifideck/releases/latest" rel="" target="_blank">https://github.com/mubaraknumann/unifideck/releases/latest</a></p>
</div>
<ol>
<li>Once you've installed the plugin, access it via the Quick Access Menu. Navigate to the Decky section and select "Unifideck" from the list.</li>
<li>Once inside the plugin, you should see options to log in to several different storefronts that aren't Steam. Just tap on the login button for whichever storefront you're interested in.</li>
<li>Your Deck will prompt you do sign in like normal to that service. Do note that for Xbox services, you will need to have Microsoft Edge installed on your Deck. Don't worry, if you don't have it installed the plugin will prompt you through it.</li>
<li>Give it some time after sign in, but your 3rd-party games should appear in your Library as if they were regular Steam games now!</li>
</ol>
<h3 id="method-2-heroic-games-launcher">Method 2 (Heroic Games Launcher)</h3>
<div class="admonition info">
<p class="admonition-title">About Heroic Games Launcher</p>
<p>Heroic Games Launcher is an open source tool that allows you to quickly launch your games in your Epic Games, GOG, or Amazon Prime Gaming libraries. Their respective official clients do not officially support Linux, but Heroic does. Additionally, Heroic will automatically adjust Proton compatibility for your games, so you do not have to fiddle with it on your own. If you have any games on these platforms, this may worth a peek!</p>
</div>
<ol>
<li>While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.</li>
<li>Navigate to "Switch to Desktop" and select it. Go through any set up stuff that appears on screen about KDE Plasma (the name for the desktop environment) if you've never been in Desktop Mode.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">Wallet Information</p>
<p>If you unplug your Deck from the charger while in Desktop Mode, it may ask you to set up wallet information. No, it won't ask you for credit card information. Just click the option for the "classic file".</p>
</div>
<ol start="3">
<li>In the Dock, click on the Discover Store icon. It looks like a shopping bag.</li>
<li>Search for "Heroic Games Launcher".</li>
<li>Install it. The icon for the Heroic Games Launcher looks like a blue shield with a sword in the middle of it.</li>
<li>Exit out of the Discover Store.</li>
<li>Press on L5 on your Deck. This is the bottom most back button on the left side of your Deck. This will open up the Start Menu. Additionally, you can just tap on it from the Dock.</li>
<li>Go to the "Games" section of the Start Menu.</li>
<li>Navigate to the Heroic Games Launcher icon. Left click on it to open it.</li>
</ol>
<div class="admonition warning">
<p class="admonition-title">DO NOT?</p>
<p>Do <strong><em>NOT</em></strong> add this app to Steam from the right click menu! It is optimally used whenever Steam is closed and then reopened, and that happens when you go from Desktop Mode back to Gaming Mode.</p>
</div>
<ol start="10">
<li>Sign into whatever accounts you need to.</li>
<li>The "Library" section of Heroic will automatically populate with your games from each of the libraries you signed into.</li>
</ol>
<div class="admonition note">
<p class="admonition-title">Store Front</p>
<p>Heroic can also give you access to the store fronts you signed into. You may be able to buy games from Epic, GOG, or Amazon directly from Heroic through their "Stores" catalogue.</p>
</div>
<ol start="12">
<li>Install whatever games you want from the "Library" section.</li>
<li>Once done with that, close out of the Heroic Games Launcher by clicking on "Quit" in the bottom left and then confirming.</li>
<li>Double click on "Return to Gaming Mode" from the Desktop.</li>
<li>From the Non-Steam section of your Steam library, navigate to and select your game on Epic.</li>
<li>Select "Play" and wait for the game to launch.</li>
<li>A popup may appear asking you to set the Proton version to Experimental. Select "Yes".</li>
<li>Close out of your game like normal once finished.</li>
</ol>
<div class="admonition warning">
<p class="admonition-title">Artwork</p>
<p>If you had installed the SteamGridDB Decky plugin, now is a good time to add artwork for your Non-Steam game!</p>
</div>
<p><a href="../steam-deck/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="chiaki-ng-playstation-remote-play">chiaki-ng (PlayStation Remote Play)</h2>
<div class="admonition info">
<p class="admonition-title">What Is Chiaki?</p>
<p>Sony's official PlayStation Remote Play client is not available on Linux. Some developers took it upon themselves to make a free and open source alternative to Sony's official client called Chiaki which supports Linux. Another developer took it upon themself to make a fork of the original Chiaki project in order to optimize the Chiaki experience for the Steam Deck, leading to the birth of chiaki-ng (formerly known as chiaki4deck). In the end, you'll have a device which is akin to a PlayStation Portal but with much more functionality.</p>
</div>
<div class="admonition warning">
<p class="admonition-title">Assumptions Made!</p>
<ul>
<li><strong>This guide assumes you are using a PlayStation 5</strong>. The instructions shouldn't differ by much if you are using a PlayStation 4, but in terms of how to access certain settings on your PlayStation 4 it may differ. Regardless, in order for this to work you <strong>MUST</strong> have a PlayStation Network (PSN) account.</li>
<li><strong>This guide assumes that for setup, your Steam Deck and PlayStation are connected to the same network</strong>. After this is set up, it won't matter anymore but in order to initially get started your devices need to be on the same network.</li>
</ul>
</div>
<ol>
<li>While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.</li>
<li>Navigate to "Switch to Desktop" and select it.</li>
<li>In the Dock, click on the Discover Store icon. It looks like a shopping bag.</li>
<li>Search for "chiaki-ng".</li>
<li>Install it. The icon for chiaki-ng looks like a circle with Kirby eyes surrounded by spikes in a triangular manner. The top spike has Wi-Fi signals coming out of it.</li>
<li>Exit out of the Discover Store.</li>
<li>Press on L5 on your Deck. This is the bottom most back button on the left side of your Deck. This will open up the Start Menu. Additionally, you can just tap on it from the Dock.</li>
<li>Go to the "Games" section of the Start Menu.</li>
<li>Navigate to the icon for chiaki-ng. Right click on it.</li>
<li>Left click on "Add to Steam". This will be helpful for later, as now this program is in our Steam Library as a Non-Steam game.</li>
<li>Once it's done loading, left click on chiaki-ng.</li>
<li>Put your Deck aside for now, as we won't be needing it for a bit.</li>
<li>Turn on your PlayStation. Sign into your PSN profile.</li>
<li>Navigate to the Settings from the Home menu.</li>
<li>Navigate to the "System" option and select it.</li>
<li>Navigate to the "Power Saving" subsection. Select "Features Available in Rest Mode" from here.</li>
<li>Make sure that "Stay Connected to the Internet" and "Enable Turning On PS5 from Network" are enabled.</li>
<li>Back out until you go back to the list of "System" sub-options.</li>
<li>Navigate to the "Remote Play" subsection. Make sure "Enable Remote Play" is enabled.</li>
<li>Leave your PS5 on but put your controller aside. Pick up your Steam Deck again. It may have gone to sleep, so just lightly tap the Power button if so.</li>
<li>On Chiaki, you should be able to see your PS5 from the menu listed as "(unregistered)". If not, close out of chiaki-ng and reopen it from the Start menu. Click on your PS5 in Chiaki.</li>
<li>The "Host" text box should be filled with an IP address. We can safely ignore this for now.</li>
<li>Click on "PSN Login". It will redirect you to your web browser and ask you to sign into PSN. Please do so.</li>
<li>Once signed in, you should see a blank page that says "redirect" at the top left. Copy the webpage's URL.</li>
<li>Refocus on chiaki-ng. Click on "Click to Paste URL".</li>
<li>Click on "Get Account ID" on the top right.</li>
<li>Put aside your Steam Deck for now and pick up your PS5 controller. You should still be in the "Remote Play" subsection.</li>
<li>Select "Link Device". An 8 digit code should now appear on screen. You will also see a timer counting down from 300 seconds (5 minutes).</li>
<li>Put your PS5 controller down and pick up your Steam Deck again.</li>
<li>Use those 5 minutes to enter that code into the "Remote Play PIN" box in chiaki-ng.</li>
<li>Once you've done that, select "Register". You can turn off your PS5 after this.</li>
</ol>
<div class="admonition info">
<p class="admonition-title">Two PS5s?</p>
<p>You may notice 2 options for the same PS5 on chiaki-ng's interface. Note that the first option is to be selected when your Deck is on the same network as your PS5 and are streaming it from your house. The second option will say "Remote Connection via PSN" when away from your PS5's network.</p>
</div>
<ol start="32">
<li>Close out of chiaki-ng.</li>
<li>Close out of the browser.</li>
<li>Double click on "Return to Gaming Mode" from the Desktop.</li>
<li>Once in Gaming Mode, press the Steam button and select Library.</li>
<li>Navigate to the Non-Steam section.</li>
<li>Find chiaki-ng, and hover over its Library page.</li>
<li>Select chiaki-ng, but do NOT launch it.</li>
<li>Select the gear icon.</li>
<li>Navigate to "Properties" and select it.</li>
<li>Rename "chiaki-ng" to "Chiaki".</li>
<li>Back out of the Properties section.</li>
<li>Select the controller configuration button.</li>
<li>Find a community layout that works best for you.</li>
<li>Close out of that menu.</li>
<li>Close out back to your Library.</li>
</ol>
<div class="admonition warning">
<p class="admonition-title">Artwork</p>
<p>If you had installed the SteamGridDB Decky plugin, now is a good time to add artwork for your Non-Steam game!</p>
</div>
<ol start="47">
<li>Launch "Chiaki".</li>
<li>Select your PS5 using the appropriate on screen option and get to gaming! You would exit out of it like you would a normal Steam game in Gaming Mode. (By pressing the Steam button and then selecting "Exit game").</li>
</ol>
<p><a href="../steam-deck/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="kde-connect-wireless-file-transfer">KDE Connect (Wireless File Transfer)</h2>
<div class="admonition info">
<p class="admonition-title">What Is KDE Connect?</p>
<p>By default, an average Linux-based operating system does not have a desktop environment; normally it would only have a Terminal window and that's it. However, SteamOS comes bundled with the desktop environment called KDE Plasma from the KDE Community. Because the KDE Community is so generous, they will allow you to wirelessly transfer files to and from KDE environments and other devices using their KDE Connect application on both devices, so long as they are both connected to the same network.</p>
</div>
<div class="admonition warning">
<p class="admonition-title">Assumptions Made!</p>
<ul>
<li><strong>This guide assumes that for setup, your Steam Deck and your other device are connected to the same network</strong>. After this is set up, it won't matter anymore but in order to initially get started your devices need to be on the same network.</li>
<li><strong>This guide assumes your secondary device is another computer</strong>! Although it is possible to use KDE Connect with a cellular device, it is much simpler and intuitive to use it with a PC.</li>
</ul>
</div>
<ol>
<li>While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.</li>
<li>Navigate to "Switch to Desktop" and select it.</li>
<li>Press on L5 on your Deck. This is the bottom most back button on the left side of your Deck. This will open up the Start Menu. Additionally, you can just tap on it from the Dock.</li>
<li>Go to the "Internet" section of the Start Menu.</li>
<li>Navigate to KDE Connect and left click on it.</li>
</ol>
<div class="admonition danger">
<p class="admonition-title">DO NOT!</p>
<p>Do <strong><em>NOT</em></strong> add the KDE Connect app to Steam from the right click menu! This application is reliant on having access to your file explorer on Deck, which is only available on Desktop mode!</p>
</div>
<ol start="6">
<li>On another device, access this webpage.</li>
<li>On that other device, open <a class="external" href="https://kdeconnect.kde.org/download.html" rel="" target="_blank">this webpage</a>.</li>
<li>Download and install KDE Connect for whatever operating system your PC is using.</li>
<li>Open KDE Connect on your PC.</li>
<li>On either device, you should see the name of the other device. Assuming you are looking from your PC simply double click on "steamdeck" from the devices list in KDE Connect.</li>
<li>Your Deck will get a notification to pair it with the other device. Select "Pair" on the notification.</li>
<li>Minimize the KDE Connect windows on both devices and leave them running in the background. In your task bar you should see an icon that looks like a cell phone with a gear on its screen. This means that KDE Connect is running in the background.</li>
<li>On your PC or on your Steam Deck, all you have to do now is right click on a file and from the context menu select...<ul>
<li><strong>Windows</strong>: "Send to" &gt; "Send to remote device via KDE Connect"</li>
<li><strong>MacOS</strong>: "Send File via KDE Connect". It will then ask you which device to send to. Make sure "steamdeck" is selected and select "OK".</li>
<li><strong>SteamOS / A Linux Distro Using The KDE Plasma Desktop Environment</strong>: "Send to '(device name)' via KDE Connect"</li>
</ul>
</li>
<li>If your file is large, wait for it to fully transfer over. Your Steam Deck will have a notification with a progress bar telling you how long to wait.</li>
<li>On your target device, your file will appear in the Downloads directory in your file explorer.</li>
</ol>
<p><a href="../steam-deck/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="using-cheats-in-pc-games">Using Cheats In PC Games</h2>
<div class="admonition info">
<p class="admonition-title">How?</p>
<p>Have you wanted to ever use a cheat code on your games on Steam? Well, not only can you on Windows but also on Deck too! There is a nice community of people who make things called "trainers", which feature toggle on and off switches for cheats you can use on your PC games. We will be making use of such trainers with a nifty Decky Loader plugin called CheatDeck.</p>
</div>
<div class="admonition warning">
<p class="admonition-title">Please Do This!</p>
<p>If you haven't already, please follow my instructions on how to install Decky Loader and some or all of my recommended plugins!</p>
</div>
<div class="admonition note">
<p class="admonition-title">For The Sake Of The Guide</p>
<p>For this guide, I will walk you through how I got a working trainer for <em>Kingdom Hearts: Final Mix</em> running on my Steam Deck. The process for doing this for other games should not differ by much, however.</p>
</div>
<ol>
<li>While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.</li>
<li>Navigate to "Switch to Desktop" and select it.</li>
<li>In your Deck's web browser, open this webpage.</li>
<li>While looking through this very guide on your Deck, open <a class="external" href="https://flingtrainer.com/" rel="" target="_blank">this webpage</a>.</li>
<li>In the website's search bar, search for "Kingdom Hearts Final Mix". Remember that pressing the Steam + X buttons as a combo will bring up an onscreen keyboard.</li>
<li>Navigate to the result for this game and click on it.</li>
<li>Click on the download link for the standalone version that has the biggest file size. Download the <code>.zip</code> file to a location of your choice</li>
<li>Extract the <code>.zip</code> file you just downloaded from FLiNG Trainer. A <code>.exe</code> file for your trainer should have been extracted. Once that's done, you may delete the <code>.zip</code> file if you wish.</li>
<li>Close out of Firefox and Dolphin. You should now be at the Desktop.</li>
<li>Double click on "Return to Gaming Mode".</li>
<li>Press the button to access the Quick Access Menu.</li>
<li>In the Decky plugin section, you should see a store icon at the top right. Navigate to it and select it.</li>
<li>Navigate to CheatDeck and select "Install". This plugin should be near the top of the store listings, since it is sorted alphabetically.</li>
<li>Wait for it to finish, then back out as much as you can.</li>
<li>Press the Steam button.</li>
<li>Navigate to "Settings" and select it.</li>
<li>In the "System" category, make sure the toggle for "Enable Developer Mode" is switched on. Don't worry, you won't be developing anything.</li>
<li>Back out as much as you can.</li>
<li>Navigate to your copy of <em>KINGDOM HEARTS -HD 1.5+2.5 REMIX-</em> and make your cursor hover over it.</li>
<li>Press the Menu button once. If an option for "CheatDeck" doesn't show up, back out and then press the Menu button again.</li>
<li>Navigate to "CheatDeck" and select it.</li>
<li>In the "Normal" category, make sure "Enable Cheat" is toggled on. This should open a dialogue box that says "Cheat path".</li>
<li>Select the folder icon next to that dialogue box.</li>
<li>Navigate to wherever you saved the <code>.exe</code> file for your trainer and select that <code>.exe</code> file.</li>
<li>Navigate to "Save Settings" and select it. A notification should pop up at the bottom saying that your normal settings were saved.</li>
<li>Press B twice.</li>
<li>Select <em>KINGDOM HEARTS -HD 1.5+2.5 REMIX-</em>, and then select "Play".</li>
<li>You should see that the trainer launched on top of your game. Simply press the Steam button, navigate to the "Switch Windows" submenu in the category for this Kingdom Hearts collection, and select the correct window for your game.</li>
<li>In the launcher for the collection, press X to open the configuration settings.</li>
<li>For some reason, this trainer only works on the Deck when the game is configured as "Windowed". Make sure you change that in the resolution settings. Since you launched the game in Gaming Mode, the resolution will not be visibly impacted. The need to make the game windowed should not be a thing for most other games.</li>
<li>Back out of that menu, and launch <em>Kingdom Hearts: Final Mix</em>.</li>
<li>Press the Steam button, and like you did to get to the game, switch back to the window for your trainer.</li>
<li>Enable/Disable whatever cheats you'd like to use.</li>
<li>Switch back to the game's main window.</li>
<li>You can now play your game with cheats!</li>
</ol>
<p><a href="../steam-deck/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="protontricks">Protontricks</h2>
<div class="admonition info">
<p class="admonition-title">Why Do I Need This?</p>
<p>Let’s say you’re trying to run a game on your Deck via Proton, but something just isn’t working right. Maybe the game needs a certain .NET or Visual C++ runtime, or maybe you’re trying to get a launcher like <a class="external" href="http://battle.net/" rel="" target="_blank">Battle.net</a> or Rockstar to actually load past its splash screen. Protontricks is a must-have tool that lets you install extra Windows components and tweak Wine/Proton prefixes (the fake C:\ drives every game you play under Proton creates specifically for that game) directly.</p>
</div>
<div class="admonition warning">
<p class="admonition-title">Please Do This!</p>
<p>Make sure that you've ran the game you're trying to edit a prefix of at least once! This way, the Deck will have configured the prefix for you, and will be available for modifying in the first place! Just having the game installed is not enough!</p>
</div>
<ol>
<li>While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.</li>
<li>Navigate to "Switch to Desktop" and select it.</li>
<li>In the Dock, click on the Discover Store icon. It looks like a shopping bag.</li>
<li>Search for "Protontricks".</li>
<li>Install it. The icon for Protontricks looks like a full wine glass.</li>
<li>Exit out of the Discover Store.</li>
<li>Press on L5 on your Deck. This is the bottom most back button on the left side of your Deck. This will open up the Start Menu. Additionally, you can just tap on it from the Dock.</li>
<li>Go to the "All Applications" section of the Start Menu.</li>
<li>Navigate to the icon for chiaki-ng. Left click on it.</li>
<li>Protontricks will scan your Steam library for installed prefixes. Scroll to and select the game you want to configure. Click OK. Wait a few short seconds afterward.</li>
<li>Click on OK to "Select the default wineprefix".</li>
<li>A menu will appear. If you want to install specific Windows components (like <code>dotnet48</code>, <code>vcrun2015</code>, etc.), click on the box for "Install a Windows DLL or component".</li>
</ol>
<div class="admonition note">
<p class="admonition-title">For Power Users</p>
<p>Protontricks can also run custom commands inside a game's Proton prefix, change Wine settings, or even open a file explorer directly inside a prefix to mess with files manually.</p>
</div>
<ol start="13">
<li>Click on OK.</li>
<li>Navigate through the list that pops up. Click on a package (or packages) you would like to install. Then, click OK.</li>
</ol>
<div class="admonition info">
<p class="admonition-title">SHA-256 Checksums</p>
<p>You may get warnings that Protontricks didn't get the proper SHA-256 checksums for the installers it grabs. This is totally fine. All a SHA-256 checksum is is a digital fingerprint for your files. Functionally, a finger, regardless of whose it is, does the same things as another person's finger, it's just that each finger has a unique fingerprint identifying who a finger belongs to. A SHA-256 checksum aims to accomplish this for digital files.</p>
</div>
<ol start="15">
<li>Follow the instructions of the installers that pop up. The app will handle downloading and configuring them in the correct Proton prefix.</li>
<li>Once the installer(s) have finished, click on Cancel 3 times to close out of Protontricks.</li>
<li>Double click on Return to Gaming Mode from your desktop to go back.</li>
<li>Launch your game through Steam. It should now run with the components you installed!</li>
</ol>
<p><a href="../steam-deck/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="vortex-mod-manager">Vortex Mod Manager</h2>
<div class="admonition info">
<p class="admonition-title">What Is Vortex?</p>
<p>Vortex is a mod manager made by the people over at Nexus Mods. It is meant to integrate with games that have mods on <a class="external" href="http://nexusmods.com/" rel="" target="_blank">nexusmods.com</a> with your installed libraries. Unfortunately, Vortex is a Windows only application (for now). If you've been following this guide thus far, you might think "Oh, just add it as a Non-Steam game and force it to run under Proton", but this wouldn't work as Proton creates fake C:\ drives for every "game" you play. This means that in a hypothetical Vortex "game", you wouldn't have access to your Steam game installation library as it just doesn't exist in the fake C:\ drive that Vortex would create. However, this doesn't stop community modders for doing things to counteract this and automate letting you use Vortex on your Steam Deck!</p>
</div>
<ol>
<li>While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.</li>
<li>Navigate to "Switch to Desktop" and select it.</li>
<li>Open Firefox. It should be in your task bar.</li>
<li>Open this megathread on your Deck and navigate to this part of the megathread.</li>
<li>Right click <a class="external" href="https://raw.githubusercontent.com/pikdum/steam-deck/master/install.desktop" rel="" target="_blank">this link</a>. Click "Save Link as...".</li>
<li>In the file explorer, select the Desktop. Do NOT save yet!</li>
<li>Get rid of the <code>.download</code> extension in the file name bar. (<code>install.desktop.download</code> should now become <code>install.desktop</code>).</li>
<li>Once that's done, click "Save".</li>
<li>Close out of Firefox.</li>
<li>In the desktop, double click the "Install Pikdum's Tools" icon. Press "Continue" or "Execute" after that if prompted.</li>
<li>Wait for it to finish doing a quick install of necessary background tools.</li>
<li>Once it's finished, the Konsole window will close and you'll be back in the Desktop. Double click on the "Install Vortex" icon. Be patient, as a Konsole window will appear and take a bit to install the following:<ul>
<li>Vortex</li>
<li>A Steam Linux Runtime</li>
<li>A version of GE-Proton</li>
<li>A prefix for Vortex with links in it to your Steam games installed on your internal drive (J:) and/or your microSD card (K:)</li>
<li>Any necessary Visual C++ runtimes or the like.</li>
<li>A bunch of files on your Desktop for certain games that you are to use after deploying mods for them.</li>
</ul>
</li>
<li>Once that install is finished, the Konsole window will automatically close itself. You can now double click the icon on your Desktop to open Vortex. Once it's open, you may get a notification telling you that "Extensions are updated. Restart now." Please click on that restart button in that notification.</li>
<li>Sign into NexusMods if you don't already have an account with them. This can be done by clicking on the red icon that outlines a person. It will open up Firefox automatically and sign you into NexusMods. You can also create an account here if you haven't already. which is a <strong><em>required</em></strong> step since installing mods from NexusMods requires an account. Don't worry, it's free.</li>
<li>Click on the Games tab on the left.</li>
<li>Search for your game of choice and click on it. Vortex may tell you that support for that game is provided through an extension and ask you to download such an extension, to which click on the "Download" button at the bottom right of that window. Vortex will restart afterwards.</li>
<li>You may get a warning that Vortex couldn't find your game and that you'd need to manually locate it. A file explorer will appear, but it won't look like the Dolphin file explorer you're probably used to by now, rather something that looks more like old school Windows. This is just what the software acts on, as, remember, you are running these Windows applications under a virtual environment.</li>
<li>Double click on "My Computer".</li>
<li>Double click on "(J:)".</li>
<li>Click on the folder for your game.</li>
<li>Click on "Open" at the bottom right. You may get a warning asking which platform the game is installed through. Select "Steam" (if applicable, which it most likely is) and then select OK. You may also get a warning saying that your mods have been purged. Just click OK at the bottom.</li>
<li>Click on the Settings tab on the left.</li>
<li>Click on the "Mods" subsection on the top.</li>
<li>Click on the "Suggest" button to automatically map your mods to the correct spot.</li>
<li>Click on the "Apply" button next to the "Suggest" button.</li>
<li>In the "Deployment Method" dropdown below it, change it from "Symlink Deployment" to "Hardlink Deployment".</li>
<li>Click on the "Apply" button next to that dropdown.</li>
<li>Click on the "Mods" tab for the game of your choice on the left.</li>
<li>Minimize Vortex.</li>
<li>Open Firefox.</li>
<li>Go to <a class="external" href="https://nexusmods.com/" rel="" target="_blank">https://nexusmods.com</a>.</li>
<li>Search for the mods you want with your game.</li>
<li>On the mod's page on NexusMods, there should be a "Vortex" button at the top right for downloading through there. Click on that.</li>
<li>Click on "Slow Download".</li>
<li>Your mod will now install through Vortex, and you'll see once you unminimize Vortex. Please unminimize Vortex as you may never know if there are any pop ups that may arise about mod installations in Vortex which you'd need to attend to.</li>
<li>Repeat steps 29 and 32-35 as needed for however many mods you need.</li>
<li>Once you've installed all of your mods, click on one of those mods in the list. Make sure to click somewhere near the middle of its row, as to not interfere with other UI elements.</li>
<li>Press Ctrl + A on your keyboard.</li>
<li>Click on "Deploy Mods" on the bar on top.</li>
<li>You're done with Vortex. Close out of it. You may need to use one of Pikdum's post-deploy scripts. Make sure to double click on that. This will rename certain <code>.exe</code> files within your game installation such that when pressing Play on Steam the game will boot directly instead of through the launcher. Note that you'll only need to do this once after deploying mods for the first time. Games that Pikdum delivers these post-deploy scripts are as follows:<ul>
<li>Fallout 3</li>
<li>Fallout 4</li>
<li>Fallout New Vegas. There is also a <em>pre</em>-deploy for this game as well. This is self-explanatory.</li>
<li>Oblivion</li>
<li>Skyrim Legendary Edition</li>
<li>Skyrim Special Edition</li>
</ul>
</li>
<li>Double click the "Return to Gaming Mode" icon.</li>
<li>Navigate to the game you modded in your Library, and select it.</li>
<li>Press Play. Enjoy your mods!</li>
</ol>
<div class="admonition warning">
<p class="admonition-title">Mods Not Working?</p>
<p>Sometimes just installing mods isn’t enough; they might need extra setup. Some games need special launch options in Steam or certain <code>.dll</code> files added with Protontricks. A quick search on Google, the game’s forums, or ProtonDB can point you in the right direction. For example, to get mods working in <em>FF XII</em>, I had to install <code>vcrun2022</code> using Protontricks and use this launch command: <code>WINEDLLOVERRIDES="dinput8=n,b" %command%</code>. It’s different for every game, so just <strong>keep an eye out</strong>!</p>
</div>
<p><a href="../steam-deck/">Back to Top</a><br/>
<a href="../">Back to Base</a></p>
<h2 id="achievement-manager">Achievement Manager</h2>
<p>Fun Fact: Just as easy as a game on Steam can give you achievements, it can also take them away from you! That’s because achievements are handled through the Steamworks API, which developers implement into their games. Think of an API like a vending machine for computers: a program presses a button or 2 (makes a request) on the machine (a database or server) after paying (authenticating with the database/server), and out goes a soda (a response gets sent to the program from the database/server). Similarly, a game accesses the Steamworks API to give you achievements. Very rarely will a game ever take them away from you, as there's usually no reason to if you're progressing through a game normally, but it can very much happen in some cases.</p>
<p>But what if you could manipulate how many achievements you do or don't have for a game in your library? Let's say you were emulating an old game, but then later bought that same game on Steam. Of course, you could play through the game again the natural way through Steam this time, but that would take way more time than just (in some cases) converting and importing your existing save to Steam Cloud. And even after importing your save file, you'll notice that you don't have any achievements for your hard work registered in Steam. This is where a tool called Steam Achievement Manager comes in: originally a Windows based tool that lets you edit what achievements you do or don't have in any game in your library. The Linux community has done a great job at making a version of SAM for Linux, while I took it upon myself to streamline that process of getting that port to your Deck!</p>
<div class="admonition warning">
<p class="admonition-title">Use At Your Own Risk!</p>
<p>As far as I could find, there haven’t been any reports of people getting banned for using SAM or SAMRewritten. That said, <strong>it's still smart to treat it as "use at your own risk"</strong> This is super common with homebrew tools across all platforms, and not just Steam, however people online like to fearmonger about this tool in particular. Honestly, if you’re careful and don’t do anything wild, you’ll be just fine.</p>
</div>
<ol>
<li>While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.</li>
<li>Navigate to "Switch to Desktop" and select it.</li>
<li>Open Firefox. It should be in your task bar.</li>
<li>Open this megathread on your Deck and navigate to this part of the megathread.</li>
<li>Go to <a class="external" href="https://github.com/PaulCombal/SamRewritten/releases/latest" rel="" target="_blank">this website</a>.</li>
<li>Download the latest <code>.AppImage</code> that has the <code>-gtk</code> suffix to its filename. Save it to a convenient location. (I choose the Applications folder inside the Home section of the file explorer).</li>
<li>Double click on SAMRewritten.</li>
<li>You will see a partial list of all your games. Not every game is listed. If the game you're looking for is listed, simply click on it. If not, find it's app ID (the quickest way to do this is to open the game's launch page on Steam, click on "Store Page", and find it in the URL of the game's store page), enter it into the search bar, and click "launch appID (app ID)".</li>
<li>Click on the lock icon(s) next to the achievement(s) you want to (en/dis)able.</li>
<li>Click on the save icon near the top right of the window.</li>
<li>Click on the left arrow near the top left of the window.</li>
<li>Close out of SAMRewritten.</li>
<li>Double click on Return to Gaming Mode.</li>
<li>Open up the game's launch page. You should now see your achievements listed (or lack thereof)!</li>
</ol>
<p><a href="../steam-deck/">Back to Top</a><br/>
<a href="../">Back to Base</a></p></div>
</article>