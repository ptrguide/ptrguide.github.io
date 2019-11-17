## PTR2TOOLS Hat editing

### Programs you will need:

1. [MSYS2 MingW](https://mgrich.github.io/html/ptr2tools)

2. A PTR2 iso (get it yourself, we can't legally provide a download link.)

3. UltraISO or any other [.iso editing program](https://ptrguide.github.io/ptr2-iso-edit-tools)

4. [paint.net](https://getpaint.net), [GIMP](https://www.gimp.org/), [Photoshop](https://www.photoshop.com/), or whichever photo editing software you use

5. [Rainbow](https://www.dropbox.com/s/tzfosqzbifqieo4/rainbow_win32_bin_dev.zip?dl=1)

### MSYS part

Hi there, today I will show you how you can edit hats on PTR2.

First, you need to extract your iso files and make a seperate folder for that.

Now, in MSYS your directory should be in the data folder of your extracted iso folder.

Now, type in this: ptr2int extract [st00gm0.int] [Folder name]

### Rainbow part

Now, once that has been extracted go to the extracted int folder, now to edit your tm1/hat/mark, you will need to go to the folder your hat is currently on, for example: If your hat is Yellow, you go to HAT_YELLOW folder, now, open up Rainbow and in the File tab, select "Open", then locate the tm1 you want to edit, for example: Yellow hat's tm1s are r4_para_hat01 - Main Beanie, r4_para_hat02 - The other part of the beanie, and r4_para_mark - The Mark of parappa's hat.

And remember, 1 = red, 2 = Blue, 3 = Pink, and 4 = Yellow.

Select the tm1 you want to edit in rainbow, then you click "Export" on the file tab.

There will be 2 files, one is an xml file, and one is a png, what you wanna do is open your image editing program, drag the png to your editing program, and edit the hat. Once you're done with that, in Rainbow you're gonna click "Import" on the File tab, then you're gonna select the XML file, that is basically the png. Now, once you've done that, go to the File tab again, then click "Save", it will save as a tm2.

Now go to your explorer, locate your data folder, go to the stage you extracted, go to the Hat folder you're on, (again, example is if you're on yellow hat you select HAT_YELLOW), and delete your xml and png (you don't have to the game will ignore it), and delete your original tm1 you wanted to edit, then rename your tm2 into a tm1. And now you're set! 

### MSYS part (again)

Go back to MSYS and type in ptr2int create [intname.int] [Extracted int folder]

NOTE: Do NOT name your int the int you extracted, for example, do NOT do ptr2int create st08gm0.int 8, that will overwrite the original int.

Once you've created your int, locate it and copy it.

### .iso Editing part

Go to your ISO editing program. I have UltraISO so i'm gonna show you how to do it with UltraISO. You can also use ImgBurn, but this may be a little different if you use ImgBurn.
Locate your ISO on UltraISO, click on it, go to data, paste your int that you created, then go to your original int you edited, select rename, copy the name of the int, then delete the original int, then you go to the int you created and select rename, then paste the int name. {For example: I made an int called Stage5.int, I rename it to st05gm0.int.} After you do that, click "Save" on the File tab, and wait till it's done saving, then open up PCSX2, then located the iso you edited, and boot it up.

### Results

Go to the stage you edited, and you will see your hat has been edited! If it's a backup hat, you might wanna update PTR2Tools in MSYS.

Tut provided by luqity. 

Thanks to no and RMGRich for knowledge on this.

And thanks to rich again for updating ptr2tools.

Thanks to PTR2☆TM for rewriting portions of this tutorial.

if you need any help dm me, or join the ptr2modding server here: [https://discord.gg/xpvVnYd](https://discord.gg/xpvVnYd)

And credit to Chibi for the original method.
