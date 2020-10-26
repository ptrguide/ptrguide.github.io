## Model Swapping

[← Home](https://ptrguide.github.io)

Model swaps were discovered by pips, and uses the ["Inserting your content into .int files"](https://ptrguide.github.io/custom-files-into-int-files) tutorial.

### A few things to clear up:

1. Model swapping may not work all the time if you fail to do it properly.

2. This isn't swapping models, but more like replacing one with another (unless the 2 models to change are EXACTLY the same size, in which you can actually swap them).

3. If you didn't know, models are .spm files, do not attempt to replace a model with a file that isn't a .spm.

You will need:

- [QuickBMS](http://aluigi.altervista.org/papers/quickbms.zip)

- [parappa2_extract.bms](https://pastebin.com/WqSsPdBT)

- [HxD](https://mh-nexus.de/en/hxd/) or any hex editor

### Setting up:
When you have your .int extracted, the .spm files are in the last folder. (usually 6 or 7)

So you need to get the model you want to change, I'll refer to this as "Original Model"

COPY ORIGINAL MODEL AS A SEPERATE FILE, and call it something like "OriginalOriginalModel.spm", you will need it for the ["Inserting your content into .int files"](https://ptrguide.github.io/custom-files-into-int-files) tutorial.

You will need a model to replace it with (IT HAS TO HAVE THE SAME OR SMALLER SIZE AS THE MODEL YOU WANT TO CHANGE)
For this tutorial, I'll refer to this as "Replacing Model".


### Replacing Original Model:
So open up Original Model and Replacing Model in your hex editor.
You DO NOT want to change the first 5 rows of the Original Model, so copy everything beyond the 5 rows in Replacing Model.
![Gyazo Image](https://gyazo.com/75b31a6316e935959be689778ace41dc.png)

But before you copy it, you have to fill Replacing Model with zeroes until it's the EXACT SAME SIZE AS ORIGINAL MODEL. (this is one of the reasons why we need replacing model to be smaller)

So now you can copy it, goto Original Model in your hex editor, then highlight everything beyond the first 5 rows, then click the edit tab and click "Paste write", now you can save the .spm and start following Frinkeldoodles tutorial to insert the .spm into the int.

NOTES:
If you don't 100% understand what Frinkeldoodle is saying, here's some stuff to go by:
"modifiedFile.ext" is the result of replacing the model (what you just did).
"originalFile.ext" is the "OriginalOriginalModel.spm" file you saved earlier before you started.

Now you should be able to follow the ["Inserting your content into .int files"](https://ptrguide.github.io/custom-files-into-int-files) tutorial and be able to finish the mod!
