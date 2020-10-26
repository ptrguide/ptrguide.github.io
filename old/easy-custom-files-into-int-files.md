## Inserting your content into .int files (easier)

[← Home](https://ptrguide.github.io)

Super easy tutorial.

### Steps::

1. Get [pwf2tools.](https://ptrguide.github.io/pwf2tools-v11.zip)

2. Using [7zip](https://www.7-zip.org/), [WinRAR](https://rarlab.com/download.htm), or whatever program that you use to extract compressed files (it MUST be able to extract .iso files!), extract the PTR2 .iso file.

3. Open pwf2tools, click "pwf2int", click "Extract an INT", then navigate to the "data" folder of the folder containing contents extracted from the .iso file, then select the .int file you want to edit. It **HAS** to be (x being the stage number) st0xgm0, **NOT st0xhk0** unless you're editing Boxy Boy dialog or something. ~~I really don't know why anyone would want to do that...~~ Select the folder you want to extract the contents of the .int file to, then click "Extract your INT!"

4. Now, find a tutorial for what you're trying to do and complete the steps from the point AFTER you extract the .int files in those tutorials. If you're doing a hat edit, check the [hat editing tutorial](https://ptrguide.github.io/hat-editing). **We'll have a pwf2tools version eventually.** If you're editing textures of a model, check [its tutorial.](https://ptrguide.github.io/edit-textures-of-models) 

5. Once you're done editing whatever it is you want to edit, make sure the folder with the contents of the .int file you extracted has edited files of the **same name as the old, unedited files and replace the unedited files**. Once you double-check that the file structure is the same as the fresh, unmodified folder that contains the extracted .int contents, you're ready to compress those files back into an int file. 

6. Re-open pwf2tools, press "pwf2int", then click "Create an INT". After you've clicked those two boxes, select the folder containing the contents of the .int. Make sure you select the folder that contains subfolders such as "PROPS" and the different hat folders. For example, say I extract the contents of the .int to C:/users/YOURUSERNAMEHERE/Documents/PaRappa the Rapper 2 (U)/Modding/ExtractedINTs/st01gm0, select that folder. Your game will be ruined if you select just the HAT_BLUE folder or something silly like that. 

7. Now, click the button to the RIGHT of the box in which you type the path of the new .int file itself (make sure it's Create AN INT, not Create YOUR INT!). This will open up a box asking where to save your new .int file to. Navigate to the **DATA folder** in which your extracted game contents are in (for example, I would navigate to C:/users/YOURUSERNAMEHERE/Documents/PaRappa the Rapper 2 (U)/PTR2/data), then name the .int file the same name as the original, unmodified .int is called (for example, if you're modifying stage 7, call your new .int st07gm0.int.). A dialog box will appear asking if you would like to overwrite the old file. Click "Yes". Now, you can finally click "Create your INT!".

8. Once your new .int file is ready, open your .iso editing software of choice (I'm writing this step with ImgBurn in mind), click the button saying "Create image file from files/folders", then open your extracted PTR2 ISO folder that now has your modified .int file. Now, create a new .iso in your .iso editing software using whichever "Start" button or whatever starts the .iso creation process. You should have your .iso with your modified .int file now!

9. Open the ISO in PCSX2, and BANG! Your changes should be present in-game!
