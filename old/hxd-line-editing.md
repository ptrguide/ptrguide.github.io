## Custom Lines using Hxd

Ew. I'm not going to even format this properly since this is so ancient. [Use the ptr2besms tutorial please.](https://ptrguide.github.io/ptr2besms)

(Note:if you don't understand something I am saying, you can ping me @fishy7798 on the PTR2 discord)
You will need:
- A hex editor (presumably HxD)
- Cheat engine 
- knowledge of hex editing


                 SECTION 1: INPUTS


Lines is PTR2 will look like a mess, but each input is actually 56 hex long. (the red is one input) https://imgur.com/a/CjAIb
If you paste it into HxD, and turn the # of hex per line to 56, it will look much more organized. 
Result: https://imgur.com/a/ipFJt
The lines are much more organized if you do this, and a whole set of lines looks like this: https://imgur.com/a/UWPrr

Guide to what every part of an input is: https://imgur.com/a/T75TZ

Line location:
All dots on the line are divisible by decimal value of 24, the first dot has a value of zero the, and 2nd dot has a hex value of 24.
You can set it to a value between 24, and it will appear slightly off of the 24 mark, depending on how far away it was from 24. 

All button id values:
1- triangle
2- circle
3- X
4- square
5- L
6- R
7- shuriken

Animation Id:
The animation id is just the animation the character plays, if it's set to an invalid #, it will just do the idle animation.

Voice Value:
Voice value is the value that sets the sound that the character makes when you do that input. It ranges from 0-how many total voice lines that the set of lines uses. You can only use sounds for that set of lines. (No pull the lever or whatever in lesson 1 sadly)

2nd set of values

This is the 2nd sound and animation values. These are used for words like "the" in "toast the" they will be part of the same input and will play after.
The 0c in the top input is how long after the first sound the 2nd sound will play. This value can be anything. If there is no second sound, all the values where there would be a second sound are FF's


                                        SECTION 2: SUGGESTLINE


If you scroll down after the inputs, you will encounter the suggestline (highlighted in red): https://imgur.com/a/vUkMp
If you copy it, then paste it into HxD and set the # of hex per line to 52, it will look much more organized. 
Image of a full suggestline in HxD: https://imgur.com/a/bFwRO

The suggestline is organized in a similar way as an input.
Here is what the values mean: https://imgur.com/a/JCMkR

Who owns the line:
This value is who owns that line, it can have 3 possible values: 02 for the teacher, 04 for parappa, and 08 for boxy boy. You can experiment with this to see what effect it has.

# of inputs in the line:
This should be self explanatory, but i will explain it anyway. This value is simply how many inputs are in the line, it is required edit this if you wan't to add inputs. (more on that later)

Where the game finds the lines:
This is a 2 byte value that is simply where the game finds that line, you need to  edit this when adding inputs, too.

How long until the line begins:
This is simply a 2 byte value that says how long the game waits until the line begins. you can experiment with this to figure out how it works


How long until the line ends: 
This is simply a 2 byte value that dictates when the line ends. you can experiment with this to figure out how it works

Line length value:
this is how long the line will appear in the game. Watch out for the 00 before, as it is part of it too. This will always be a 2 byte value, just like all of the 2 byte values.

(NOTE: the suggestline will always be below the inputs)


I will be updating this when i can add some new info.
