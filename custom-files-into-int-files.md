## Inserting your content into .int files

==================================================
Inserting Custom Files Into .int Files - A Complicated (for now) Journey in Modding Parappa the Rapper 2
A Tutorial by Frinkeldoodle, with some edits made by PTR2☆TM
--------------------------------------------------

*********************************************************************
ARE YOU DOING A HAT TEXTURE EDIT?
Follow this tutorial by Chibi instead, it's simpler and should work:
[https://pastebin.com/bhfVwyuA](https://pastebin.com/bhfVwyuA)
*********************************************************************


## NOTE: If you're getting stuck following the tutorial, please send a message on the Discord.

### Files/Programs Required:
- An .int file
- quickbms.exe as well as three different scripts . . .
	- parappa2_extract.bms (my slightly edited version of parappa_rapper.bms (which was made from the creator of QuickBMS))
		Link: [https://pastebin.com/WqSsPdBT](https://pastebin.com/WqSsPdBT)
	- parappa2_compress.bms (Obtained from a post made by oddMLan in a Github thread (I hope you don't mind my usage of it! ^^"))
		Link: [https://pastebin.com/qq7XHpMv](https://pastebin.com/qq7XHpMv)
	- parappa2_decompress.bms (Basically parappa2_compress but in reverse. Kinda put together with dollar store duct tape, eheheh...)
		Link: [https://pastebin.com/sUPW8Mdb](https://pastebin.com/sUPW8Mdb)
- Hex editor (I myself use HxD Hex Editor)

### Skills Required:
- Must be comfortable doing things in a hex editor
- Must be somewhat tech-savvy, and possibly willing to look stuff up on the net if you don't understand something
- Must have a good deal of patience and some organizational skill (files can get messy pretty quickly)

==================================================
# Extracting Files from .int
--------------------------------------------------
1. Use parappa2_extract.bms with QuickBMS to extract the files from the .int. Pretty straightforward, right?
==================================================

At this point, you can start messing around with the files that were extracted. This tutorial won't cover how to edit those; I'll create tutorials in the future outlining that. I'll also list tutorials others have made doing so below:

.TIM1/.TIM2, From Tradarked on the PTR Modding Discord: https://pastebin.com/qTErdzAB

For every file you edit, keep a copy of the original file handy. 
*** From here on out, I'll refer to your modified file as "modifiedFile.ext" and the original file as "originalFile.ext". ***

==================================================
# Before Inserting File Into .int (aka The Part Where I Start To Lose You)
--------------------------------------------------
There are a few things to know before doing this. I will use "folder.dat" to refer to the compressed file you create using parappa2_compress.bms, "folder.int" to refer to the original data you're replacing inside the .int file, and "the complete .int file" to refer to the entire file. Apologies in advance if this is confusing.
1. Before folder.int starts, the complete .int file will have the hex string "11 22 33 44", then a bunch of info about the data in hex format as well as a listing of all of the files, then a bunch of empty data, and then finally eight bytes representing the compressed and uncompressed sizes of the data in little-endian format. It seems to usually be 2056 bytes long, but expect it to be far, far longer if there are a lot of files within folder.int and/or folder.int is big. (If you need an example of what this pre-folder.int data looks like, please let me know.) I'll refer to this data as the "preamble".
2. There is some empty data after folder.int. This can be added to with more empty data if your folder.dat is smaller than folder.int to keep the complete .int file the same size. I'll refer to this empty data as the "postamble".
3. folder.dat MUST be smaller or equal to the size of folder.int. The game WILL crash if you try to exceed the size of the compressed data.
==================================================

==================================================
# ACTUALLY Inserting File Into .int (aka The Part Where I /REALLY/ Lose You)
--------------------------------------------------
There are multiple ways to do this. This method is slightly more convoluted than other methods, however I've found that this method is more reliable.

## PART 1: Preparing the original data

1. Take note of the files inside the folder containing the file(s) you edited are in.
2. Find the preamble with that exact list of files inside the original complete .int file. Copy the data after the preamble and save it to a new file, not including the preamble or the postamble. (I'll call this new file originalFolder.int)
3. Decompress originalFolder.int using parappa2_decompress.bms. (I'll call the resulting file originalFolder.dat)
	3a. If originalFolder.dat turns out funky for whatever reason, try replacing line 3 in parappa2_decompress.bms with the two 
	commented lines. You'll need to give QuickBMS the size of the uncompressed folder, which you can do by right-clicking on it and
	selecting "Properties". Give the size in bytes, and I highly suggest adding a few extra hundred bytes for padding.
4. You should now have two files, originalFolder.int and originalFolder.dat.


## PART 2: Preparing the new data

1. Open your hex editor, and in it, open originalFolder.dat, originalFile.ext, and modifiedFile.ext.
2. Within the hex edtior, find the contents of originalFile.ext in originalFolder.dat. Replace that data within originalFolder.dat with the contents of modifiedFile.ext. Save this as a new file (I'll call the file you're saving here "modifiedFolder.dat")
3. Use QuickBMS and parappa2_compress.bms on modifiedFolder.dat to create a compressed version of the folder. I'll call the resulting file "modifiedFolder.int".
4. Compare the size of originalFolder.int and modifiedFolder.int. If modifiedFolder.int is larger by even a single byte, STOP. This will not work if modifiedFolder.int is larger than originalFolder.int, go back into your modified files and see what you can do to reduce the filesize somewhere. Once you've finished this, go back to step 1 in this part (Preparing the new data)
5. Open your hex editor again, and in it, open the original complete .int file, originalFolder.int, and modifiedFolder.int.
6. If modifiedFolder.int is smaller than originalFolder.int, append modifiedFolder.int with empty data at the end until it matches the size of originalFolder.int.
7. Find the contents of originalFolder.int inside the original complete .int file. Replace that data within the original complete .int file with the contents of modifiedFolder.int. Save this as a new file (I'll call this modified.int, but you should name it the same thing as the original .int file, but put it in a different location (possibly a folder for modified .int files?))
8. Use your favorite .iso editor to replace the original .int file with your modified complete .int file.
9. Test!
==================================================

If it loads properly, congrats! You managed to decipher my confusing instructions and put your own files into an .int file!
If it crashes, see where you might've gone wrong and try fixing it. Or even experiment a bit. Experimenting is how I figured out how to do this, after all :P
Note that you can use in-game saves with modified .iso files, HOWEVER I would not suggest using save states made with unmodified .isos on modified .isos.
