## Edit textures of models

[← Home](https://ptrguide.github.io)

### Step One: Get the stuffs

#### What you need:

1. PCSX2 (https://pcsx2.net) TO EMULATE THE GAME

2. PaRappa the Rapper 2 ISO (find it yourself. You can also rip the game from its PS2 disc.)

3. [Pwf2tools](https://cdn.discordapp.com/attachments/302537923910303744/661723180909723696/pwf2tools-vX-distrib1.zip)

4. and motivation of course
 
### Step Two: Extract the int for files

[Go here and follow Steps 2 and 3.](https://ptrguide.github.io/easy-custom-files-into-int-files)
 
### Step Three: Choose your model

Go to PROPS and choose a model.

All of the models are .spm files so choose one of those.

Parappa's model is para_para.spm (A common one that's edited.  Just know that PaRappa's model in Stage 5 is called something different 
for some reason having to do with the different hair styles).

Then move your file to where all the folders of the int are stored. (Back one)
 
Step Four: Extracting the textures into a PNG file

**pwf2spm may create a blank file with no contents. You may want to get ptr2tools instead if the following fix doesn't work:**

-Go to the extracted folder containing pwf2tools

-Open the "bin" folder

-Open pwf2int.exe, pwf2tex.exe, then pwf2spm.exe

-Try it again.

To get MingW and ptr2tools, follow [the installation instructions here.](https://mgrich.github.io/html/ptr2tools)

### Using ptr2tools (command line):

cd into your folder holding your int files.

Then do these commands:

1. Ptr2spm gtex0 (model name) (output just name this anything that doesn't have spaces)

2. Ptr2tex e TEXTURES (Output from last command) (Folder where textures will be stored in)

Now just edit the png files.  Just make sure to stay in a 16 color limit or else the game WILL NOT accept your textures.

### Using pwf2tools (GUI):

1. On the main menu in pwf2tools, press "ptr2spm".

2. Complete each box it gives you. Remember to click the button beside each box to complete it!

3. Press "Convert your SPM to tex0!"

4. Close the pwf2spm window (if it doesn't automatically close).

5. On the main menu in pwf2tools, press "ptr2tex".

6. Press "Extract textures".

7. Complete each box it gives you. Remember to click the button beside each box to complete it!

8. Press "extract your tex0's textures to edit them!"

9. Close the pwf2spm window (if it doesn't automatically close).

10. Now, you may open your image editing software of choice and edit the textures.

### ptr2tools (command line, continued):

When you're done do this command:

3. Ptr2tex inject TEXTURES (Output from earlier) (Folder with model textures)

Lastly, we're going to make our folder an int again.  So cd again from the beginning and stop once you're at the folder where the int folder is.

4. Ptr2int create [newintname.int] [Extracted int folder]

### pwf2tools (GUI, continued):

11. On the main menu in pwf2tools, press "ptr2tex".

12. Press "Import Textures".

13. Complete each box it gives you. Remember to click the button beside each box to complete it!

14. Press "Inject your textures into your INT's tex0s!"

15. Close the pwf2spm window (if it doesn't automatically close).

16. On the main menu in pwf2tools, press "ptr2int".

17. Press "Create an INT"

18. Complete each box it gives you. Remember to click the button beside each box to complete it!

19. Press "Create your INT!"

### After using either method: 

Then just insert your int file into the data folder of your iso.

Done! You did it! Now, just compress together your iso and then play!
