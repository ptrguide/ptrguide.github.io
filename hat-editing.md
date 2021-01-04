## pwf2tools hat editing

[← Home](https://ptrguide.github.io)

### Programs you will need:

1. [pwf2tools.](https://github.com/pahaze/pwf2tools-cs/releases)

2. Your legally obtained PTR2 ISO.

3. UltraISO/ImgBurn/isomod. Any ISO editing/injecting program will work! I'm going to be using ImgBurn for this tutorial.

### Extracting your int 

First of all, extract your ISO using your respective choice of application. (7zip/WinRAR will work too if you don't want to use UltraISO or Windows' built in explorer.)

Then extract your int with pwf2tools by using pwf2int. (Don't extract to just your desktop, make a new folder.)

### Editing your hat

Open pwf2hat (included with pwf2tools version-12b2). It works the same as Rainbow, but is way smaller and efficient and automatically renames the TIM2s to TM1 for you!
Open your hat file(s) you want to edit from your color choice (HAT_COLOR (RED, BLUE, PINK, YELL)). it will be called r(1-4)_para_mark (Example: r4_para_mark).
You will see the hat texture. Go to File > Export. Save it wherever. When you go to the folder you extracted to, you will see a PNG with your hat. Edit it as you please with whatever photo editing application. Hats can have as many colors as you want, unlike normal textures in TM0 files. Just remember to save it when you are finished (**YOU CANNOT RENAME IT. KEEP IT THE SAME NAME AS IT WAS.**).
Then, go back to pwf2hat. Go to File > Import. Import the xml file for the hat you exported (ex: r4_para_mark_01.xml). You will see your texture there! Now go to File > Save and overwrite the tm1 file you edited (ex: r4_para_mark_01.tm1).

### Injecting into created int

Go back to pwf2int and go to the "create" tab. Use your INT's extracted folder to create it. Do NOT use the hat folder.

### Injecting into your ISO

It is HIGHLY recommended to backup your ISO!!! If you are ready, proceed.

Find the INT file you created. It HAS to be named the same thing that you extracted! For example, if you extracted stage 1, you would have to name your INT st01gm0.int. 
ImgBurn: Overwrite the file in ISODIR/DATA. Then open ImgBurn, and go to "Create image file from files/folders". In the extracted ISO directory, you should see everything such as DATA, DATAS, EXT, etc. Drag it all into the huge box in ImgBurn (Source box). Then create a destination ISO, call it whatever you want. Click the button at the bottom to create it. Click yes on any dialouges that come up.

### Results

When you start the game and go to your stage, you should see your hat! If not, try again. If you are still having trouble, go check out the PTR2 modding Discord here: [https://discord.gg/xpvVnYd](https://discord.gg/xpvVnYd)