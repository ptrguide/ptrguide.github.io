## Bad/awful song swapping

[← Home](https://ptrguide.github.io)

It is unknown who originally made this tutorial, but this is a modified version of that tutorial (thanks to PTR2☆TM#).

### Steps:
1. You will need to read BloatedC's tutorial on how to do it, because this is a modified method of it. Read the tutorial [here.](https://ptrguide.github.io/song-swapping-in-ptr2)

  1a. We expect that you have read that tutorial if you are on this step.
  
2. Open up MFaudio to the bad/awful file. Set it to 2 channels, and 400 interleave. (because it's four channels, 2 for each rank)

3. Save it as a .wav file (yes, I know, it is slow and doesn't sound right)

4. Now, put your .wav of the song you edited to fit the good rank, and save it as a .raw (uncompressed PCM) with 200 interleave and 2 channels.

5. Open the .raw file in MFAudio. 

6. **HERE'S THE IMPORTANT PART!** Even, though it's wrong, put the interleave to 200, but put the channels to ONLY ONE (mono). Now save it as a .wav as mono. 

7. Open up Audacity, and open up the bad/awful .wav you made. The top channel is bad, and the bottom is awful. Delete whatever channel your swapping with and put the mono .wav from MFaudio earlier into the channel you deleted for replacement. **MAKE SURE THE OTHER CHANNEL IS IN THE ORIGINAL SPOT! (like make sure awful is at the bottom if you're swapping bad)**

8. Now, save the .wav.

9. Open MFaudio, and insert the .wav file, and save it as a .raw as 2 channels and 400 interleave.

10. Make sure the file extension is .wp2 and not .raw.wp2 or just .raw

11. Now, put it back in the game's .iso file using your preferred [.iso editing tool.](https://ptrguide.github.io/ptr2-iso-edit-tools)

### Ta-Dah! You should have a bad/awful song swap!
