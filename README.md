# SPK_RAS
Random Ambient Sounds for Arma 3 Epoch

This tiny simple script will give you the ability to insert custom soundfiles (.ogg) and give you back the background ambience like in Arma 2 DayZ Epoch.
The sounds are executed random and you can setup the timers.

Have fun with it and feel free to use it at your server.
Report bugs please.


How-To:

- Edit your description.ext and insert your custom soundfiles to the class you want to use.
  (CfgMusic is recommended, but you also can use CfgSounds)

- Copy your soundfiles in the folder related to the path you setted in description.ext.

- Edit your init.sqf and copy/paste the line as in the example file.

- Copy the folder "custom" to the root of your missionfile.
- If you want to put this anywhere else, you have to change the paths.

--------------------------------------------------------------------------------------------------------

To configurate the script, you only need to edit "RAS_settings.sqf"

_rasStyle:
//choose which way you want to run the script -> true = CfgMusic | false = CfgSounds
//CfgSound = every player is forced to hear the sound with your volume configuration in description.ext
//CfgMusic = the player can decide about music-volume, also he can deactivate it

rasTracks:
//Array of used soundfiles you described in description.ext

_minGap:
//(number in minutes) Minimum gap between the tracks

_maxGap:
//(number in minutes) Maximum gap between the tracks

_addT:
//(number in minutes) Maximum random added time to the gap

_secGap:
//(number in minutes) Security time between tracks
//Triggers only if _rasStyle = false; is used

--------------------------------------------------------------------------------------------------------

This script will gets updated and improved by time (when i get it) :)

cheers
