# Unreal Tournament Single Player Mutators

This package allows you to play the single player campaign with mutators!  This was originally written for my [Crowd Control and Randomizer mutators](https://github.com/theastropath/UT2K4CrowdControl), but seemed like it might be useful on its own!


## Compiling

I have been compiling this project using [UMake](https://github.com/SeriousBuggie/unreal-umake).  Simply put the contents of this repository into a UT2k4SPMutators folder in the main Unreal Tournament 2004 install directory, then drag the files inside the Classes folder onto UMake.
The compiled .u file will be put into the System folder.


## Installing

Either compile the .u file or download it from the Releases page and put it into the System folder of your Unreal Tournament 2004 installation. Once that is done, you must make some changes to your UT2004.ini file in the System directory.  Note that once this is done, you will need to create a new Profile and start fresh.  At the moment there is no support for loading normal profiles.

Open the file and find the line that starts with "SinglePlayerMenuClass=" and change it to

```
SinglePlayerMenuClass=UT2k4SPMutators.UT2K4SPMutator_Main
```

Next, find the line that starts with "GUIController=" and change it to

```
GUIController=UT2k4SPMutators.UT2K4GUIControllerMutator
```

and you should be able to create a new save in the Single Player menu and use whatever mutators you want!

If you want to revert to the normal single player campaign, you can change those lines back to:

```
SinglePlayerMenuClass=GUI2K4.UT2K4SP_Main
GUIController=GUI2K4.UT2K4GUIController
```

## Adjusting Mutators Used in Campaign Mode

After you have created a Single Player profile, go to the Mutators tab before starting a match.  Select the mutators you want to use (eg. Crowd Control, Simulated Crowd Control, or Randomizer), then start the match.  These mutators will be remembered for any subsequent games, but can be changed at any time between matches!

## Feedback
  
Join the Discord server to discuss this mod or to provide feedback: https://mods4ever.com/discord

  

