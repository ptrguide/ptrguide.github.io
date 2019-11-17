## Edit textures of models

### Step One: Get the stuffs

#### What you need:

1. PCSX2 (https://pcsx2.net) TO EMULATE THE GAME

2. PTR2 Iso TO ACTUALLY MOD IN AND PLAY (USA or PAL or JP, it doesn't matter but I'm not giving it to you because that's I L L E G A L)

3. [Pwf2tools](http://ptrguide.github.io/pwf2tools-v9.zip)

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

(I was having problems with pwf2tools doing this so you may have to do this through the command line for now. In pwf2tools, it's basically the same thing except that everything has its own button. It's quite self-explanatory.)

To get MingW, follow [the installation instructions here.](https://mgrich.github.io/html/ptr2tools)

Now cd into your folder holding your int files.

Then do these commands:

1. Ptr2spm gtex0 (model name) (output just name this anything that doesn't have spaces)

2. Ptr2tex e TEXTURES (Output from last command) (Folder where textures will be stored in)

Now just edit the png files.  Just make sure to stay in a 16 color limit or else the game WILL NOT accept your textures.

When you're done do this command:

3. Ptr2tex inject TEXTURES (Output from earlier) (Folder with model textures)

Lastly, we're going to make our folder an int again.  So cd again from the beginning and stop once you're at the folder where the int folder is.

4. Ptr2int create [newintname.int] [Extracted int folder]

Then just insert your int file into the data folder of your iso.

Done! You did it! Now, just compress together your iso and then play!
