<img src="https://github.com/msx05-noah/amityOS-documentation/blob/main/amitydoc%20banner.png"
style="width:6.71354in;height:1.14086in" />

### **IMPORTANT**

1.  Take this document with a grain of salt. A good handful of stuff in
    here has either not been started, isn’t finalized, or are just
    concept ideas. I can’t promise a release date for whenever a release
    of this operating system will ever come out, nor whenever I still
    start developing this. I’m just a teenager with a bunch of ideas

2.  I know how it feels to be a solo developer, and it’s hell. Hopefully
    in the future I can get a proper team of developers and help and
    contribute with this operating system and make it awesome. Minor
    contributions like code reworks and bug fixes are also appreciated.

3.  This is now being rewritten as a Linux distribution. After talking
    with someone on Discord, I have made it my choice to make this based
    on Linux with a heavily modified Desktop Environment. This project
    seemed ambitious from the get-go, especially because I wanted it to
    be a fully working operating system built from the ground up. The
    issue with the kernel is the program compatibility, and I thought
    about it for a while. This is the final decision I’ll be making.

4.  This document is best viewed with a computer at 100% scaling/DPI in
    your browser of choice.

Document credits are at the very bottom of this document.

Additional feedback and comments; direct to blackcomb.rtm@gmail.com

### **Introduction (Mostly a rant on modern Operating Systems)**

**You may skip this part if you want to.**

Most of today's operating systems have become difficult to engage with.
They often seem more like spyware and lack the charm that their
predecessors possessed. This is especially true for Windows 11, and many
AI applications that track user activity. The trend began years ago with
the release of Windows 8 and Windows 10, which automatically enabled the
option to send diagnostic data to Microsoft.

