## Song swapping in PTR2

Tutorial originally created by [BloatedC](https://twitter.com/BloatedC), with edits from PTR2☆TM. Some, if not all text was transferred from the original Pastebin document, but now more visually appealing and slightly easier to follow!

Notes:
-Personally I use [UltraISO](https://www.ultraiso.com/) for editing my iso files, not sure how well it works for other programs but you're welcome to try. This little guide is gonna be written with [UltraISO](https://www.ultraiso.com/) in mind. With that noted in [UltraISO](https://www.ultraiso.com/) make sure "recompile ISO when saving" is unchecked and Super Restore is enabled.
(Note from PTR2☆TM: You can also use [ImgBurn](http://imgburn.com/), but do keep in mind that the current version of [ImgBurn](http://imgburn.com/) is bundled with [OpenCandy](https://en.wikipedia.org/wiki/OpenCandy), a type of [adware](https://en.wikipedia.org/wiki/Adware).)
-Get the program [MFAudio](https://www.zophar.net/download_file/3180), it's the program I use to convert the proprietary format Parappa uses into something readable and editable.

##### Steps

1. Open the Parappa 2 iso with UltraISO and navigate to the folder called "SND".
2. Find the track you want to replace. They should have a .wp2 file extension. The numbers correspond to the stage number and the letters such as "g" and "c" correspond to the "good" and "cool" levels respectively. NOTE: the bad and awful mixes are interleaved tracks, making them a lot harder to modify. I can't help you with that as I've yet to experiment with it.
3. Extract the track you want to replace and open it in MFAudio.
4. Set the interleave to 200 and export as a .wav file.
5. Do the proper audio mixing to replace the song in your audio editor of choice (I use and recommend [Audacity](https://www.audacityteam.org/download/), it's free and functional). MAKE SURE the tempo of the new song matches the old and the silence at the beginning and end is the same as the original. If the tempo is off the song will sound terrible and the game will softlock if the silences aren't the same as the game expects them to be. THIS IS VERY IMPORTANT! [Look for the song you are swapping using this list and make sure the song you're replacing it with matches the original's BPM.](./bpmlist.md)
6. Save your finished track as a .wav file.
7. Open your new track with MFAudio, set the output as RAW Uncompressed and set the interleave to 200. DO NOT FORGET TO DO THAT, THE AUDIO WILL BE DISTORTED IF YOU DON'T! (The effect is pretty funny tho)
8. Save the track with the same file name as the track you're replacing including the .wp2 extension. Be sure the file ends in .wp2 and not .wp2.raw.
