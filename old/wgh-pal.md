## Windows Glitch Harvester tutorial for PAL Corruptions

[← Home](https://ptrguide.github.io)

### What you will need:

1. Latest version of Windows Glitch Harvester
2. PaRappa the Rapper 2 PAL version

### Steps:

Start up PCSX2 and Windows Glitch Harvester.

When you start the emulation, press "Hook process" in Windows Glitch Harvester and find ''pcsx2'' in the search.

Now you have sucessfully hooked PCSX2 with WGH. Now, onto the settings.

#### Intensity:
How much will the program corrupt. Always set it at 25-400 (Unless if its food court,then do 100-1000)

#### Starting Adress:
This part is important, this will dictate at what adress will the corruption start at. Always set it at around 122675849

#### Blast Range:
Always have this on,or otherwise you may risk corrupting the RAM, which may result in crashing/softlocks. Set it around 75401996

##### Corruption engine settings:
Corruption engines are the main ''corruptors'' of the game. In WGH, there are 2 engines.

#### Nightmare Engine:
RANDOM:Changes or replaces values 

#### RANDOMTILT:
Tilts a value by a random increment TILT:Tilts a value based on intensity

#### Pros:
Corrupts textures (can sometimes create confetti if you spam it alot)
Corrupts polygons
Causes audio problems
Can create very interesting results

#### Cons:
Can crash often
May create crazy flashing color polygons (which have a seizure on your screen)
Generally a great risk.

#### Vector Engine:
Corrupts 32-bit floats by changing values. You can change what kind of floats it corrupts.
**Note: Always use Big Endian**

#### Pros:
Polygon glitches
Corrupts the HUD
Can make the audio sound strange or just plain stupid (Pitch change ,incorrect sounds etc)
Sometimes corrupts textures and/or models 

#### Cons:
Instead of using Blast,use Blast until Effect
Will crash if spammed with a high intensity value.

Now you are ready to corrupt PaRappa the Rapper 2 (PAL). Have fun. Or don't, I don't really care.

If you have any problems, ask the Discord. [https://discord.gg/NgA47V9](https://discord.gg/NgA47V9)
