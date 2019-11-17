## Advanced song swapping

### Guide originally created by TurkeyTheGobbler, with edits and formatting changes by PTR2☆TM.

TurkeyTheGobbler wrote this with UltraISO in mind. I've tried to clean it up, but that may not have worked. If you use [ImgBurn](http://ptrguide.github.io/ImgBurn-20191117T191421Z-001.zip) and need help, join the [Discord](https://discord.gg/YauNkFX) or email us at ptrhelpline@hotmail.com.

### Steps:

1. To get started your going to need three programs, [UltraISO](https://ultraiso.com) or [ImgBurn](http://ptrguide.github.io/ImgBurn-20191117T191421Z-001.zip), [Audacity](https://www.audacityteam.org/download/) and [MFAudio](https://www.zophar.net/download_file/3180). 

2. Now with all these programs at our disposal, we can get started. First, you'll need to deicide which song you'll want to swap.

3. Open your [.iso editing program](https://ptrguide.github.io/ptr2-iso-edit-tools) of choice, then open the game's .iso file.

4. Now that we have the .iso ope,n go to the folder in the ISO called "SND", then find the stage's designated .wp2 file.

4a. Here are some examples:
  
Stage 1: st01gm0g.wp2   

Stage 3: st03gm0g.wp2

Stage 7: st07gm0g.wp2   

5. For now, we are only going to edit Good song files. Make sure the last letter of the file is "g."

6. To extract the song, right click on the song you want and click "Extract To...", then choose where you want to put it. You must remember where you put it. *You will need it if you want to switch the song back to normal.* 
Alternatively, you can make a copy of the game's .iso file and use that instead rather than have to make a bazillion edits to the main .iso file.

7. Now that it is extracted, you can close your [.iso editing program](https://ptrguide.github.io/ptr2-iso-edit-tools) of choice, and open [MFAudio](https://www.zophar.net/download_file/3180).

8. **PAY A LOT OF ATENTION TO THIS:** In [MFAudio](https://www.zophar.net/download_file/3180), open the .wp2 file you extracted, now if you hit play you'll notice that the song is very staticy, and corrupt. To fix this, change the interleave in the input section to 200. Do not mess with anything else in the Input section.

9. **ALSO PAY A LOT OF ATENTION TO THIS:** Now that this is done, in the output section, change the output to "WAV- Microsoft RIFF - Uncomressed PCM". Then go ahead and click "Save As", then name it to something you'll remember and "Save as type" should be "Microsoft WAV Files (.wav)". Now, save it to where ever you like. I personally have a Parappa Modding folder. If you believe that you will make a mess, I recommend that you do the same. Click "Process!" You may now close MFAudio.

10. Now. you can open Audacity. To import the song you want to change, go to File, Import, Raw Data..., (the .wav file) 

11. In the popup that has appeared, change the sample rate to "48000"Hz (This is the sample rate Parappa music runs at). Change the Channels to Mono.

12. Now, drag the song you want into Audacity. It can be in any format. Ex: MP3, WAV

13. **This is one of the most important parts of this tutorial.** You must have the same silences in the song you choose and the original. What this means is you must match up the beginning and end silences of the song. To do this without doing too much work is by using "Generate". You can use it to create silence. 

14. To do this, highlight the area you need silence and click Generate, Silence... then click "okay" when the popup appears.. If you're having trouble with this part, look up a tutorial on "Audacity silence". The song needs to be the same length as the original, you can also use the silence tool to cover this. To get the highest quality, match the tempo with the original. (optional)

15. Now you can click "x" on the original audio to only be left with the song you choose.

16. **PAY A LOT OF ATENTION TO THIS:** To save the song you just made, click File, Export Audio, name it whatever you want, then click "Save as type", then "Other uncompressed files", then change the header to "WAV (Microsoft)"The encoding should be set to "Signed 16-bit PCM". Now you can save it and close Audacity.

17. **PAY A LOT OF ATENTION TO THIS:** Open up MFAudio again and set the input file as the song you just exported. Change the output file format to "RAW - Raw Sound Data - Uncompressed PCM". Next, change the output channels to 2 (Stereo).

18. **PAY A LOT OF ATENTION TO THIS / VERY ODD PART:** You need to click "Save As", then click cancel instead of saving. Now you can change the Interleave in the output section, which you change to 200. Now click "Save As" and change the "Save as type" to "All files (*.*)" Then, name the file st01gm0g.wp2. Replace the number 1 with whatever stage number you are editing. Now save and click "Process!"

19. Finally reopen your .iso editing program, open the .iso that you want to add your modded music to, then locate the folder. Insert your .wp2 file into the program, then move it to the SND folder, then delete the old, un-edited .wp2 file and replace it with your newly-edited .wp2 file.

20. Now, save your .iso as a new .iso file.

21. Open up PCSX2, navigate to the stage, and your changes should be there!

## Troubleshooting

If you need to read this part it either didn't work or you are willing to put the original .wp2 file back into the .iso (which you probably won't need to do since you should have made a copy of the .iso with the modded track and still have the original, unmodded .iso file.)

**The song is high-pitched, staticy, and is a total mess.** Youu need to retry the interleave parts again and double check if you missed anything.

**The game softlocks and crashes.** You didn't properly add the silences in Chapter 2.

**I want to restore the original song for some reason.** To restore the original song, open your .iso editing software, open the .iso file, then drag the original, unmodded .wp2 file into the .iso and replace the modded .wp2 with the original one. Save the .iso, and the original song should be back.

Anymore isuses? Ask the Parappa Modding Discord [here.](https://discord.gg/YauNkFX) You can alternatively email ptrhelpline@hotmail.com if you don't use Discord.

