# SpotlightX

![When typing in the start of one of the start menu programs, it will autocomplete:](https://i.imgur.com/YfQRsqj.gif)

## Quick Start Guide

| Release Version | Download |
| --------------- |:-------------:|
| 0.0.1           | [Download](https://github.com/TorinFelton/SpotlightX/releases/tag/V0.0.1) |
| 0.0.2           | [Download](https://github.com/TorinFelton/SpotlightX/releases/tag/V0.0.2) |


### Installation

1. Select a version above or follow the link for the latest stable version. [Stable Version](https://torinfelton.github.io/SpotlightX/)

2. Hit "Download Latest" to download the setup file.

3. After download is completed go through set up wizard.

4. After setup wizard is completed restart your computer.

5. Use hotkey ``**ALT+S**`` to reveal SpotlightX.

### Getting Started

- To Launch: Press ``**ALT+S**``  
Will launch search bar.

- Autocompleting Commands: ``**TAB**``  
Pressing **TAB** when typing a command will allow you to autocomplete the command.

- To search google: Type ``"search <your Search Query>"``  
Opens default browser and searches via google.  
Example: **search** SpotlightX Help

- Open Windows Settings: Type ``"setting <settings page to visit>"``  
Will open corresponding windows settings page.  
Example: **Settings** nightlight

- To add a file path: Type ``"addpath <full folder path to add>"``  
This will allow you to add a program, file, and or a shortcut to SpotlightX that can be launched directly from the commandbar. 
Example: **addpath** C:/User/ect

- To remove file path: Type ``"removepath <full folder path to remove>"``  
This will remove an added program and restart the program.  
Example: **removepath** C:\User\ect

- Launching Programs: Type ``"<program or file name>"``  
As long as the program or files path has already been added then the file will be opened with the system's default program that is configured to open them.  
Example: **Notepad** or **file.txt**

- Changing background gradients: ``"background <color1>:<offset><color2>:<offset2>"``  
This will allow you to tailor the command bar's gradient colors to your liking. You can find examples [here](https://torinfelton.github.io/SpotlightX/customisation.html)

- Changing text color: ``"textcol <color>"``  
Changes the text & caret color to the input value.

- Restart SpotlightX: ``"reload"``

## Overview

![The bar upon launch looks like this, and will disappear when you click off or press Esc:](https://i.imgur.com/ZsW1MnZ.png)

If you don't want to read a bunch of text, visit the [SpotlightX Site](https://torinfelton.github.io/SpotlightX/)

SpotlightX is a minimal, simplistic command bar that makes launching programs or searching things a lot easier than they are with the default Windows 10 search bar. In the future, I intend to go beyond the basic feature set of the Windows 10 search bar and make even more useful commands, while maintaining the simple look and feel of the program throughout (and trying to keep it lightweight).

The general motivation behind this was that sometimes the Windows 10 Search Bar can behave strangely and not do what the user would like, or doesn't have the shortcuts quickly available. For example, even if you type in the same few programs every day to launch, they take a while to be found and sometimes the first result that comes up is a Bing search instead of the program you have installed... SpotlightX doesn't do this, there is no weird determination of results or forcing Bing search down your throat, it just does what you need it to do and disappears after.


## Current Features

- All shortcuts in the System's start menu & the user's start menu will be loaded and can be run directly from the bar
- You can load any program, file, folder, and or shortcut in by adding the file path. (See Getting Started)
- Working tab-autocompletion based on available programs/commands
- Minimalistic Icons & No scary error messages
- Hotkey (Alt + S) to bring up SpotlightX, program runs quietly in the background without interruption and window disappears when not needed
- Search function for Google (though in future you'll be able to change search engine)
- Ability to launch windows settings from simplistic command ``"settings <settingpage>"``, all settings page names are autocompletable.
  The autocompletion for these setting names has used the ms-settings URI list for all locations [here](https://github.com/TorinFelton/SpotlightX/blob/master/CleanUI/CleanUI/config/ms-settings.txt)
- Ability to change background + text color

## Goals/Upcoming Ideas

- Custom commands implemented via JSON (hopefully with a UI for the user to edit the JSON with)
- Custom actions for these commands to carry out (e.g run program, set setting, search something, etc.)
- (DONE) Ability to customize icons + style of bar (gradient, coloring, etc.)

![Launch Settings Function](https://i.imgur.com/p7wMNS6.gif)

## Troubleshooting Guide

![Simplistic Error Message - to show invalid command input](https://i.imgur.com/TibVPGY.png) (Example of error icon)

1. **Error Popup** ``"Could not register hotkey, exiting program..."``  
    - This message may appear upon launch of the program due to one of two things; the program may already be running and therefore cannot re-register the hotkey as it is in use, or there is another program which is using this hotkey. Press Alt + S to check if the SpotlightX bar already pops up, or if something else does.

2. **Error Popup** ``"Couldn't load folder: <folder path>"``  
    - This message will appear when the program has attempted to find a folder at the given path from a previous addpath command, but has failed. Please check that the path is valid (no typos, strange characters, pointing to a file and not a folder, etc.) and make sure to use the command removepath to remove the incorrect path from the path list.

3. **No response with ALT+S hotkey**  
   - Check that program is running. Relaunch program and try again.  
    - Ensure hotkey is not being used by another program. 

4. **SpotlightX not active on startup**  
    - Ensure it is enabled in task manager startup apps.



|[Developed By Torin](https://github.com/TorinFelton/) |
[Buy me a coffee](https://buymeacoffee.com/torin)|

## Link Tree

- [Submit an Unknown Error](https://github.com/TorinFelton/SpotlightX/issues)
- [SpotlightX Page](https://torinfelton.github.io/SpotlightX/)  
- [SpotlightX Help](https://torinfelton.github.io/SpotlightX/help.html)