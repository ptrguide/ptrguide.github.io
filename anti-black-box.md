## How to Fix The Black Box in PCSX2 (when playing PaRappa the Rapper 2)

[← Home](https://ptrguide.github.io)

Are you stuck with this black box issue when playing PaRappa the Rapper 2?
![What the black box issue looks like.](https://cdn.discordapp.com/attachments/302537923910303744/655451803399487503/unknown.png)

This tutorial will explain how to remove said black box obstruction. **Note: This tutorial will NOT work for users using AMD graphics cards.**

### You Will Need

[-PCSX2 1.5.0](https://buildbot.orphis.net/pcsx2/index.php) (Make sure you download the latest build under "Revision"!)

-A copy of PTR2 (find it yourself)

[-oddMlan's Video Plugin](https://github.com/PCSX2/pcsx2/files/2898446/GSdx32-SSE4-lg.zip)

-Software to extract .zip files [7zip is good.](7zip.org)

### Steps:

Step 1. Extract the folder containing oddMlan's video plugin. 

Step 2. Navigate to the extracted folder containing oddMlan's video plugin, click on the file once, then hit CTRL+C on your keyboard.

Step 3. Navigate to your installation of PCSX2 in your computer's File Manager.

Step 4. Open the "plugins" folder, then hit CTRL+V. It should copy oddMlan's plugin into your plugins folder

Step 5. Open PCSX2. Don't open PaRappa yet.

Step 6. Press "Config" in the menu at the top, then press "Plugins/BIOS Selector".

Step 7. Press the Plugins button at the top left if are not on that menu. Once you do that, this window should appear:

![The Plugins box.](https://media.discordapp.net/attachments/645628315927052308/655454370246295593/unknown.png)

Step 8. Click the dropdown menu box beside "GS", then click on this option:

![oddMlan's video plugin](https://cdn.discordapp.com/attachments/645628315927052308/655454895163310122/unknown.png)

Step 9. Once that's selected (obviously double-check that it IS that plugin specifically!), click "Apply" in the bottom-right corner, then click "OK".

Step 10. In the PCSX2 window, click "Config" again, but this time, hover over "Video (GS)". Then, press "Plugin Settings..."

A window like this should pop up:

![Plugin Settings](https://cdn.discordapp.com/attachments/645628315927052308/655455603497631845/unknown.png)

Now, here is the important part.

### Plugin Settings

Adapter: If you have a high-end graphics card like I do (I have a nVidia GeForce GTX 1050), use your graphics card as the adapter. If you have a low-end PC, use the Intel Graphics option or the "Default Hardware Device".

![Adapter](https://cdn.discordapp.com/attachments/645628315927052308/655455917566853143/unknown.png)

Renderer: This MUST be set to OpenGL (Hardware). My other computer (desktop) doesn't even have a proper graphics card, so it wouldn't let me use any Hardware plugin. If the game doesn't load and a window pops up (forget what it says) that prevents the game from running, you unfortunately can't do this tutorial. Use the Software plugin instead if you can't run Hardware.

![Renderer](https://cdn.discordapp.com/attachments/645628315927052308/655457394523897888/unknown.png)

Interlacing: To ensure that there isn't any shaking while you play the game, I strongly recommend that you choose "Bob tff (use blend if shaking)". 

![Interlacing](https://cdn.discordapp.com/attachments/645628315927052308/655457566603739136/unknown.png)

Allow 8-Bit Textures and Large Framebuffer: These aren't really that useful, so leave them both unchecked.

![8Bit](https://cdn.discordapp.com/attachments/645628315927052308/655458111192301608/unknown.png)

Some Graphical Options: If you have a high-end PC and you want the game to look really nice, choose "3x Native" as the Internal Resolution and 4x/8x for the Anisotropic Filtering option. If you have a low/mid-end PC or you want to make the game look natural, set the Internal Resolution to Native, and turn Anisotropic Filtering off. I have the Texture Filtering option set to Bilinear (PS2). I sorta recommend setting it to that just to make sure everything goes well. Keep the Minimapping (Ins) and the CRC Hack Level options blank or turn them off (by selecting off). 

![Graphical](https://cdn.discordapp.com/attachments/645628315927052308/655458347297800212/unknown.png)

IMPORTANT STEP: In order to remove the black box / noodles themself, you MUST make sure "Enable HW Hacks" is checked/enabled. Once it's enabled, click "Configure Hacks". A window should appear with a bunch of options. YOU MUST lick the checkbox beside "Disable Depth Emulation" and make sure that box is checked. 

![HW Hacks](https://cdn.discordapp.com/attachments/645628315927052308/655460206578499597/unknown.png)

Once you've clicked that checkbox in the HW Hacks window, press OK. 

For Accurate Date, if you have a high-end PC, this may be useful. I'm not too sure what it does in this case, so let's just leave it on for now.

![Important](https://cdn.discordapp.com/attachments/645628315927052308/655459829820948521/unknown.png)

Blending Unit Accuracy: If you have a high-end PC, set this option to High (recommended high-end PC). If you run a low-end PC, set this option to Basic (Recommended low-end PC). If you use a mid-end PC, set this option to Medium.

![Blending](https://cdn.discordapp.com/attachments/645628315927052308/655460893517152296/unknown.png)

Once you've done all of this, you can click "OK".

### Steps (continued)

The black box / noodle issue should be gone. To verify that you've done this correctly, open Stage 3 (you can skip through the cutscene / Boxy Boy by holding L1 and L2 / your keys/buttons mapped to L1 and L2 at the same time when you click "Single Player" when selecting Stage 3. Hold these buttons until the Loading screen pops up. If you did this correctly, once the loading screen is gone, it should go right to the stage.). The black box should be gone and you should have no depth issues / objects covering the lines.

#### If you need help, join the [Discord](https://discord.gg/HRCMKdM) or email ptrhelpline@hotmail.com.
