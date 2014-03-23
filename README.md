X3TC_AL_abandon_ships_russbozz
==============================

AL_abandon_ships_russbozz script for X3TC


AL Plugin: AL_russbozz_Abandon_Ships

This is an Artificial Life plugin for the game X3 Terran Conflict to add random ship wreaks and cleanup after itself so the universe isn't overrun with usless ships floating in space.



This script leaves the default wrecks alone, so they will still be there before, during and after this script is used.
Al_russbozz_Abandon_Ships should work on any universe map (even non connected ones) due to the sector choice method built in. The ships will usually spawn in the sectors in an area centered around the player. The minimum range  is 1 sector (the ship can't spawn in the same sector as the player) and the maximum is bound only by the universe.
It runs on a Default 15 min interval but may not spawn a ship wreak every run. 
The "spawn interval" and "probability of a spawn" are both configurable in the plugin configuration menu and affect the range at which a ship can spawn. 

Every time a ship is spawned a message is recieved by the player, though with a little delay. This feature is able to be toggled in plugin configuration menu.

Al_russbozz_Abandon_Ships spawns random ships of the following classes based on probability. For example, a "scout"->M5 is much more common to be pilotless than "cruiser"->M6.
M5(~20% probability), M4, M3, TS, TS(xl), TP ,M8, M6, TL (1% probability), M7 (<1% probability)



The ships will be removed after varying amounts of time depending directaly on the spawn interval. The spawn interval can be set in the pluigin configuration menu.
There is a max limit of (10) spawned ships at any time. This was done to keep the universe clean. Once there is an open spot in the list another ship has the possibility to spawn.
One caveat, the script won't remove ships from the player's current sector (X3TC kept going kaboom on that event and it looks funny to have big abandoned ship (TL,M7) dissappear[jump] for no reason)
There are 3 spawn schemes that vary how probable a ship class is to spawn. The names are {Normal, Generous, Realistic} and each has a set of probabilities that reflect different curves. Some may not spawn a class at all, I recommend Normal for any class to be a possibility.



NOTE:
M6, TL and M7 are spawned with little or no equipment and absolutely no shields (so you cam board them w/o too much difficulty)


REQUIREMENTS:
*T-file (9314_L044) (should be able to be downloaded near where AL_russbozz_Abandon_Ships was found)
*lib_place_in_sector_russbozz (Download seperately, just like T-file)
*Community Configuration Menu : V1.51 (or higher): 03/01/2012 by Cycrow (http://forum.egosoft.com/viewtopic.php?t=218088)
*Community Configuration Menu will need a hotkey set (if you wnat to change the default settings)



INSTALL:
Drop all files into their respective folders. (all scripts into the scripts folder, t-file (downloaded seperately) into the t folder)



UNINSTALL:
In Game, goto "Artificial Life" settings then switch "Abandoned Ships" to "NO"
All ships not claimed will be removed and you will receive a message at completion of uninstall.
Save your game and quit X3TC.
Remove files listed (excluding t-file if other scripts of mine are installed, though leaving it won't hurt)

scripts folder:
al.plugin.russbozz.abandon.ships
al.russbozz.abandon.ships.config
al.russbozz.abandon.ships.events
al.russbozz.abandon.ships.main
al.russbozz.abandon.ships.spawn
al.russbozz.abandon.ships.uninstall
turret.cmd.russbozz.turret.idle

t folder:
9314-L044.xml



Thanks to
LV for the AL Plugin template (very helpful)
Apricotslice for Concept. (X3TC Create Abandoned Ships on Startup) Link : http://apricotmappingservice.com/



The Dry Stuff:

As for EULA:
Ha! a What!? use et as you wish, if you can build one better off of my code or had a few tweeks for better proformance go right ahead do it.  Use it in whatever you want.

Give credit where credit is due
~Yup don't care if you list my name on something or not; just don't blatantly claim it as your own.

- Russbozz
