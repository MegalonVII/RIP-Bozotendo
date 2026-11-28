# RIP Bozotendo, Steam Deck

!!! warning "Important Warning"

    Until I say it isn't, **this megathread will continually be in a state of WIP**! I am continually working to add things to here that may be pertinent to us. If you want information on something, please let me know. I will try my best to update this thread as needed or as I come along certain information.

## Disclaimers

- The Steam Deck runs a "distro" of Linux called SteamOS. I know that to a new person, Linux seems scary. But SteamOS is very beginner friendly to work with. You'll have a hang of it just by following this guide (which is meant to be read sequentially).
    - This comes at a downside where some games that require the use of an anti-cheat, such as Valorant, will **NOT** work on the Steam Deck. While the developers of these games can simply just "flip a switch" to allow Linux gamers to play these games, they do not allow it for the time being. If you wanted to play these games on your Deck, I'm so sorry. Don't fret, however, since there is [this website](https://areweanticheatyet.com/) that tells you whether an anti-cheat game will work on Linux!
- **The Steam Deck's Desktop Mode is your friend!** We will be using it frequently to install tools needed to maximize your Steam Deck's potential.
- The Steam Deck doesn't have a "proper" process for hacking one like, say, a Wii or 3DS has, where it has a sort of indescribable hacker-man feel to it. But, you can do some pretty cool stuff outside of what Valve normally would let you do with a Steam Deck.
    - Just know that since we will be doing things in Desktop Mode, while everything is doable without a mouse and keyboard it is recommended that you use one for navigating it. This can be done by docking your Steam Deck into a dock, or by using Steam Link to stream your Steam Deck's display to your PC.
        - Should you choose not to utilize a mouse and keyboard, the Steam deck gives you functionality within the device's hardware. The way clicking works is kind of counterintuitive but in your hands it will make sense.
            1. Left click is by either pressing down on the right track pad or by pressing R2.
            2. Right click is by pressing L2.
            3. Your mouse is controlled by either the right track pad or the right joystick. Alternatively, you can try using the touchscreen to interact with things on screen.
            4. The scroll wheel is controlled by the left track pad and the left joystick.
            5. To invoke the on-screen keyboard, press Steam + X on your Deck.
- Fun fact: In Desktop Mode, if you right click on an application's icon in either Dolphin (the file explorer) or in the start menu, you can add that application to Steam as a Non-Steam game. This will allow you to access that application back in Gaming Mode. A good use case for this may be for adding applications like Discord (Vesktop, as the more commonly utilized Discord client for Deck users is called. More on this later.) or Firefox to Steam so that you can quickly navigate to them from Gaming Mode instead of having to manually go to Desktop Mode every time.
- You may see reference to something called "Proton" in this part of the megathread. Proton is an open source tool created by Valve which allows for Linux to create Windows environments for your Windows Steam games to run underneath Linux. Because of its open source nature, other people have taken it upon themselves to create their own versions of Proton so that these new versions of Proton can do what Valve's doesn't. More on this later.
    - Speaking of Proton, the way it works is that the Steam Deck will create fake Windows `C:\` drives for your each of your individual games to work in, which can take up anywhere between 255 MB to ~1.5 GB of storage. Additionally, games will also install compiling their own individual shader caches, which can take up more storage in a range of between a few kilobytes to upwards of 15 GIGABYTES. In lieu of this, **I would advise against buying a 64 GB Steam Deck unless you plan on upgrading the SSD**! Additionally, to play it safe I'd always caution **not to fill up the storage on your Steam Deck and always leave around 10-15 GB free AT ALL TIMES**!
        - If you'd like to learn how to upgrade the SSD on your Steam Deck I will not be going over it on this Rentry, but you can [watch this YouTube video](https://youtu.be/YF2Dy7Ol_Ew). If you're going this route I'd recommend getting **at least a 1 TB SSD** to go with your Deck, but **no more than 2 TB**!

## Recommended Settings Tweaks

Here's some settings you should tweak on your Deck to make it more seamless and console-like!

1. While in the Steam UI, press the Steam button.
2. Navigate to "Settings" and select it.
3. Navigate to "Display".
4. In the Display settings, navigate to "Automatically Scale User Interface" and make sure it is toggled on. This scales the UI to your TV when docked.
5. If you'd like to reduce blue light emission when playing at night, navigate to "Schedule Night Mode" and make sure it is toggled on. Use the drop downs below to schedule times in which Night Mode is active.
6. Navigate to Maximum Game Resolution. In the drop down, set the resolution to "Native". This auto-adjusts game resolution when docked.
7. Press B.
8. Navigate to "Power" and select it. You should have your cursor over "Battery Percentage". Make sure it is toggled on.
9. Right below that toggle, make sure "Enable battery charging limit" is toggled on. This can be helpful if you're frequently docking your Steam Deck to an external display or if you play a lot while the Deck is charging as to not degrade the battery's health over time. Use the slider below to set the charge limit; I recommend 80%. *Note: it may take some getting used to seeing that 80% as "fully charged".*
10. Navigate to "When plugged in, dim after" and select 20 minutes from the drop down.
11. Navigate to "On battery power, dim after" and select 5 minutes from the drop down.
12. Navigate to "When plugged in, sleep after" and select "Disabled" from the drop down.
13. Navigate to "On battery power, sleep after" and select 20 minutes from the drop down.
14. Press B.
15. Navigate to "Downloads" and select it.
16. Navigate to "Limit download speed" and make sure it is toggled on.
17. In the box below, set the limit to `10000000` Kbps. This gets rid of Steam's internal bandwidth cap for game downloads!
18. Navigate to "Allow downloads during gameplay" and make sure it is toggled on. *Note: for more intensive games, having downloads going in the background while playing may hinder performance.*
19. Press B.
20. Navigate to "Game Recording" and select it.
21. From the three choices below, choose "Record Manually". Now, you can press Steam + A to start/stop recordings in game. If you'd like you can navigate further down to "Record Microphone" and toggle that on in case you want to record your voice as well.
22. Press B twice.

## Decky Loader

!!! info "About Decky Loader"

    Decky Loader is a plugin loader directly for your Steam Deck when it is in Gaming Mode. It can do a whole range of things, such as giving you a range of tools to fine tune how the hardware works or changing how Gaming Mode looks like to you. Highly customizable with a very simply set up process.

1. While in the Steam UI, press and hold down on the Power button until you see a menu appear.
2. Navigate to "Switch to Desktop" and select it. Go through any set up stuff that appears on screen about KDE Plasma (the name for the desktop environment) if you've never been in Desktop Mode.

!!! note "Wallet Information"

    If you unplug your Deck from the charger while in Desktop Mode, it may ask you to set up wallet information. No, it won't ask you for credit card information. Just click the option for the "classic file".

3. Click on the Firefox icon in the Dock. Go through the setup process. Firefox is the default browser on your Deck.
4. Go to <https://decky.xyz/>.
5. Right click the "Download" button at the top right of the page and left click "Save Link As...".
6. In the file explorer, select the Desktop. Do NOT save yet!
7. Get rid of the `.download` extension in the file name bar. (`decky_installer.desktop.download` should now become `decky_installer.desktop`).
8. Once that's done, click "Save".
9. Close out of Firefox.
10. In the desktop, double click the "Install Decky" icon. Press "Continue" or "Execute" after that if prompted.
11. It may ask you to temporarily set your sudo password to "Decky!". Your "sudo" password is the password running tasks in what is the equivalent of running as administrator on Windows. (**S**uper **U**ser **DO**). Let it.
12. Ask it to install the "release" version. You won't need the "prerelease" version unless you know what you're doing.
13. Once it's finished installing, close out of the Konsole window the script was running in.
14. Double click on "Return to Gaming Mode" in the desktop.
15. In Gaming Mode, press the 3dots button ("Quick Access Menu", as it'll be called here after). You should see an icon that looks like a wall plug. Navigate to it.

!!! note "Decky Icon Not Showing?"

    If you don't see that wall plug icon, give it a bit. And if still not, press and hold the power button and restart the device.

16. You should see a store icon at the top right. Navigate to it and select it.
17. Install whatever plugins you'd like from their store.

### Recommended Decky Plugins (Store)

#### ProtonDB Badges

Sometimes, whatever Valve says is Deck "Verified" or Deck "Playable" or Deck "Unsupported" is incorrect. Adding this badge to the game's Gaming Mode start page allows you to click navigate and select it to gain Linux gaming community insight on how to properly configure the game of your choice to work with your Linux device.

It has been helpful to me at least where a game in my Library is marked as Deck "Unsupported" by Valve. However, ProtonDB was able to tell me to get a custom version of Proton to get this game working with my Deck. (More on custom versions of Proton later).

#### PowerTools

If you know what you are doing, you can directly monitor CPU and GPU usage through this plugin to optimize performance in certain situations.

#### SteamGridDB

This tool is for adding artwork for whatever game/program you have listed on Steam, be they official or unofficial.

1. Hover a title in your Library or Home and press the Options button (looks like 3 lines on top of each other next to Y).
2. Select "Change Artwork". If it doesn't appear, press B and then press Options while hovering over the title again.
3. Choose whatever artwork you'd like.
4. Restart after you're done as prompted.

#### CSS Loader

This one is probably the most intricate plugin on its own. It allows you to completely customize the look of your Gaming Mode UI. It has its own plugins to extend to this plugin.

1. In the Decky plugin menu from the Quick Access Menu, navigate to "CSS Loader" and select it.
2. Navigate to the Download icon at the top right and select it.
3. Install whatever CSS theme you want.
4. Once that's finished, select the gear icon next to the "Reinstall" button.
5. Enable the theme you just downloaded by simply pressing A.

##### "SimpleDeck"

Do you want a quick way to install as many themes as possible? I've got the right thing for you!

1. In the Decky plugin menu from the Quick Access Menu, navigate to "CSS Loader" and select it.
2. Navigate to the Download icon at the top right and select it.
3. Set the filter to "Profile".
4. Select "SimpleDeck". It should be by me, obviously. :)
5. Select "Install".
6. Once that's finished, select the gear icon next to the "Reinstall" button.
7. Enable the profile you just downloaded by simply pressing A.

#### Audio Loader

This plugin lets you change the UI sounds of Gaming Mode along with add background music to Gaming Mode in case you ever feel bored of there being no music. This plugin is made by the same people who made CSS Loader.

1. In the Decky plugin menu from the Quick Access Menu, navigate to "Audio Loader" and select it.
2. Navigate to the Download icon at the top right and select it.
3. Navigate to "Manage Packs" and select it.
4. Set the filter to whatever you are looking for. If you are looking for UI SFX, select "Audio". If you are looking for background music, select "Music".
5. Find some audio you might like and select it.
6. Select "Install". A vinyl should start spinning to indicate it is installing.
7. Once the vinyl stops spinning, press B twice to back out of the Audio Loader store.
8. Go back to the Decky plugin menu from the Quick Access Menu, navigate to "Audio Loader" and select it.
9. Select the respective packs of audio you just downloaded from the correct dropdowns.
10. Press B twice to back out of the Quick Access Menu.
11. Press the button to access the Quick Access Menu.
12. Navigate to the Decky plugin menu.
13. Navigate to "Audio Loader" and select it.
14. Navigate to "Enable Legacy Features" and select it.
15. From both dropdowns, select whichever sounds you downloaded.
16. Close out of the Quick Access Menu.

If you want some recommendations, I have my Deck set to have "Dreamy SFX" and "Dreamy Ambience" for the UI sounds and the background music respectfully. Though, I do sometimes change it up to have "azure sounds" and "azure tides" as the respective audio playing in the background. Do note, however, that he reason why background music is considered a "Legacy Feature" is that the implementation is buggy and the developers of the plugin simply do not want to fix that. One such bug is that **if you wake up your Deck from Sleep Mode the background music will NOT immediately start playing!** *This can be fixed, however,* by simply repeating steps 11-16 but only retoggling the dropdown for background music. Alternatively, you can set up the Game Theme Music plugin (detailed further on) and a login PIN through the Settings, in order to then pre-emptively set your Deck to Sleep Mode as it is in the info page for a game in order for this music to play once you simply press B to exit out.

#### TabMaster

This plugin lets you customize what tabs in your library you will see in the Library section of the Deck's UI.

1. In the Library section of your Deck's UI, navigate to the top bar where all of the tabs are.
2. Press the Menu button.
3. Customize as you'd like!

### Recommended Decky Plugins (Non-Store)

!!! info "What Does This Mean?"

    There are tons of Decky plugins out there that are not on their official store. It takes time for a proper review process from the Decky team that people don't want to go through, or these plugins don't fit under guidelines proposed by the Loader team. Could be one reason or another. Here are a few plugins I think are worth looking at that are past the store. I've also included the respective GitHub links to downloading these plugins. From Desktop Mode, you will need to download them to a folder of your choice. (Most likely, the downloads folder).

#### (Prerequisite) Turning on Developer Mode in Decky Settings

!!! info "Developer Mode"

    This allows you to install a plugin from a `.zip` file from outside the Store. Don't worry, we won't actually be "developing" anything. The intention behind this is so that people who *do* make plugins can quickly test their builds of it before going through the review process, but this feature is available to anyone who wants to install 3rd-party plugins.

1. In Gaming Mode, press the Quick Access Menu button. You should see an icon that looks like a wall plug. Navigate to it.
2. You should see a cog icon at the top right. Navigate to it and select it.
3. In the General tab of the settings, navigate to the toggle for "Developer mode" and toggle it on.

There should now be a tab in the settings called "Developer", where the first option is "Install Plugin from ZIP File". This is how you will be installing these plugins. The first time you select the "Browse..." button there will be a 5 second cooldown on a warning that these plugins would be "use at your own risk" before moving forward, but after those initial 5 seconds that popup just becomes a warning from then on out. All plugins below will assume that from the GitHub links for them, you downloaded these plugins and "Browse"d to install them.

#### Decky MultiFramegen

If you are playing a heavy AAA game (for example, *Clair Obscur: Expedition 33*), you'll quickly notice that the Steam Deck may in fact be underpowered to handle the game at a usable frame rate while still looking good. Upscaling technology has been around for a while now as a tool PC gamers use to squeeze more performance out of their hardware. The way it usually works is by having the game render at a lower resolution (say, 480p), while an upscaling algorithm reconstructs the image at a higher resolution (for the Deck, it's 800p). This can usually increase your frame rates in-game without sacrificing too much visual quality.

Natively, the Steam Deck supports certain upscalers that games provide, such as AMD's FSR or Intel's XeSS. However, NVIDIA's DLSS normally requires NVIDIA hardware, and not every game supports the latest upscaling models. Thankfully, this plugin solves a lot of these issues. It lets you hijack the upscaling `.dll` files that certain games come installed with (particularly DirectX 12 games that support DLSS) and tell the game to use a different upscaling model instead, while it thinks it's still using the original one. This can potentially give you sharper visuals, better performance, or both.

Additionally, you may notice that even with better upscaling, the game may still not run at a high FPS. For example, when I tried running *Expedition 33* after playing around with upscaler models, I was only getting around a smooth 30 FPS. Not unplayable, but a smooth 60 FPS or higher would be nicer. This Decky plugin also allows you to use something called **MAKO FrameGen**, which generates artificial frames between real ones to give the illusion of getting a 2x, 3x, or even 4x multiplier to your FPS. There is a slight trade-off in input latency and occasional visual glitches, and it won't feel quite as responsive as a genuine higher frame rate, but it can make games look significantly smoother. "Download more FPS", if you want to keep it more layman-friendly.

!!! info ""

    <https://github.com/MWGIH/DeckyMultiFrameGen/releases/latest>

!!! warning "AI Disclosure"

    This plugin has an extensively documented use of how Claude and other AI agents are used during the development of this plugin. However, the person behind the plugin is also a seasoned developer with extensive credentials and coding knowledge that exceeds mine. As such, I would refrain from calling this plugin "vibe coded", but I think it is also fair to disclose that AI was used in the development of this plugin.

Once you've installed this plugin, I recommend installing every option you see as a backend. From there, you can play around with configurations that you like per game. My general recommendation is using "HelixSR + MAKO". The former injects DLSS 3.7 into your game, which is generally seen as better than FSR 4 that AMD provides. MAKO is then used to interpolate frames into your game to give an appearance of higher FPS. With MAKO, I recommend that you turn on Adaptive Frame Generation and then set the Target FPS to your Deck's refresh rate –– 60 FPS on the LCD model and 90 FPS on the OLED model. This way, I like to think of it as a sort of "set and forget" type deal so you don't have to continuously fiddle around with how much of an FPS multiplier you want.

#### Game Theme Music

Do you remember how on the Wii, when you selected a channel from its UI it would play music before you launched the game? Well, with this plugin you can set music to play in your Steam game's page ("launch page" as I'll call them from here on) that opens up in order to launch a game! You know, that one page where you can see your activity and achievements with the giant Play button on it? That one. Do note that this also works with the launch pages for your Non-Steam games as well. This plugin should (partially) be made by me! :)

!!! info ""

    <https://github.com/MegalonVII/SDH-GameThemeMusic/releases/latest>

!!! warning "About Store Version"

    I have this plugin on the official Decky store, but that version is **outdated**. Please use the GitHub one for now while I work to get that update on the store as well!

1. Navigate to any game in your Library and select it. Do *NOT* select Play to launch it.
2. Navigate to the gear icon and select it.
3. Navigate to "Change Theme Music..." and select it.

!!! note "Not Appearing?"

    If you are attempting this after just waking up your Deck from Sleep Mode or anything relating to a power cycle, do note that this option will not appear in that settings menu you just pulled up. To remedy this, just press B and then A again.

4. You'll see a list of YouTube videos to choose from slowly populate the UI, though if you'd like to fine tune this selection you can edit the search parameter by simply pressing A. The onscreen keyboard will open up, so use that to search for something more specific. The default search parameter will be "(game title) Theme Music".
5. Navigate to a video you think is fitting. You can select "Play" to preview the video's audio just to hear how it sounds.
6. If you've found an audio you like, navigate to Download and select it. This can take a few short seconds to a few minutes, depending on how long the video is and how fast your internet speeds are.
7. Press B to go back to the game's launch page. You should now be able to hear the song you downloaded!

#### AnyAspectRatio

The Deck's screen's aspect ratio is 16:10, when usually games these days try fitting themselves onto a 16:9 aspect ratio of modern displays. Some games already have implementations for differing aspect ratios, but most games that don't will have black bars going along the top and bottom of the screen when playing the game. This plugin allows you to then patch any game that's supported under this plugin to make the resolution fit to your Deck's screen. More immersive! All you really have to do is just click "Patch" for the game you're playing in the plugin's options in Decky!

## Vesktop (Discord)

!!! info "What Is Vesktop? Why Install?"

    Discord's main client is available for Linux, but it is very under supported. This is where Vesktop comes in. It is a modified Discord client with the Vencord mod already pre-installed. Vesktop allows you to add plugins to your Discord experience to enhance it infinitely. The main reason to install this is because of being able to join Discord voice chats while playing games on your Deck.

1. While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.
2. Navigate to "Switch to Desktop" and select it.
3. On the Dock, open Firefox to this exact guide.
4. Copy the following script made by yours truly: 
    ```bash
    curl -fsSL https://gist.githubusercontent.com/MegalonVII/cc69d04c666a3fd420ebce010cab36b8/raw/steamdeck-vesktop-appimage-install.sh | bash
    ```
5. Press on L5 on your Deck. This is the bottom most back button on the left side of your Deck. This will open up the Start Menu. Additionally, you can just tap on it from the Dock.
6. Go to the "System" section of the Start Menu.
7. Open Konsole.
8. Click on "Paste" at the top right of the window.
9. Press A.
10. Once the script is done, close out of the Konsole window. You should see an icon for Vesktop on the Desktop, but we will not be utilizing this for now. This is just for future use.
11. Press on L5 on your Deck to open the Start Menu again.
12. Go to the "Internet" section of the Start Menu.
13. Navigate to the icon for Vesktop. Right click on it.
14. Left click on "Add to Steam". This will be helpful for later, as now this program is in our Steam Library as a Non-Steam game.
15. Once it's done loading, left click on Vesktop.
16. Sign into Discord like normal.
17. Once signed in, close out of Vesktop.
18. Double click on "Return to Gaming Mode" from the Desktop.
19. Once in Gaming Mode, press the Steam button and select Library.
20. Navigate to the Non-Steam section.
21. Find Vesktop, and hover over its Library page.
22. Press the Options key over Vesktop.
23. Navigate to "Properties" and select it.
24. Rename "Vesktop" to "Discord".
25. Back out of the Properties section.
26. Launch "Discord" from your Library.
27. Vesktop will prompt you to enable their Steam Deck configuration. Enable it.
28. Press the Steam button to open the "game's" Steam menu.
29. Exit out of the "game".

!!! warning "Artwork"

    If you had installed the SteamGridDB Decky plugin, now is a good time to add artwork for your Non-Steam game!

Now, you can access Discord calls and content and participate directly from your Steam Deck. Additionally, in Gaming Mode, you can leave Discord running in the background while another game is running, meaning you can participate in voice chat while playing another game.

## EmuDeck

!!! info "What Is EmuDeck?"

    Emulators are a big part of PC gaming. However, with how the Steam Deck's OS is divided into 2 parts it's hard to manage all the games you are emulating. EmuDeck entirely removes this problem from you. It works to simplify the process of setting up emulators for your Steam Deck as much as possible and adding your ROMs as Non-Steam games to your Library. As such, it's really only a one-time setup unless you add more ROMs to your collection.

### Onboarding/Initial Setup

1. While in the Steam UI, press and hold down on the Power button until you see a menu appear.
2. Navigate to "Switch to Desktop" and select it. Go through any set up stuff that appears on screen about KDE Plasma (the name for the desktop environment) if you've never been in Desktop Mode.

!!! note "Wallet Information"

    If you unplug your Deck from the charger while in Desktop Mode, it may ask you to set up wallet information. No, it won't ask you for credit card information. Just click the option for the "classic file".

3. Click on the Firefox icon in the Dock. Go through the setup process. Firefox is the default browser on your Deck.
4. Go to <https://emudeck.com/>.
5. Click the "Download button. It should take you to the section for your operating system. Click "SteamOS". A pop up will appear comparing the early access version to the free version. Click "Download for free".
6. In the file explorer, select the Desktop. Do NOT save yet!
7. Get rid of the `.download` extension in the file name bar. (`EmuDeck.desktop.download` should now become `EmuDeck.desktop`).
8. Once that's done, click "Save".
9. Close out of Firefox.
10. In the desktop, double click the "Install EmuDeck" icon. Press "Continue" or "Execute" after that if prompted.
11. Wait for it to finish doing a quick install of necessary background tools.
12. Once it's finished, it should open the proper setup page in the EmuDeck application. You should see 2 options, an "Easy Mode" or a "Custom Mode". Easy Mode alleviates all set up struggle but installs everything it can. Custom Mode allows for you to fine tune what you actually need. We will be selecting Custom Mode for our set up. Press "Next".
13. Select your appropriate ROM directory (in my case, my internal storage), and then select "Next". This is where all your ROMs and BIOS files will go for later. If you chose the internal storage, once everything is done you should see an `Emulation` folder in your Home folder in the file explorer. If you chose an SD card, that same `Emulation` folder will be on the root of your SD card. We will ignore the "Custom Directory" option.

!!! note "EmuDeck Error"

    You may see that EmuDeck may throw an error at you which tells you to restart EmuDeck. Just ignore this. Do not be worried. My Steam Deck does not have an SD card in it, and when I clicked the option to choose SD Card, the error popped up again. My guess is it is just panicking over not finding an SD card in your Deck.

14. Select your device. In our case, the Steam Deck. Press "Next".
15. Choose the option for "Highest" integration. This means that your ROMs will show up in your Steam Library once this whole process is done, so that you can launch them directly from Gaming Mode.
16. Select the emulators you'll need for your own tastes and then select "Next". Here's a rundown of every emulator you should see.
    - **Azahar**: A 3DS emulator. It is a merger of PabloMK7's old Citra fork and Lime3DS, both of which are now discontinued.
    - **BigPEmu**: An Atari Jaguar emulator. I don't think this is pertinent to anyone in our server.
    - **Cemu**: A Wii U emulator.
    - **Dolphin**: A GameCube and Wii emulator.
    - **DuckStation**: A PlayStation emulator.
    - **Flycast**: A multiplatform Sega Dreamcast, Naomi, Naomi 2 and Atomiswave emulator. I don't think this is pertinent to anyone in our server.
    - **MAME**: It stands for "Multiple Arcade Machine Emulator". I don't think this is pertinent to anyone in our server.
    - **melonDS**: A DS emulator.
    - **mGBA**: A GameBoy Advance emulator.
    - **Model2**: A Sega Model 2 emulator. I don't think this is pertinent to anyone in our server.
    - **PCSX2**: A PlayStation 2 emulator.
    - **PPSSPP**: A PlayStation Portable emulator.
    - **PrimeHack**: A mod for the Dolphin emulator which aims to tune the controls of *Metroid Prime Trilogy* into something more inline with a modern FPS game. This means bringing proper mouse and keyboard functionality and/or dual analogue stick functionality. I don't think this is pertinent to anyone in our server.
    - **RetroArch**: A core based frontend for as many emulators as you can think of. Often times, these cores are not as updated as their standalone versions, (think `mGBA.exe` vs. its RetroArch counterpart), but it is very functional for all of its use cases. I'd only use this if you want to emulate a console that isn't on this list, or if you only want to use just one emulator for (mostly) everything.
    - **Rosalie's Mupen GUI**: A GUI frontend for a Nintendo 64 emulator.
    - **RPCS3**: A PlayStation 3 emulator.
    - **Ryujinx**: A Nintendo Switch emulator.
    - **ScummVM**: It stands for "Script Creation Utility for Maniac Mansion Virtual Machine". It is like a special translator that helps old video games run on modern computers. Many classic games from the late 80s and 90s were designed for older computers or consoles that don’t exist anymore. These games were often made using specific engines (like SCUMM, hence the name). ScummVM steps in by emulating those old environments. I don't think this is pertinent to anyone in our server.
    - **ShadPS4**: A PlayStation 4 emulator.
    - **Supermodel**: A Sega Model 3 emulator. I don't think this is pertinent to anyone in our server.
    - **Vita3k**: A PlayStation Vita emulator.
    - **Xemu**: An original Xbox emulator. Use case for this is very fringe, as most of the time you'll be able to run the same games on PCSX2, however, if any of you are into Halo this may be worth a look.
    - **Xenia**: An Xbox 360 emulator. Use case for this is very fringe, as most of the time you'll be able to run the same games on PCSX2, however, if any of you are into Halo or one of the other few Xbox exclusives this may be worth a look.

!!! note ""What About Yuzu, Citron, and Eden?""

    You may notice that I left out sections in this guide for Yuzu, Citron, and Eden. This is intentional on my behalf. For anyone familiar with the emulation scene, you may know that Yuzu was a Nintendo Switch emulator that Nintendo themselves had settled with the devs to take down from the internet. However, due to Yuzu's open source nature, this didn't stop other community members from forking the repository's codebase for their own and building on top of that as the original project was being shut down. Citron was one such Yuzu fork, while Eden is a fork of Citron due to some developers having a falling out with the other Citron devs. EmuDeck *only* provides *configurations* (ie, setting up controls and adding your games to your Steam library) for your *own* backups of Yuzu builds, meaning you'd need to scour the internet for a working backup of Yuzu before the project was shut down and place it in the `Applications` tab in your Dolphin file explorer. They will NOT provide support for it, meaning if you run into a problem using Yuzu they won't help you. This same BYO principle applies to Citron and Eden as well. Thus, I would recommend not bothering with them for the time being. You won't see further mention of them throughout the rest of this megathread.

17. Select your "Emulator and Tool Configurations" and press "Next". It should automatically select the emulators you had selected in the previous step. Additionally, it may select 2 options at the bottom of the list after scrolling: "EmulationStationDE" and "Pegasus". Deselect them, as we are working towards getting our ROMs to appear in our Steam library.
18. Configure Auto Saves if you'd like and press "Next". I normally leave this **OFF** but it is up to you. This feature creates save states every time you close out of a game in an applicable emulator so that when you reopen it later you pick up right where you left off.
19. Sign into your RetroAchievements account from here. If you don't have one, create one on their website and then come back to the EmuDeck set up process to sign into it from there. Press "Next" once finished.

!!! info "About RetroAchievements"

    RetroAchievements is a nifty thing which allows you to earn community made achievements in your retro collection of emulated games. You will simply sign into your account through the settings of your emulator if it supports RetroAchievements, and you're good to go! Note that EmuDeck configures RetroAchievements for DuckStation, PCSX2, PPSSPP, and RetroArch.

!!! warning "Regarding RetroAchievements on RetroArch"

    This is just a thing with me, and may not be applicable to you, but RetroAchievements does not want to properly load up responses on my Steam Deck. This means I cannot use it on my Deck. If this happens to you once this whole process is finished...

    1. Open the RetroArch app from the start menu
    2. Navigate to Settings -> Achievements
    3. Turn them off.
    4. Back out to Main Menu. Navigate to Main Menu -> Configuration File
    5. "Save Current Configuration".
    6. Back out and then navigate to Main Menu -> Quit.

19. Configure game bezel if you'd like and press "Next". I normally leave this **ON** but it is up to you. This feature adds borders that look like the console you're emulating if using an applicable emulator.
20. Configure Aspect Ratio for Classic Sega Systems if you'd like and press "Next". Not applicable to me, but I'd leave it as **4:3**.
21. Configure Aspect Ratio for Classic Nintendo if you'd like and press "Next". I leave this as **4:3**.
22. Configure Aspect Ratio for Classic 3D Games if you'd like and press "Next". I leave this as **16:9** usually **but in some cases I revert back to 4:3**.
23. Configure Aspect Ratio for GameCube Games if you'd like and press "Next". I leave this as **16:9**.
24. Configure LCD Shader for Handheld Systems if you'd like and press "Next". I leave this **OFF** but it is up to you.
25. Configure CRT Shader for Classic 2D Games if you'd like and press "Next". I leave this **OFF** but it is up to you.
26. Configure CRT Shader for Classic 3D Games if you'd like and press "Next". I leave this **OFF** but it is up to you.
27. Configure Controller Layout if you'd like and press "Next". I leave this as **A=A** or **"Controller Layout Match"** but it is up to you.
28. You'll see a final summary of what you're setting up on the screen. Read over it and if you're okay with it press "Finish". If not, press "Back" and reconfigure whatever you need to.
29. Wait for the installation to finish. It is installing your emulators and whatever other configurations you'll need. This will take a while, so grab a coffee or something. It may throw up a popup or 2, just accept them all.
30. Once this is done, it will throw on the success screen. Press "Next".
31. It will ask you to import games from here. Press "Manual Copy".
32. Press "Open Emulation Folder". It will open your file explorer in your installed and fully configured `Emulation` folder.
33. You'll see a `bios` folder and a `roms` folder. Both of which have folders inside of them which are very important. Here's a guide on how to get started with each of EmuDeck's emulators.
    - **Azahar**
        - Place your ROMs in `Emulation/roms/3ds` or `Emulation/roms/n3ds`.
    - **BigPEmu**
        - Place your Jaguar ROMs in `Emulation/roms/atarijaguar`.
        - Place your Jaguar CD ROMs in `Emulation/roms/atarijaguarcd`.
    - **Cemu**
        - Place your ROMs in `Emulation/roms/wiiu`.
    - **Dolphin**
        - Place your GameCube ROMs in `Emulation/roms/gc` or `Emulation/roms/gamecube`.
        - Place your Wii ROMs in `Emulation/roms/wii`.
    - **DuckStation**
        - Place your ROMs in `Emulation/roms/psx`.
        - Place your BIOS file(s) in `Emulation/bios`. BIOS is **REQUIRED**.
    - **Flycast**
        - Place your Dreamcast ROMs in `Emulation/roms/dreamcast`.
        - Place your Atomiswave ROMs in `Emulation/roms/atomiswave`.
        - Place your NAOMI ROMs in `Emulation/roms/naomi`.
        - Place your NAOMI 2 ROMS in `Emulation/roms/naomi2`.
    - **MAME**
        - Place your MAME ROMs in `Emulation/roms/mame`.
        - Place your MAME BIOS file(s) in `Emulation/roms/mame`. BIOS is **REQUIRED**.
    - **melonDS**
        - Place your ROMs in `Emulation/roms/ds`.
    - **mGBA**
        - Place your GBA ROMs in `Emulation/roms/gba`.
        - Place your GBC ROMs in `Emulation/roms/gbc`.
        - Place your GB ROMs in `Emulation/roms/gb`.
    - **Model 2**
        - Place your ROMs in `Emulation/roms/model2/roms`.
    - **PCSX2**
        - Place your ROMs in `Emulation/roms/ps2`.
        - Place your BIOS file(s) in `Emulation/bios`. BIOS is **REQUIRED**.
    - **PPSSPP**
        - Place your ROMs in `Emulation/roms/psp`.
    - **Primehack**
        - Place your ROM of *Metroid Prime Trilogy* in `Emulation/roms/primehacks/`.
    - **RetroArch**
        - Place your ROMs for various system in the folders listed in this little table. If your system of relevance is not listed in this table, I'd imagine the EmuDeck folder structure is pretty intuitive. (i.e. NES ROMs go in `Emulation/roms/nes`, SNES ROMs go in `Emulation/roms/snes`, etc.).
    - **Rosalie's Mupen GUI**
        - Place your N64 ROMs in `Emulation/roms/n64`.
        - Place your N64DD ROMs in `Emulation/roms/n64dd`.
        - Place your N64DD BIOS file(s) in `Emulation/bios`. BIOS is **REQUIRED** for N64DD.
    - **RPCS3**
        - Place your ROMs in `Emulation/roms/ps3`.
        - Install your **(REQUIRED)** BIOS directly through RPCS3 by...
            - Opening the application from the Start menu.
            - Pressing on `File -\> Install Firmware`.
            - Navigating to where your firmware file is downloaded and selecting it.
            - Closing out of RPCS3.
    - **Ryujinx**
        - Place your ROMs in `Emulation/roms/switch`.
        - Place your `.keys` files in `Emulation/bios/ryujinx/keys`. Keys are **REQUIRED**.
        - Install your **(REQUIRED)** BIOS directly through Ryujinx by...
            - Opening the application from the Start menu.
            - Pressing on `Tools -\> Install Firmware -\> Install a firmware from XCI or ZIP`.
            - Navigating to where your firmware archive is downloaded and selecting it.
            - Closing out of Ryujinx.
    - **ScummVM**
        - Place your ROMs in `Emulation/roms/scummvm`.
    - **ShadPS4**
        - Place your ROMs in `Emulation/roms/ps4`.
    - **Supermodel**
        - Place your ROMs in `Emulation/roms/model3`.
    - **Vita3k**
        - Place your ROMs in `Emulation/roms/psvita/InstalledGames`.
        - Install your **(REQUIRED)** BIOS directly through Vita3k by...
            - Opening the application from the Start menu.
            - Pressing on `File -\> Install Firmware`.
            - Navigating to where your firmware archive is downloaded and selecting it. This can be directly downloaded from Sony from [here](https://www.playstation.com/en-us/support/hardware/psvita/system-software/). Make sure once it's finished installing, select `Delete Archive?` if it shows up.
            - Navigating to where your system fonts file is downloaded and selecting it. This can be directly downloaded from Sony from [here](http://dus01.psp2.update.playstation.net/update/psp2/image/2022_0209/sd_59dcf059d3328fb67be7e51f8aa33418/PSP2UPDAT.PUP?dest=us). Make sure once it's finished installing, select `Delete Archive?` if it shows up.
            - Closing out of Vita3k.
    - **Xemu**
        - Place your ROMs in `Emulation/roms/xbox`.
        - Place your BIOS files in `Emulation/bios`. BIOS is **REQUIRED**.
            - Rename your MCPX Boot ROM Image to `mcpx_1.0.bin`.
            - Rename your Flash ROM Image to `Complex_4627v1.03.bin`.
    - **Xenia**
        - Place your Xbox 360 ROMs in `Emulation/roms/xbox360/roms`.
        - Place your Xbox Live Arcade ROMs in `Emulation/roms/xbla/roms`.

!!! info "Regarding ROMs And BIOS"

    Generally speaking, Vimm's Lair is a great resource for finding ROMs. If you need help finding a specific ROM, feel free to ask me in our Discord server.

34. Once you've configured all your necessary files, close out of the file explorer.
35. Press "Close" and then "Next" on the EmuDeck application interface.
36. Click on "Launch Steam ROM Manager". Press "OK" on the prompt to enter Gecko Mode. Do note that if you are doing without a mouse and keyboard, you will no longer be able to use the right stick for controlling the mouse and must use R2 as left click.
37. Click on "Choose". Select your Steam profile and select "Save". Advance from there.
38. Turn off the toggle for all parsers.
39. Scroll through all the parsers and select which ones that are necessary for you.

!!! danger "Regarding Cemu."

    Do ***NOT*** use the Proton builds of Cemu! It is recommended to just use the Native versions. Additionally, if you are following our bot's emulation wiki (in our case, you should only be following steps 2-5 and then placing the ROM in the correct folder on your Deck listed above), please select your ROM format as `.wua`!

40. Once finished, click on "Add Games" and then "Parse".
41. If you'd like, configure the artwork as needed.
42. Once you have the artwork you want, press "Save to Steam". Wait for that to finish.
43. Close out of Steam ROM Manager. Press "Next" on the EmuDeck application interface.
44. Read over the Emulation Hotkeys, and then click on "Finish".
45. Click on "Manage Emulators".
46. Click on "Update Configurations". This will take a short bit. Just wait. Once it's done, click "Close".
47. Click on "Update" below "Update your Emulators".
48. Click on "Update Flatpaks". Then, click OK on the popup behind the Konsole window. Wait for the Flatpaks to update, and then press OK.
49. In the EmuDeck UI, click on "Update AppImages, Binaries, and Windows Executables". Then, click OK on the popup behind the Konsole window. Wait for everything to update, and then press OK.
50. In the EmuDeck UI, click on "Back".

!!! note "If SRM Failed..."

    At this point, if Steam ROM Manager failed for you, you can follow steps 37-43 from here by simply clicking on the Steam ROM Manager button in the UI.

!!! note "If You'd Like..."

    At this point, if all you care about is retro gaming, you're done. Just close out of the EmuDeck application and return to Gaming Mode from the Desktop. Your ROMs should be populated in your Steam Library. However, the next few sections are dedicated to optional things that EmuDeck can do.

!!! danger "DO NOT!"

    Do ***NOT*** add the EmuDeck desktop app to Steam from the right click menu! I just never really got this to work, and the EmuDecky plugin should be more than enough to satisfy your needs for this app while in Gaming Mode. (More on this later).

### GyroscopeDSU

!!! info "What Is This?"

    GyroscopeDSU is a tool that allows you to use the Steam Deck's gyroscope features with Wii, 3DS, Wii U, and Switch games. If you plan on emulating these games, please follow these instructions!

1. While still in the EmuDeck desktop application, scroll down the side menu until you see "Gyroscope". Click on it.
2. Click "Install".
3. A Konsole window should appear, installing it.
4. Once finished, press any key to exit the Konsole. Or just close out of it.
5. Click on the Start menu and select "Restart".
6. Confirm the selection. Once finished restarting, your Deck should now boot into Gaming Mode.

!!! note "Why Restart?"

    You may have noticed that I said to restart the Deck instead of selecting the option in your Desktop to "Return to Gaming Mode". This is because clicking on that icon does **NOT** actually restart your Deck despite it looking like it does. We need to restart our Deck as GyroscopeDSU has now become core functionality of our Deck.

7. Assuming you've already added your games to your Steam library, select a game that may require gyro functionality.
8. Open the Controller Settings by selecting on the game pad icon.
9. Set the "Gyro Behavior" to "Directional Pad".
10. Calibrate the gyrometer by scrolling down to the "Gyro Calibration" section and selecting "Calibrate".
11. Place your Deck on a flat surface within 4 seconds of pressing the "Calibrate" button.
12. You should know if the Deck has finished calibrating the gyro if it says "Calibration Succeeded". Once it does, grab your Deck again and press the B button.
13. Press B again to exit back into the game's selection page.

!!! warning "About Gyro Calibration"

    You will need to repeat steps 7-13 for **EVERY** game that may require gyro support in your Steam library!

### EmuDecky

!!! info "What Is EmuDecky?"

    EmuDecky is a Decky Loader plugin that...

    - Lets you quickly see all the hotkeys configured by EmuDeck for your games. (i.e. For Wii U games, pressing L5 or R5 switches between the game screen and what would be the Gamepad's screen).
    - Lets you configure quick settings like bezels, shaders, etc.
    - Lets you configure aspect ratios for your games.
    - Lets you update your emulators from Gaming Mode.

    ... with more features to come!

!!! warning "Please Do This!"

    If you haven't already, please follow my instructions on how to install Decky Loader and some or all of my recommended plugins!

1. While still in the EmuDeck desktop application, scroll down the side menu until you see "EmuDecky". Click on it.
2. Click "Install EmuDecky".
3. You're done!

### EmuDeck Compressor

!!! info "What Is This?"

    ROMs of games from later generations like PlayStation 3 or Nintendo Switch can be massive in size. Some ROMs can be as big as tens of gigabytes in size! This is where the EmuDeck Compression Tool comes in. At the cost of ever so slightly longer loading times in your games (in most cases so small it's almost unnoticeable), your ROM collection can be compressed to, in some cases, half its size!

1. While still in the EmuDeck desktop application, scroll down the side menu until you see "EmuDeck Compressor". Click on it.
2. Read the information on screen about formats the compressor compresses to.
3. Scroll down until you see a button that says "Run the Compression Tool". Click on it.
4. A Konsole window and a little GUI (graphical user interface) should pop up on screen. Focus on the GUI.
5. Click on "Bulk Compression" and then click "Select".
6. It will now scan your `roms` folder and the folders inside of it for uncompressed ROMs. Check all the consoles that show up on screen and then click "Select".

!!! info "Regarding PSP ROMs"

    If you are compressing PSP ROMs, it will prompt you to choose between a CSO or CHD format. CHD format compresses a bit more but only works in emulators, while CSO format works with real modded PSPs and real modded PSVitas at a slightly more bloated file size. Choose which format you'd like.

7. Once it finishes, close out of the tool. It should close the GUI and the Konsole window. You should now be back in the EmuDeck desktop app.

### Cloud Services

!!! info "What Do You Mean By This?"

    EmuDeck also allows you to, directly from Gaming Mode, access certain browser-based applications for watching movies/TV shows/YouTube, listening to music/podcasts, and browsing social media. That is, if you configure these services to work with EmuDeck.

1. While still in the EmuDeck desktop application, scroll down the side menu until you see "Cloud Services". Click on it.
2. A popup will appear here with a few options. Click on the bubble next to the first option which says "Manage Cloud Services".

!!! note "What About The Other Options?"

    There are a lot of other options here, but in this guide we will be ignoring them. These options are for remote play clients for PlayStation or streaming to/from another PC, or are other general applications. They aren't really pertinent to media to access directly from your Deck.

3. Click "Select".
4. Tick off whichever options are relevant to you for streaming services. In my case, I selected `Spotify.sh`, `Twitter.sh`, and `YouTube.sh`.

!!! note "Discord?"

    There is an option for `Discord.sh` in this list. Ignore it. We already installed a better version of Discord earlier. :P

5. Once finished, click "OK".
6. It will then prompt you to use Steam ROM Manager for your changes to take effect. This is exactly what we'll be doing in the next subsection.

### Once Finished With ROM Compression And/Or Cloud Services

1. Open Steam ROM Manager from the EmuDeck side menu. Remember that you'd have to use Gecko Mode if it's applicable to you.
2. Toggle off all parsers by clicking on and off the slider at the top right.
3. Select the parsers for the consoles that you had compressed earlier and/or the parser for "Cloud Services".

!!! danger "Regarding Cemu."

    Do ***NOT*** use the Proton builds of Cemu! It is recommended to just use the Native versions. Additionally, if you are following our bot's emulation wiki (in our case, you should only be following steps 2-5 and then placing the ROM in the correct folder on your Deck listed above), please select your ROM format as `.wua`!

4. Click on "Add Games" on the menu at the bottom.
5. Click "Parse".
6. Click "Remove from Steam". Now that the ROM(s) with the old format(s) are gone, this step is necessary to remove the link between the emulator(s) and the old ROM(s). Additionally, if you had previous cloud services installed doing this step will update the list to include the ones you chose.
7. Click "Parse" again.
8. Click "Add to Steam". Wait for it to finish.
9. Close out of Steam ROM Manager.
10. Close out of EmuDeck.
11. Return to Gaming Mode from the Desktop by double click on its icon.
12. Get back to emulating and consuming other content!

## Unofficial Versions of Proton

!!! info "Why Do I Need One?"

    As mentioned earlier, Proton is an open source tool created by Valve which allows for Linux to create Windows environments for your Windows Steam games to run underneath Linux. Because of its open source nature, other people have taken it upon themselves to create their own versions of Proton so that these new versions of Proton can do what Valve's doesn't. In fact, some games work underneath Linux exclusively with other versions of Proton as opposed to Valve's version. If you look through ProtonDB, a community driven forum of people listing their experience on how to configure a game to work under Proton, you may see that one of your own games on Steam runs only under custom versions of Proton.

Currently, there are two methods to get unofficial versions of Proton installed and configured on your Deck. I will be going over both methods.

### Method 1 (Wine Cellar)

!!! info "What Is Wine Cellar?"

    Wine Cellar is a Decky Loader plugin that streamline the process of installing custom versions of Proton. It is meant to be used within either Gaming Mode or Big Picture while using the Steam application in Desktop Mode.

!!! warning "Please Do This!"

    If you haven't already, please follow my instructions on how to install Decky Loader and some or all of my recommended plugins!

1. While in the Gaming Mode UI, press the button to access the Quick Access Menu.
2. In the Decky plugin section, you should see a store icon at the top right. Navigate to it and select it.
3. Navigate to Wine Cellar and select "Install". This plugin should be at the bottom of the store, since it is sorted alphabetically.
4. Confirm the installation and wait for that installation to finish.
5. The Decky menu should open now. Navigate to the "Wine Cellar" tab and select it.
6. Navigate to "Manage" and select it.
7. Navigate to some 3rd-party compatibility tool, but in most cases you'll want to use "ProtonGE".

    !!! note "About ProtonGE"

        ProtonGE is a fork of Proton by a community member who goes by the name GloriousEggroll. He does a lot of unofficial Proton fixes with his versions that Valve probably won't do because of licensing agreements that he is not tied to.
8. Navigate to the latest version and select it. When selecting it, you could be selecting a button with 3 dots on it.
9. Select "Install" and wait for the download to finish.
10. Press and hold the Power button.
11. Navigate to "Restart" and select it.
12. Navigate to your game that only works under a custom version of Proton. Press the Options key once your cursor is over it.
13. Select "Properties".
14. Scroll down to the "Compatibility" section.
15. Check on the box that says "Force the use of a specific Steam Play compatibility tool". This should give you access to a new dropdown menu.
16. From the dropdown, select your custom version of Proton.
17. Press the B button twice.
18. Launch the game.
19. Happy gaming!

### Method 2 (ProtonUp-QT)

!!! info "What Is ProtonUp-QT?"

    ProtonUp-QT is a simple GUI-based application to streamline the process of installing custom versions of Proton. It is meant to be used within Desktop Mode, as the process for using it requires the restart of Steam.

1. While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.
2. Navigate to "Switch to Desktop" and select it. Go through any set up stuff that appears on screen about KDE Plasma (the name for the desktop environment) if you've never been in Desktop Mode.

!!! note "Wallet Information"

    If you unplug your Deck from the charger while in Desktop Mode, it may ask you to set up wallet information. No, it won't ask you for credit card information. Just click the option for the "classic file".

3. In the Dock, click on the Discover Store icon. It looks like a shopping bag.
4. Search for "ProtonUp-QT".
5. Install it. The icon for ProtonUp-QT looks like a green arrow in a white circle that says "PUPGUI" on it.
6. Exit out of the Discover Store.
7. Press on L5 on your Deck. This is the bottom most back button on the left side of your Deck. This will open up the Start Menu. Additionally, you can just tap on it from the Dock.
8. Go to the "Utilities" section of the Start Menu.
9. Navigate to ProtonUp-QT. Left click on it to open it.

!!! danger "DO NOT!"

    Do ***NOT*** add this app to Steam from the right click menu! It is optimally used whenever Steam is closed and then reopened, and that happens when you go from Desktop Mode back to Gaming Mode.

10. Left click on "Add version".
11. Select a "Compatibility tool" from the dropdown. In most use cases this will be GE-Proton.
12. Select a "Version" (preferably the latest) from the dropdown.
13. Left click on "Install".
14. Once it's finished installing, close out of the application.
15. Double click on "Return to Gaming Mode" from the Desktop.
16. Navigate to your game that only works under a custom version of Proton. Press the Options key once your cursor is over it.
17. Select "Properties".
18. Scroll down to the "Compatibility" section.
19. Check on the box that says "Force the use of a specific Steam Play compatibility tool". This should give you access to a new dropdown menu.
20. From the dropdown, select your custom version of Proton.
21. Press the B button twice.
22. Launch the game.
23. Happy gaming!

## Epic/GOG/Prime Games On Deck

### Method 1 (Unifideck)

!!! info "About Unifideck"

    Unifideck is a Decky Loader plugin which seamlessly integrates the games you have on Epic Games and all sorts of 3rd-party launchers with your Steam library in Gaming Mode. No need to go to Desktop Mode. It allows you to sign in to all the other extra storefronts and launchers from one single place and seamlessly integrate those games directly into the Steam Big Picture Mode experience.

!!! warning "Please Do This!"

    If you haven't already, please follow my instructions on how to install Decky Loader and some or all of my recommended plugins! Please be advised, however, that TabMaster configurations may conflict with this plugin. Please react accordingly!

!!! warning "Assumptions Made!"

    **This guide assumes you know how to install 3rd-party Decky plugins!** You can find instructions on how to do this earlier in this repository in the section for my recommended Decky plugins.

!!! warning "AI Disclosure"

    This plugin does not have much documentation on how AI is used behind it. However, Claude and GitHub Copilot do show up as contributors to the project, with Claude having contributed a decent amount of code to the project. This doesn't mean the plugin itself is "vibe coded", though, since the majority of contributions to the plugin have come from humans within the Decky plugin dev community. The best way to describe the development of this plugin would be "AI assisted".

!!! info ""

    <https://github.com/mubaraknumann/unifideck/releases/latest>

1. Once you've installed the plugin, access it via the Quick Access Menu. Navigate to the Decky section and select "Unifideck" from the list.
2. Once inside the plugin, you should see options to log in to several different storefronts that aren't Steam. Just tap on the login button for whichever storefront you're interested in.
3. Your Deck will prompt you do sign in like normal to that service. Do note that for Xbox services, you will need to have Microsoft Edge installed on your Deck. Don't worry, if you don't have it installed the plugin will prompt you through it.
4. Give it some time after sign in, but your 3rd-party games should appear in your Library as if they were regular Steam games now!

### Method 2 (Heroic Games Launcher)

!!! info "About Heroic Games Launcher"

    Heroic Games Launcher is an open source tool that allows you to quickly launch your games in your Epic Games, GOG, or Amazon Prime Gaming libraries. Their respective official clients do not officially support Linux, but Heroic does. Additionally, Heroic will automatically adjust Proton compatibility for your games, so you do not have to fiddle with it on your own. If you have any games on these platforms, this may worth a peek!

1. While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.
2. Navigate to "Switch to Desktop" and select it. Go through any set up stuff that appears on screen about KDE Plasma (the name for the desktop environment) if you've never been in Desktop Mode.

!!! note "Wallet Information"

    If you unplug your Deck from the charger while in Desktop Mode, it may ask you to set up wallet information. No, it won't ask you for credit card information. Just click the option for the "classic file".

3. In the Dock, click on the Discover Store icon. It looks like a shopping bag.
4. Search for "Heroic Games Launcher".
5. Install it. The icon for the Heroic Games Launcher looks like a blue shield with a sword in the middle of it.
6. Exit out of the Discover Store.
7. Press on L5 on your Deck. This is the bottom most back button on the left side of your Deck. This will open up the Start Menu. Additionally, you can just tap on it from the Dock.
8. Go to the "Games" section of the Start Menu.
9. Navigate to the Heroic Games Launcher icon. Left click on it to open it.

!!! warning "DO NOT?"

    Do ***NOT*** add this app to Steam from the right click menu! It is optimally used whenever Steam is closed and then reopened, and that happens when you go from Desktop Mode back to Gaming Mode.

10. Sign into whatever accounts you need to.
11. The "Library" section of Heroic will automatically populate with your games from each of the libraries you signed into.

!!! note "Store Front"

    Heroic can also give you access to the store fronts you signed into. You may be able to buy games from Epic, GOG, or Amazon directly from Heroic through their "Stores" catalogue.

12. Install whatever games you want from the "Library" section.
13. Once done with that, close out of the Heroic Games Launcher by clicking on "Quit" in the bottom left and then confirming.
14. Double click on "Return to Gaming Mode" from the Desktop.
15. From the Non-Steam section of your Steam library, navigate to and select your game on Epic.
16. Select "Play" and wait for the game to launch.
17. A popup may appear asking you to set the Proton version to Experimental. Select "Yes".
18. Close out of your game like normal once finished.

!!! warning "Artwork"

    If you had installed the SteamGridDB Decky plugin, now is a good time to add artwork for your Non-Steam game!

## chiaki-ng (PlayStation Remote Play)

!!! info "What Is Chiaki?"

    Sony's official PlayStation Remote Play client is not available on Linux. Some developers took it upon themselves to make a free and open source alternative to Sony's official client called Chiaki which supports Linux. Another developer took it upon themself to make a fork of the original Chiaki project in order to optimize the Chiaki experience for the Steam Deck, leading to the birth of chiaki-ng (formerly known as chiaki4deck). In the end, you'll have a device which is akin to a PlayStation Portal but with much more functionality.

!!! warning "Assumptions Made!"

    - **This guide assumes you are using a PlayStation 5**. The instructions shouldn't differ by much if you are using a PlayStation 4, but in terms of how to access certain settings on your PlayStation 4 it may differ. Regardless, in order for this to work you **MUST** have a PlayStation Network (PSN) account.
    - **This guide assumes that for setup, your Steam Deck and PlayStation are connected to the same network**. After this is set up, it won't matter anymore but in order to initially get started your devices need to be on the same network.

1. While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.
2. Navigate to "Switch to Desktop" and select it.
3. In the Dock, click on the Discover Store icon. It looks like a shopping bag.
4. Search for "chiaki-ng".
5. Install it. The icon for chiaki-ng looks like a circle with Kirby eyes surrounded by spikes in a triangular manner. The top spike has Wi-Fi signals coming out of it.
6. Exit out of the Discover Store.
7. Press on L5 on your Deck. This is the bottom most back button on the left side of your Deck. This will open up the Start Menu. Additionally, you can just tap on it from the Dock.
8. Go to the "Games" section of the Start Menu.
9. Navigate to the icon for chiaki-ng. Right click on it.
10. Left click on "Add to Steam". This will be helpful for later, as now this program is in our Steam Library as a Non-Steam game.
11. Once it's done loading, left click on chiaki-ng.
12. Put your Deck aside for now, as we won't be needing it for a bit.
13. Turn on your PlayStation. Sign into your PSN profile.
14. Navigate to the Settings from the Home menu.
15. Navigate to the "System" option and select it.
16. Navigate to the "Power Saving" subsection. Select "Features Available in Rest Mode" from here.
17. Make sure that "Stay Connected to the Internet" and "Enable Turning On PS5 from Network" are enabled.
18. Back out until you go back to the list of "System" sub-options.
19. Navigate to the "Remote Play" subsection. Make sure "Enable Remote Play" is enabled.
20. Leave your PS5 on but put your controller aside. Pick up your Steam Deck again. It may have gone to sleep, so just lightly tap the Power button if so.
21. On Chiaki, you should be able to see your PS5 from the menu listed as "(unregistered)". If not, close out of chiaki-ng and reopen it from the Start menu. Click on your PS5 in Chiaki.
22. The "Host" text box should be filled with an IP address. We can safely ignore this for now.
23. Click on "PSN Login". It will redirect you to your web browser and ask you to sign into PSN. Please do so.
24. Once signed in, you should see a blank page that says "redirect" at the top left. Copy the webpage's URL.
25. Refocus on chiaki-ng. Click on "Click to Paste URL".
26. Click on "Get Account ID" on the top right.
27. Put aside your Steam Deck for now and pick up your PS5 controller. You should still be in the "Remote Play" subsection.
28. Select "Link Device". An 8 digit code should now appear on screen. You will also see a timer counting down from 300 seconds (5 minutes).
29. Put your PS5 controller down and pick up your Steam Deck again.
30. Use those 5 minutes to enter that code into the "Remote Play PIN" box in chiaki-ng.
31. Once you've done that, select "Register". You can turn off your PS5 after this.

!!! info "Two PS5s?"

    You may notice 2 options for the same PS5 on chiaki-ng's interface. Note that the first option is to be selected when your Deck is on the same network as your PS5 and are streaming it from your house. The second option will say "Remote Connection via PSN" when away from your PS5's network.

32. Close out of chiaki-ng.
33. Close out of the browser.
34. Double click on "Return to Gaming Mode" from the Desktop.
35. Once in Gaming Mode, press the Steam button and select Library.
36. Navigate to the Non-Steam section.
37. Find chiaki-ng, and hover over its Library page.
38. Select chiaki-ng, but do NOT launch it.
39. Select the gear icon.
40. Navigate to "Properties" and select it.
41. Rename "chiaki-ng" to "Chiaki".
42. Back out of the Properties section.
43. Select the controller configuration button.
44. Find a community layout that works best for you.
45. Close out of that menu.
46. Close out back to your Library.

!!! warning "Artwork"

    If you had installed the SteamGridDB Decky plugin, now is a good time to add artwork for your Non-Steam game!

47. Launch "Chiaki".
48. Select your PS5 using the appropriate on screen option and get to gaming! You would exit out of it like you would a normal Steam game in Gaming Mode. (By pressing the Steam button and then selecting "Exit game").

## KDE Connect (Wireless File Transfer)

!!! info "What Is KDE Connect?"

    By default, an average Linux-based operating system does not have a desktop environment; normally it would only have a Terminal window and that's it. However, SteamOS comes bundled with the desktop environment called KDE Plasma from the KDE Community. Because the KDE Community is so generous, they will allow you to wirelessly transfer files to and from KDE environments and other devices using their KDE Connect application on both devices, so long as they are both connected to the same network.

!!! warning "Assumptions Made!"

    - **This guide assumes that for setup, your Steam Deck and your other device are connected to the same network**. After this is set up, it won't matter anymore but in order to initially get started your devices need to be on the same network.
    - **This guide assumes your secondary device is another computer**! Although it is possible to use KDE Connect with a cellular device, it is much simpler and intuitive to use it with a PC.

1. While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.
2. Navigate to "Switch to Desktop" and select it.
3. Press on L5 on your Deck. This is the bottom most back button on the left side of your Deck. This will open up the Start Menu. Additionally, you can just tap on it from the Dock.
4. Go to the "Internet" section of the Start Menu.
5. Navigate to KDE Connect and left click on it.

!!! danger "DO NOT!"

    Do ***NOT*** add the KDE Connect app to Steam from the right click menu! This application is reliant on having access to your file explorer on Deck, which is only available on Desktop mode!

6. On another device, access this webpage.
7. On that other device, open [this webpage](https://kdeconnect.kde.org/download.html).
8. Download and install KDE Connect for whatever operating system your PC is using.
9. Open KDE Connect on your PC.
10. On either device, you should see the name of the other device. Assuming you are looking from your PC simply double click on "steamdeck" from the devices list in KDE Connect.
11. Your Deck will get a notification to pair it with the other device. Select "Pair" on the notification.
12. Minimize the KDE Connect windows on both devices and leave them running in the background. In your task bar you should see an icon that looks like a cell phone with a gear on its screen. This means that KDE Connect is running in the background.
13. On your PC or on your Steam Deck, all you have to do now is right click on a file and from the context menu select...
    - **Windows**: "Send to" > "Send to remote device via KDE Connect"
    - **MacOS**: "Send File via KDE Connect". It will then ask you which device to send to. Make sure "steamdeck" is selected and select "OK".
    - **SteamOS / A Linux Distro Using The KDE Plasma Desktop Environment**: "Send to '(device name)' via KDE Connect"
14. If your file is large, wait for it to fully transfer over. Your Steam Deck will have a notification with a progress bar telling you how long to wait.
15. On your target device, your file will appear in the Downloads directory in your file explorer.

## Using Cheats In PC Games

!!! info "How?"

    Have you wanted to ever use a cheat code on your games on Steam? Well, not only can you on Windows but also on Deck too! There is a nice community of people who make things called "trainers", which feature toggle on and off switches for cheats you can use on your PC games. We will be making use of such trainers with a nifty Decky Loader plugin called CheatDeck.

!!! warning "Please Do This!"

    If you haven't already, please follow my instructions on how to install Decky Loader and some or all of my recommended plugins!

!!! note "For The Sake Of The Guide"

    For this guide, I will walk you through how I got a working trainer for *Kingdom Hearts: Final Mix* running on my Steam Deck. The process for doing this for other games should not differ by much, however.

1. While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.
2. Navigate to "Switch to Desktop" and select it.
3. In your Deck's web browser, open this webpage.
4. While looking through this very guide on your Deck, open [this webpage](https://flingtrainer.com/).
5. In the website's search bar, search for "Kingdom Hearts Final Mix". Remember that pressing the Steam + X buttons as a combo will bring up an onscreen keyboard.
6. Navigate to the result for this game and click on it.
7. Click on the download link for the standalone version that has the biggest file size. Download the `.zip` file to a location of your choice
8. Extract the `.zip` file you just downloaded from FLiNG Trainer. A `.exe` file for your trainer should have been extracted. Once that's done, you may delete the `.zip` file if you wish.
9. Close out of Firefox and Dolphin. You should now be at the Desktop.
10. Double click on "Return to Gaming Mode".
11. Press the button to access the Quick Access Menu.
12. In the Decky plugin section, you should see a store icon at the top right. Navigate to it and select it.
13. Navigate to CheatDeck and select "Install". This plugin should be near the top of the store listings, since it is sorted alphabetically.
14. Wait for it to finish, then back out as much as you can.
15. Press the Steam button.
16. Navigate to "Settings" and select it.
17. In the "System" category, make sure the toggle for "Enable Developer Mode" is switched on. Don't worry, you won't be developing anything.
18. Back out as much as you can.
19. Navigate to your copy of *KINGDOM HEARTS -HD 1.5+2.5 REMIX-* and make your cursor hover over it.
20. Press the Menu button once. If an option for "CheatDeck" doesn't show up, back out and then press the Menu button again.
21. Navigate to "CheatDeck" and select it.
22. In the "Normal" category, make sure "Enable Cheat" is toggled on. This should open a dialogue box that says "Cheat path".
23. Select the folder icon next to that dialogue box.
24. Navigate to wherever you saved the `.exe` file for your trainer and select that `.exe` file.
25. Navigate to "Save Settings" and select it. A notification should pop up at the bottom saying that your normal settings were saved.
26. Press B twice.
27. Select *KINGDOM HEARTS -HD 1.5+2.5 REMIX-*, and then select "Play".
28. You should see that the trainer launched on top of your game. Simply press the Steam button, navigate to the "Switch Windows" submenu in the category for this Kingdom Hearts collection, and select the correct window for your game.
29. In the launcher for the collection, press X to open the configuration settings.
30. For some reason, this trainer only works on the Deck when the game is configured as "Windowed". Make sure you change that in the resolution settings. Since you launched the game in Gaming Mode, the resolution will not be visibly impacted. The need to make the game windowed should not be a thing for most other games.
31. Back out of that menu, and launch *Kingdom Hearts: Final Mix*.
32. Press the Steam button, and like you did to get to the game, switch back to the window for your trainer.
33. Enable/Disable whatever cheats you'd like to use.
34. Switch back to the game's main window.
35. You can now play your game with cheats!

## Protontricks

!!! info "Why Do I Need This?"

    Let’s say you’re trying to run a game on your Deck via Proton, but something just isn’t working right. Maybe the game needs a certain .NET or Visual C++ runtime, or maybe you’re trying to get a launcher like [Battle.net](http://battle.net/) or Rockstar to actually load past its splash screen. Protontricks is a must-have tool that lets you install extra Windows components and tweak Wine/Proton prefixes (the fake C:\\ drives every game you play under Proton creates specifically for that game) directly.

!!! warning "Please Do This!"

    Make sure that you've ran the game you're trying to edit a prefix of at least once! This way, the Deck will have configured the prefix for you, and will be available for modifying in the first place! Just having the game installed is not enough!

1. While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.
2. Navigate to "Switch to Desktop" and select it.
3. In the Dock, click on the Discover Store icon. It looks like a shopping bag.
4. Search for "Protontricks".
5. Install it. The icon for Protontricks looks like a full wine glass.
6. Exit out of the Discover Store.
7. Press on L5 on your Deck. This is the bottom most back button on the left side of your Deck. This will open up the Start Menu. Additionally, you can just tap on it from the Dock.
8. Go to the "All Applications" section of the Start Menu.
9. Navigate to the icon for chiaki-ng. Left click on it.
10. Protontricks will scan your Steam library for installed prefixes. Scroll to and select the game you want to configure. Click OK. Wait a few short seconds afterward.
11. Click on OK to "Select the default wineprefix".
12. A menu will appear. If you want to install specific Windows components (like `dotnet48`, `vcrun2015`, etc.), click on the box for "Install a Windows DLL or component".

!!! note "For Power Users"

    Protontricks can also run custom commands inside a game's Proton prefix, change Wine settings, or even open a file explorer directly inside a prefix to mess with files manually.

13. Click on OK.
14. Navigate through the list that pops up. Click on a package (or packages) you would like to install. Then, click OK.

!!! info "SHA-256 Checksums"

    You may get warnings that Protontricks didn't get the proper SHA-256 checksums for the installers it grabs. This is totally fine. All a SHA-256 checksum is is a digital fingerprint for your files. Functionally, a finger, regardless of whose it is, does the same things as another person's finger, it's just that each finger has a unique fingerprint identifying who a finger belongs to. A SHA-256 checksum aims to accomplish this for digital files.

15. Follow the instructions of the installers that pop up. The app will handle downloading and configuring them in the correct Proton prefix.
16. Once the installer(s) have finished, click on Cancel 3 times to close out of Protontricks.
17. Double click on Return to Gaming Mode from your desktop to go back.
18. Launch your game through Steam. It should now run with the components you installed!

## Vortex Mod Manager

!!! info "What Is Vortex?"

    Vortex is a mod manager made by the people over at Nexus Mods. It is meant to integrate with games that have mods on [nexusmods.com](http://nexusmods.com/) with your installed libraries. Unfortunately, Vortex is a Windows only application (for now). If you've been following this guide thus far, you might think "Oh, just add it as a Non-Steam game and force it to run under Proton", but this wouldn't work as Proton creates fake C:\\ drives for every "game" you play. This means that in a hypothetical Vortex "game", you wouldn't have access to your Steam game installation library as it just doesn't exist in the fake C:\\ drive that Vortex would create. However, this doesn't stop community modders for doing things to counteract this and automate letting you use Vortex on your Steam Deck!

1. While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.
2. Navigate to "Switch to Desktop" and select it.
3. Open Firefox. It should be in your task bar.
4. Open this megathread on your Deck and navigate to this part of the megathread.
5. Right click [this link](https://raw.githubusercontent.com/pikdum/steam-deck/master/install.desktop). Click "Save Link as...".
6. In the file explorer, select the Desktop. Do NOT save yet!
7. Get rid of the `.download` extension in the file name bar. (`install.desktop.download` should now become `install.desktop`).
8. Once that's done, click "Save".
9. Close out of Firefox.
10. In the desktop, double click the "Install Pikdum's Tools" icon. Press "Continue" or "Execute" after that if prompted.
11. Wait for it to finish doing a quick install of necessary background tools.
12. Once it's finished, the Konsole window will close and you'll be back in the Desktop. Double click on the "Install Vortex" icon. Be patient, as a Konsole window will appear and take a bit to install the following:
    - Vortex
    - A Steam Linux Runtime
    - A version of GE-Proton
    - A prefix for Vortex with links in it to your Steam games installed on your internal drive (J:) and/or your microSD card (K:)
    - Any necessary Visual C++ runtimes or the like.
    - A bunch of files on your Desktop for certain games that you are to use after deploying mods for them.
13. Once that install is finished, the Konsole window will automatically close itself. You can now double click the icon on your Desktop to open Vortex. Once it's open, you may get a notification telling you that "Extensions are updated. Restart now." Please click on that restart button in that notification.
14. Sign into NexusMods if you don't already have an account with them. This can be done by clicking on the red icon that outlines a person. It will open up Firefox automatically and sign you into NexusMods. You can also create an account here if you haven't already. which is a ***required*** step since installing mods from NexusMods requires an account. Don't worry, it's free.
15. Click on the Games tab on the left.
16. Search for your game of choice and click on it. Vortex may tell you that support for that game is provided through an extension and ask you to download such an extension, to which click on the "Download" button at the bottom right of that window. Vortex will restart afterwards.
17. You may get a warning that Vortex couldn't find your game and that you'd need to manually locate it. A file explorer will appear, but it won't look like the Dolphin file explorer you're probably used to by now, rather something that looks more like old school Windows. This is just what the software acts on, as, remember, you are running these Windows applications under a virtual environment.
18. Double click on "My Computer".
19. Double click on "(J:)".
20. Click on the folder for your game.
21. Click on "Open" at the bottom right. You may get a warning asking which platform the game is installed through. Select "Steam" (if applicable, which it most likely is) and then select OK. You may also get a warning saying that your mods have been purged. Just click OK at the bottom.
22. Click on the Settings tab on the left.
23. Click on the "Mods" subsection on the top.
24. Click on the "Suggest" button to automatically map your mods to the correct spot.
25. Click on the "Apply" button next to the "Suggest" button.
26. In the "Deployment Method" dropdown below it, change it from "Symlink Deployment" to "Hardlink Deployment".
27. Click on the "Apply" button next to that dropdown.
28. Click on the "Mods" tab for the game of your choice on the left.
29. Minimize Vortex.
30. Open Firefox.
31. Go to [https://nexusmods.com](https://nexusmods.com/).
32. Search for the mods you want with your game.
33. On the mod's page on NexusMods, there should be a "Vortex" button at the top right for downloading through there. Click on that.
34. Click on "Slow Download".
35. Your mod will now install through Vortex, and you'll see once you unminimize Vortex. Please unminimize Vortex as you may never know if there are any pop ups that may arise about mod installations in Vortex which you'd need to attend to.
36. Repeat steps 29 and 32-35 as needed for however many mods you need.
37. Once you've installed all of your mods, click on one of those mods in the list. Make sure to click somewhere near the middle of its row, as to not interfere with other UI elements.
38. Press Ctrl + A on your keyboard.
39. Click on "Deploy Mods" on the bar on top.
40. You're done with Vortex. Close out of it. You may need to use one of Pikdum's post-deploy scripts. Make sure to double click on that. This will rename certain `.exe` files within your game installation such that when pressing Play on Steam the game will boot directly instead of through the launcher. Note that you'll only need to do this once after deploying mods for the first time. Games that Pikdum delivers these post-deploy scripts are as follows:
    - Fallout 3
    - Fallout 4
    - Fallout New Vegas. There is also a *pre*-deploy for this game as well. This is self-explanatory.
    - Oblivion
    - Skyrim Legendary Edition
    - Skyrim Special Edition
41. Double click the "Return to Gaming Mode" icon.
42. Navigate to the game you modded in your Library, and select it.
43. Press Play. Enjoy your mods!

!!! warning "Mods Not Working?"

    Sometimes just installing mods isn’t enough; they might need extra setup. Some games need special launch options in Steam or certain `.dll` files added with Protontricks. A quick search on Google, the game’s forums, or ProtonDB can point you in the right direction. For example, to get mods working in *FF XII*, I had to install `vcrun2022` using Protontricks and use this launch command: `WINEDLLOVERRIDES="dinput8=n,b" %command%`. It’s different for every game, so just **keep an eye out**!

## Achievement Manager

Fun Fact: Just as easy as a game on Steam can give you achievements, it can also take them away from you! That’s because achievements are handled through the Steamworks API, which developers implement into their games. Think of an API like a vending machine for computers: a program presses a button or 2 (makes a request) on the machine (a database or server) after paying (authenticating with the database/server), and out goes a soda (a response gets sent to the program from the database/server). Similarly, a game accesses the Steamworks API to give you achievements. Very rarely will a game ever take them away from you, as there's usually no reason to if you're progressing through a game normally, but it can very much happen in some cases.

But what if you could manipulate how many achievements you do or don't have for a game in your library? Let's say you were emulating an old game, but then later bought that same game on Steam. Of course, you could play through the game again the natural way through Steam this time, but that would take way more time than just (in some cases) converting and importing your existing save to Steam Cloud. And even after importing your save file, you'll notice that you don't have any achievements for your hard work registered in Steam. This is where a tool called Steam Achievement Manager comes in: originally a Windows based tool that lets you edit what achievements you do or don't have in any game in your library. The Linux community has done a great job at making a version of SAM for Linux, while I took it upon myself to streamline that process of getting that port to your Deck!

!!! warning "Use At Your Own Risk!"

    As far as I could find, there haven’t been any reports of people getting banned for using SAM or SAMRewritten. That said, **it's still smart to treat it as "use at your own risk"** This is super common with homebrew tools across all platforms, and not just Steam, however people online like to fearmonger about this tool in particular. Honestly, if you’re careful and don’t do anything wild, you’ll be just fine.

1. While in the Gaming Mode UI, press and hold down on the Power button until you see a menu appear.
2. Navigate to "Switch to Desktop" and select it.
3. Open Firefox. It should be in your task bar.
4. Open this megathread on your Deck and navigate to this part of the megathread.
5. Go to [this website](https://github.com/PaulCombal/SamRewritten/releases/latest).
6. Download the latest `.AppImage` that has the `-gtk` suffix to its filename. Save it to a convenient location. (I choose the Applications folder inside the Home section of the file explorer).
7. Double click on SAMRewritten.
8. You will see a partial list of all your games. Not every game is listed. If the game you're looking for is listed, simply click on it. If not, find it's app ID (the quickest way to do this is to open the game's launch page on Steam, click on "Store Page", and find it in the URL of the game's store page), enter it into the search bar, and click "launch appID (app ID)".
9. Click on the lock icon(s) next to the achievement(s) you want to (en/dis)able.
10. Click on the save icon near the top right of the window.
11. Click on the left arrow near the top left of the window.
12. Close out of SAMRewritten.
13. Double click on Return to Gaming Mode.
14. Open up the game's launch page. You should now see your achievements listed (or lack thereof)!