When Windows 11 was released in 2021, it continued down the same path.
It forced features and subscriptions on users without consent and raised
privacy concerns due to its AI components. Moreover, it rendered many
PCs from the 2010s unusable simply because they lacked the required TPM
2.0 chip, an 8th Gen Intel Core or AMD Zen+ processor, or had Secure
Boot disabled or didn’t have it at all. Although there are workarounds
to
[<u>bypass</u>](https://windowsforum.com/threads/installing-windows-11-on-unsupported-devices-risks-and-workarounds.345256/)
Windows 11’s system requirements, not only are they unofficial but you
won't be getting certain updates from Microsoft.

Microsoft's decision to stop supporting Windows 10 led to one of the
largest e-waste events in tech history due to how many devices from its
time couldn’t run Windows 11. As a result of this significant
discontinuation, many people started exploring new options, with Linux
becoming a popular choice. Linux is a monolithic open-source operating
system based on UNIX, which has been around since 1971. What sets Linux
apart is its ability to be customized with different desktop
environments, including [<u>GNOME</u>](https://www.gnome.org/), [<u>KDE
Plasma</u>](https://kde.org/plasma-desktop/),
[<u>Cinnamon</u>](https://en.wikipedia.org/wiki/Cinnamon_(desktop_environment)),
[<u>Budgie</u>](https://buddiesofbudgie.org/),
[<u>XFCE</u>](https://www.xfce.org/), and
[<u>LXQt</u>](https://lxqt-project.org/). Each desktop environment
offers their own design, features, and personality, unlike Windows which
has been using explore.exe as its main environment since Windows 95.

I've always dreamed of creating my own operating system, which I plan to
call amityOS. My goal is to combine the user experience designs from
both Windows and Linux, making it user-friendly for everyday consumers.
amityOS will include essential features that are easy to manage, aiming
to provide the best experience possible. The design will draw
inspiration from earlier versions of Windows, classic Linux
distributions, and the MacOS X series, while still remaining modern and
fully compatible with the latest software.

I want it to evoke a sense of nostalgia, reminiscent of the 2000s and
early 2010s. A time where your operating system was truly yours, and
companies weren’t farming your user activity for data.

“Amity” is [<u>another word for
peace</u>](https://www.collinsdictionary.com/us/dictionary/english/amity).

This operating system takes place from 2007 - 2013.

The internal name of this operating system is OliveGUI.

This will be based on Fedora Linux with a heavily modified KDE Plasma
base.

**This is amityOS. "Familiar, Simple, Convenient.”**

### **amityOS Key Features**

#### **Bootscreen**

A simple loading bar (similar to Windows) or a splash screen (NOGUIBOOT,
like Debian or other Linux distros).

<img src="https://github.com/msx05-noah/amityOS-documentation/blob/main/amityOS%20Bootscreen.png"
style="width:3.30851in;height:2.4694in" /><img src="https://github.com/msx05-noah/amityOS-documentation/blob/main/Bootscreen%20(neonGraphics%20take).png"
style="width:3.29226in;height:2.46354in" />

My proposal and neonGraphics proposal

#### **Basic Setup Environment**

A Windows Preinstallation Environment-styled setup process with:

- End User License Agreement acceptance

- Locale and language configuration

- Drive selection and partitioning (uses Windows drive format, Linux is
  recognized)

- Other essential first-stage setup steps (ex. Configuring drivers)

- A section for recovery tools just in case amityOS has an issue.

#### **Boot Menu/Loader**

A boot menu when loading from installation media, similar to Arch Linux
or other Linux installers. It will also have options to boot to UEFI
FIrmware Settings (The computer’s BIOS Settings) and load Memtest x86, a
diagnostic program.

This boot menu will also be able to list out Linux and Windows installs.

#### **Recovery Environment**

A complete recovery environment with working tools, inspired by but not
identical to the Windows Recovery Environment. Includes custom takes on
System Restore, Command Prompt, and similar utilities.

#### **Drive Backups**

In the case that your computer’s drive is faulty and amityOS is on it,
you have the option to make a backup of the system (which keeps files
and all data to another drive or partition), and even make image backups
of the drive.

#### **Initial Setup Page (Out-of-box Experience)**

An Initial Setup page built from the ground up, complete with an intro
video.

- User account creation with optional profile picture and password

- Desktop and system customization

- Connecting to the internet

- Whenever they want to be reminded of updates

- What apps they want to install on first boot

- Instant desktop customization (Choosing the style of different
  components)

- Which edition they can install (Part of first-time experience)

- Optional guided tour at the end

The background music \[is planned to\] be an instrumental of I Will Find
You or an edited version of Just The Way You Are by Milky and it’ll stop
playing after the Initial Setup ends.

#### **Intro Video**

A 3D animated video of a dove flying off from a branch and into the sky.
It will then freeze in place while the “amityOS” wordmark appears below
it. This is similar to the Windows XP OOBE
video.<img src="https://github.com/msx05-noah/amityOS-documentation/blob/main/Intro%20video%20stroyboard.png"
style="width:7.32023in;height:1.91103in" />

The storyboard by me.

#### **Logon Screen**

A clean login UI with accessibility options and shutdown controls.

You can make new users from the Settings Panel and logon screen, and you
can make up to 15 users. The different types of users are…

- Bureaucrat (Administrator, all permissions)

- Normal (Some limitations: Can only look through your files.)

- Guest (Enabled by default on amityOS Server, Slightly restricted)

If your device supports biometric data, you can login to amityOS with a
fingerprint reader without the need for a password. The latter is
optional. Repeated incorrect password or misidentified biometric data
will lock the account from 1 minute to 1 hour.

#### **User Interface Elements (by default)**

- **Begin Page** - It lists all applications, settings, utilities, and a
  search function. Power options are in the Actions Bar.

- **Programs Bar** - Shows running programs. You can pin them to the bar
  and change how running applications look.

- **Actions Bar** - From the left side, you can check and configure
  notifications and its respective settings. From the middle, you can
  see the date and time. From the right, you can enable some quick
  settings like enabling a dark theme, power options, volume and network
  settings, and others.

#### **Begin Page Styled (unfinished)**

\*This is something that can be changed during Initial Setup.

The default design of Begin Page is recently used apps on the left,
quick actions on the right. A full screen mode (styled like KDE’s
Application Dashboard) is a secondary option.

#### **Multiple Desktops**

On the far right side of the Programs Bar, there will be 4 icons that
are multiple desktops. You can remove and bring them back and can
disable them from the Settings Panel. Multiple desktops are good for
productivity and just like Windows 11, you can have a wallpaper and
title for each.

#### **System Sounds**

A full system sound suite, including:

- Startup/Shutdown, Logon/Logoff

- Battery Charging, Low, and Critical

- Hardware Connect, Disconnect, and Fail

- System Hand (Critical Stop), Question (Error?), Rights (UAC), and
  Warning (Exclamation)

- Device Connect / Disconnect / and Fail

- File navigation and trash empty

- Generic Ding and Notification

- and Network Connect and Disconnect

There is expected to be a collection of 4 sound schemes.

- amityOS, the default sound scheme. (Already finalized, thanks
  neonGraphics!)

- Purify, most of the sounds here will be calm (Inspired by [<u>Windows
  XP Samsung OEM</u>](https://youtu.be/J4AXrPwQyCs))

- Casual, basic generic-sounding system sounds. Nothing too special.

- Classic (A mix of Windows 9x, Windows XP, and KDE 2).

#### **System font, coding languages, and architecture.**

amityOS is planned to be coded in C, C++, Python, Assembly, Qt, and GTK.
Potentially Rust. The base itself will be Fedora Linux, but with a
heavily modified KDE Plasma.

The default system font is Hind Kochi, and this will be a x86_64 bit
operating system. A fork of OliveGUI might be designed for IA-32 bit
systems, but I won’t know how it’ll be getting done.

#### **DoveDiscover**

The \[planned\] default browser for amityOS.

This might be a Firefox fork with edited components, relying on being
secure, private, and stable. This is planned to be styled after 2009 -
2014 Firefox without ripping off Mozilla entirely.

#### **Themes**

The OS will support desktop composition. Users can choose between:

- Default “amity” theme. (Inspired by [<u>Aero
  Basic</u>](https://betawiki.net/wiki/Windows_Basic))

- “amityGrand” theme. Transparent and animated. (Optional)

- Ones resembling Windows 9x, Ubuntu 10.04, KDE Oxygen, etc.

“amity” Theme will have 3 color variants. Steel (Gray), Blueberry
(Blue), and Coal (Black; dark theme)

<img src="https://github.com/msx05-noah/amityOS-documentation/blob/main/amityOS%20theme%20demos.PNG"
style="width:3.82813in;height:2.38993in" />

Theme examples (Concept)

#### **Wallpapers and Default Wallpaper**

The main types of wallpapers will be…

- Nature (Leaves, trees, flowers, etc.)

- Architecture (City buildings, bridges, etc.)

- Abstract (alternate name is Unique)

- Standard (Colors and normal designs; plain)

- Community submitted.

- Branding wallpaper (default; depending on edition)

The default wallpaper of amityOS should be similar to [<u>Harmony in
Windows 7</u>](https://windowswallpaper.miraheze.org/wiki/Harmony),
which was created and rendered by Chuck Anderson. It should be a blue to
white gradient and streaks while the amityOS logo in the bottom right
corner positioned like Windows XP, representing the peaceful aura of
this operating system while referencing legacy pieces of software.

DIfferent colors depending on the version of amityOS.

There should be several resolutions for this wallpaper.

- 800x600 (Smallest resolution amityOS can handle)

- 1024x768 (SD 480p)

- 1152x864 (XGA, 480p)

- 1280x720 (HD, 720p)

- 1280x960 (QuadVGA, 720p)

- 1280x1024 (720p)

- 1366x768 (FWXGA, 720p)

- 1600x900 (WSXGA, 720p)

- 1920x1080 (FHD, 1080p)

- 1920x1200 (WUXGA, 1080p)

- 2560x1440 (2K)

- 3840x2160 (WQUXGA, 4K)

- 3840x2400 (4K).

The logon screen wallpaper is a similar concept, but the dove is big and
transparent on the left accompanied by a blue gradient.

#### **Iconography**

Skeuomorphic, Windows Aero-inspired icon design; realistic, and highly
polished. Takes some small inspiration from Ubuntu 10.04 and KDE 3.5.
Some pieces of modern UI will show but they won’t be as noticeable.

Take some notes from
[<u>IconFactory.</u>](https://design.iconfactory.com/microsoft-windows-vista-icon-suite/)
and [<u>ReactOS Desktop
Icons</u>](https://reactos.org/sites/default/files/Mizu-Desktop.png).

#### **Daily-Driver Ready**

Stable and feature complete to use as your main OS.\
(“i use amityos btw :3”)

#### **Device Configurator**

Similar and has the same functions as Windows’ Device Manager.

#### **Development branches (like Windows Insider Program)**

- Stable (Public) - Recommended for main use. Bugs fully removed and
  will run nice.

- Beta - Polished features or new features. Expect running into bugs and
  issues.

- Canary - Not recommended for main use. Apps and features will not be
  as functional and this is mostly used as a kernel testing ground.
  Expect instability.

- Release Preview - Decent to use, but bugs around small corners are
  expected.

After around 90 - 360 days of use, some pre-release builds of amityOS
will no longer function after a specific date. It will display an error
message in the style of a verbose boot screen telling you to either use
a finalized build of amityOS or a later compile.

#### **Version and naming scheme**

amityOS releases will be codenamed after various pieces of media or
landscapes.

Version naming will be like Ubuntu.

As an example, amityOS \[Codename\] 24.09 translates to amityOS
\[Codename\] Sept. 2024 Release.

#### **Multiple Editions**

Several SKUs, including:

- Personal - Designed for personal use

- Advanced - Meant for businesses

- Junior - Meant for less-powerful PCs

- Enterprise - Designed for big IT companies.

- Server - Web-hosting for major infrastructures.

and a special extended support release called…

#### **amityOS LWSR**

LWSR stands for “Long-While Servicing Release”.

Similar to Windows IoT Enterprise LTSC, This gets longer support than a
usual amityOS release, and it’s completely stripped of any useless
resources and applications and only includes \[your definition of\]
basic essentials. This is also a good time to mention…

#### **Product Lifecycle**

- Usual releases of amityOS will get around 3-5 years of support. A new
  release is expected to already be out by then. Junior gets the least
  amount at 2 years.

- Enterprise and Server editions get more than that at around 5-8 years.

- amityOS LWSR gets over 10+ years of support; most years will be 12,
  and a new release of amityOS LWSR releases every 4 years.

#### **Windows Application Compatibility**

Wine will be used for this process, especially because this is Linux.
Zorin OS seemed to do extremely well with this so maybe we could dig
more into it.

This might have some issues.

*\*The next 4 sections will be editable depending on the configuration
you set during OS setup.*

#### **Optional additional apps**

Some editions (like Home) can come preloaded with extra software; others
remain minimal. There will be a program to control what programs come
preinstalled during the Initial Setup, and you have the option to choose
what gets installed on first boot and what doesn’t. You must have an
internet connection.

This automatically restarts the PC.

This can be changed after the first logon.

#### **Basic Applications**

Bundled apps include:

- Painting Program - “Creativity”

- Text Editor - “Jotter”

- Calculator

- Terminal, it will accept Linux commands and some Windows ones.

- Screenshot Tool - “Snipper”

- amityOS Help Center - guide for getting around the operating system

- System tour - “Get Started”. It’ll be both interactive and animated,
  and an HTML version will be made just like Windows XP.

- File Navigator - “Folder Venturer”

- Settings Panel

- Mail program

- Media Viewer - “Watcher”; can view Photos, Music, and Videos.

- Accessibility Tools - “Ease of Use” center

- Archive extractor and other folder related goodies

- Alarm and Calendar program; make timers and reminders\
  …and more.

#### **Preinstalled Third-Party Software**

This contains both open and closed source software. A few examples are…

- Waterfox for private and advanced web browsing, that is if you don’t
  like DoveDiscover. Other alternatives include Vivaldi, Zen, Firefox,
  and other Firefox/Chromium forks.

- VLC Media Player for media watching and listening.

- LibreOffice, a free and open source take on Microsoft Office.

- KDevelop, VSCodium, or Notepad++, software development programs to
  enhance your workflow.

- Either Krita or GIMP, good alternatives if you don’t like the built-in
  amityOS art program. Not sure about Photoshop at the moment.

- foobar2000 for listening to music and audio files.

- Some other FOSS (Free and open source) and closed-source programs.

More can be added if the user says so.

LibreOffice only comes with amityOS Advanced and onwards, Personal and
Junior users have to install manually.

#### **(Optional) Software Center**

A “Store” that pulls installers from a hosting website, their respective
hosters, or a trusted software repository. It retrieves the installer
and extracts the program directly on the system. Requires an active
internet connection to pull the information.

This function is inspired by the [<u>Application
Manager</u>](https://reactos.org/sites/default/files/Mizu-AppManager.png)
in ReactOS, which does a similar action.

#### **Folder Venturer**

A simple file browser with similar functions to any operating system
like searching files, managing drives, making new folders, organizing
folders, and other things. This operating system is planned to use the
Windows drive format (ex. C:\\ like Windows and ReactOS.

Concept art of the default layout:

<img src="https://github.com/msx05-noah/amityOS-documentation/blob/main/Folder%20Venturer%201.jpg"
style="width:2.97627in;height:2.46387in" /><img src="https://github.com/msx05-noah/amityOS-documentation/blob/main/Folder%20Venturer%202.jpg"
style="width:2.58854in;height:2.43029in" />

Default folders:

- Desktop

- Documents

- Downloads

- Songs (Music)

- Photos

- Clips (Videos)

- Recent Files

When you first open Folder Venturer, you'll be greeted with a First Time
Setup program. You’ll be able to change how the style of the UI looks.
Some choices include…

- Traditional - Folder redirects on the side and command bar at the top
  with actions to search directories and drives, change folder sizes,
  address bar, (optional) Up button to go up a directory, and other
  choices.

- Windows 8 styled - command bar is replaced by a ribbon.

- Windows Classic styled - The left side had a details pane and a
  classic folder pane.

- LXQt / Thunar styled - Modified Windows Classic style with a \*NIX
  look.

- Custom - Make it how you’d like.

#### **Settings Panel**

This is the control center of amityOS. Here, you’re able to customize
all the corners of amityOS to your liking. Some sections are listed
depending on the edition of amityOS.

This has many different sections like…

- **System and Defense** - See your system specifications and protect
  yourself in the online world with amityOS’s built-in Threat Protection
  software. You can also uninstall and configure programs.

- **Hardware** - Configure devices that are compatible and connected to
  your computer. You can change settings related to your keyboard, mouse
  and cursor, monitor, and other external devices like SD Cards, Flash
  drives, etc.

- **Network and Connectivit**y - Set up or configure your Ethernet,
  Wi-fi, or modem connections. You’re even able to set up NASes,
  servers, etc.

- **People** - Create and manage user accounts and change their
  hierarchy.

- **Nation and Region** - Manage keyboard layouts, system languages, and
  other translatable parts of your system.

- **System Customization** - Play around with system sounds, themes,
  wallpapers, colors, screen resolutions, and much more! This is one of
  the main selling points of this operating system.

- **Accessibility Options** - Make amityOS easier to use for people with
  disabilities. You can change text size, enable a screen reader,
  hearing controls, etc.

- **Additional Options** - Some settings that don’t fit a category are
  put here instead, like x86 components.

#### **System Languages**

This operating system is planned to come in different languages for
non-English (United States) speakers. These include but are not limited
to…

- English (International and other variants)

- Spanish (includes Central/South America variants)

- French (includes African variants)

- Italian

- German (with translated locales from Austria and Lichtenstein)

- Portuguese (Portugal and Brazil variants)

- Swedish

- Norwegian

- Finnish

- Russian

- Ukrainian

- Chinese (includes Cantonese from Hong Kong SAR, and Taiwan variants)

- Japanese (with Kanji, Hiragana, and Katakana variants)

- Korean

- Vietnamese

- Haitian Creole (modified French pack)

- Arabic

- Persian

- Urdu

- Hindi

- Bengali

- Bosnian

- Serbo-Croatian (Cyrillic and Latin script swapable)

- Indonesian

- Thai

…and many more.

#### **Entertainment**

A few classic games like…

- Solitaire

- Chess

- Minesweeper

- Poker

- Hold ‘Em

- Generic Matching Game

- Tower Shooting game (totally NOT Angry Birds.)

To play games with proper animation, you’ll need a video card supporting
graphics acceleration. Animations will be disabled by default.

Sample media like…

- Sample Images. May include animals, nature, or other things.

- Sample Music. Up to 5-8 songs, artists and other important metadata
  will be kept.

- Sample Videos. Can be a water stream, animals in the wild, or any
  other scenery.

Some other entertainment might be a TV viewing program similar to
Hyponix from Linux Mint. Internet connectivity required.

#### **Frequent Updates**

A built-in update service accessible from the Settings Panel.

This will be a rolling release operating system, so you’ll be getting
the latest and greatest updates to make amityOS more stable!

#### **Telemetry**

There will be little to NO telemetry in amityOS.

The only form of “telemetry” will be user data, which you can either
disable or enable. By enabling it, we will be able to see how your
experience is with the operating system and that’ll give us notes and
tell us what we should fix in the future.

#### **Artificial Intelligence**

amityOS will **not** have a <u>single</u> AI component. Some AI tools
like ChatGPT might be available as an app for amityOS, but no component
of amityOS is planned to be AI-based.

As stated previously, this is meant to be an operating system that works
how you want it, not the other way around.

#### **Feedback app**

Send feedback to the developer(s) of amityOS. You’ll have to…

- Use an email (required) or your PC username (optional)

- Report what’s the issue with the operating system; provide images
  and/or videos.

- Explain how we can fix the issue.

- What else you’d like to see in amityOS.

#### **Design Language**

Amity Design Language will combine the familiarity and depth of classic
desktop interfaces with the clarity and simplicity of modern user
experience design. It will be a mix of Skeuomorphism (pre-iOS 7 and
pre-Windows 8) and Modern Design (Anything after 2013). The goal is to
provide calm, usable computing that balances warmth and clarity.

### **Miscellaneous things**

#### **Open Source versatility (WIP)**

amityOS is planned to be open source, under its alternate name
“OliveGUI”.

#### **Promotional Material**

This is subject to change!

#### **Custom Drivers (Unsure)**

Drivers built from the ground up, leveraging Windows-style driver
models. Transparent themes can still be used without drivers but they
will be buggy.

This might be a challenge.

#### **Gaming (Unsure)**

While this operating system isn’t entirely focused on gaming, some
gaming software, video drivers, and extras might be included.

Steam is expected to run mediocre if it ever comes to amityOS.

#### **Runs on Older Hardware**

Optimized to run smoothly on 10–15-year-old machines, similar to
lightweight Linux distros. ThinkPad support will be golden. Modern
hardware is very recommended

#### **Verbose and NOGUI boot configs**

If you don’t like how the amityOS bootscreen is and would rather see
your PC information on the bootscreen, then you can enable it that way.

#### **Easter Eggs**

This is subject to change!

### **amityOS Extras (Codename Asahina)**

This is a pack to add some additional addons to amityOS like programs,
themes, sound packs, and other things. This is similar to Microsoft
Plus! from Windows 95, Windows 98, and Windows XP, and Windows Ultimate
Extras from Windows Vista. This is a separate download.

Here’s what I have planned.

#### **Widgets**

Similar to Windows Sidebar / Desktop Gadget Gallery, macOS Sonoma’s
dashboard, and KDE Plasma’s Widgets, amityOS might have desktop widgets
that can display real-time information. You can have them anywhere on
the desktop or stick them to the side of the screen. Here’s what I have
planned…

**Clock** - Displays the current time, and you can choose your own style
and timezone.

**Notes** - Lightweight sticky notes gadget you can use for reminders or
random thoughts.

**News** - Displays headlines from your chosen provider, and it updates
every 3 - 6 hours. Requires an internet connection.

**Daily Scripture** - Get daily quotes from your chosen holy book. You
can choose the Bible, Quran, Torah, Buddhist teachings, etc. Requires an
internet connection.

**Puzzle** - Word games, riddles, and brain teasers.

**Mini Game** - Same practice as previous entry.

**Search** - Find something you’re looking for, either on your computer
or the internet. Internet connection required for web searches.

**Photo Reel** - Choose a folder of photos to show off in a mini
slideshow.

**System Monitor** - A resource monitor, but smaller and in gadget form!

**Media** - Play a small video or a piece of music. Playlist support is
planned.

**Translator** - Small little language translator on your desktop with
potential browser integration. Translate up to 50+ languages.

**Clipboard History** - Similar function to Windows 11. View what you’re
copied and pasted in recent times.

**Battery (Laptop Only)** - Displays your battery percentage and warns
you when below 15%.

**Mood Forecast** - Custom messages either telling you to be clean or do
some personal activity. Tied with a teenage mentality or little joke.

**Daily Dove** - Same practice as previous entry, but it’s peace
centered and optimistic.

#### **Additional Programs**

This is subject to change!

#### **Additional Games**

This is subject to change!

#### **Additional Themes and Sound Schemes**

This is subject to change!

#### **Custom boot screens**

If you don’t like how the current amityOS bootscreen looks, you’ll be
able to change it. A patcher for the bootscreen will be provided and the
whole process will be managed by a Bootscreen editor tool designed for
amityOS. This can also change the verbose bootscreen if you want it to.

The bootscreens will most likely be references to pieces of media I
enjoy, taking slight inspiration and influence from them. The media in
question might be songs, games, franchises, shows, UI designs, UXes, and
other things I enjoy.

### **Document credits**

- msx05 / Noah - Main writer

- neonGraphics - Logo and Bootscreen

More to come soon!
