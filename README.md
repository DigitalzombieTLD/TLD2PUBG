# How to use Nvidia Ansel & Freestyle with The Long Dark

#[The backstory]
Nvidia released their Ansel plugin for Unity a few years back. It was easy to integrate for devs and modders alike. 

#[The problem]
They don't anymore. Nvidia discontinued the plugin and moved it completely into the graphics drivers.
The old plugin doesn't work realiable (if at all) anymore because of the changes to the drivers.
Nvidia is making the old plugin incompatible with newer graphics drivers, bit by bit.

Implementing Ansel & Freestyle happens only in the driver through a whitelist.
Is the game you are playing on that whitelist and you got Geforce Experience installed, it will just work.
Game developers need to request the addition to that list. No chance for modders.

In very old driver version that list could be edited. Not anymore.

#[The solution]
We got no access to the whitelist. But we *do* have access to the game.
The solution is to RENAME the game to something thats already on that list.

In this case ... we just choose PUBG.

1. Remove previous AnselMods
2. Copy the "MakeMePUBG.bat" file from the zip into your TLD folder (next to the tld.exe)
3. Start the "MakeMePUBG.bat" with admin right
4. It will copy the "tld.exe" and renames the copy to "TSLGAME.exe"
5. In addition it will create a virtual folder (symlink) with the name "TSLGAME_Data" that will point to the original data folder
6. Start the game through the "TSLGAME.exe". 
7. Gamewindow title will change and the graphics drivers activates the keyboard shortcuts for Ansel & Freestyle (ALT+F2 or Alt+F3)

8. To uninstall, delete the TSLGAME.exe and TSLGAME_Data folder
9. Have fun!
