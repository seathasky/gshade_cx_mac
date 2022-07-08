# Gshade for Crossover Mac
Simple guide for getting Gshade installed in to your Crossover Mac games.<br>
I've added additional steps for <b>Sims 4 players</b>, please pay attention for the <img src="/gh images/the_sims2.png"></a> icon!</p>

<h3>Prerequisites:</h3>
- Latest Mac Crossover installed (download Mac CX here: https://www.codeweavers.com/)<br>
- A working Windows 64-bit executable game within Mac Crossover that uses DirectX 9 or 11. <br>
- Knowledge of working directories inside MacOS.<br>

<hr>
Support inside the <b>XIV on Mac</B> discord in #support-gshade text channel: https://xivmac.com/discord
<hr>


<br>
<img src="/gh images/newsims.png"></a> </p>

<div align="center"> <a href="https://www.youtube.com/c/Indriana-sims" </a>


[![Sims4TutroialbyIndriana](https://raw.githubusercontent.com/seathasky/gshade_cx_mac/main/gh%20images/indrianatTN.png)](https://www.youtube.com/watch?v=rs_lHlIQHqw "Video showcasing mod support on Mac")</div>

<img src="/gh images/othergames.png"></a> </p>

<hr>

<h1>Start here to setup Gshade:</h1>

Choose one of 2 Download options:<br>
1)  <b>(RECOMMENDED)</b> Download/clone this github<br>
2)  or Download "gshade_installer.sh" from https://github.com/HereInPlainSight/gshade_installer<br><br>


<img src="/gh images/first.png"></a> </p>

Type "sh" space, and drag either "manual_gshade.sh" or "gshade_installer.sh" into terminal. <br><br>

Example:<br><br>
<img src="/gh images/kik.gif"></a> </p><br>


You should now see install options in terminal after the script has loaded:
<img src="/gh images/install1.png"></a> </p>


Type "2" to Install to a custom game.<br>

<img src="/gh images/customgame.png"></a> </p>

When <b>"Install with dxgi?</b> prompt comes up,<br>

Type "Y" if your game is a DirectX 11 64-bit game <br>
or "N" if your game is a DirectX 9 64-bit game <br><img src="/gh images/the_sims2.png"></a><b> (Sims 4 players choose "N" here!)</b></p><br><br>

<hr>

If prompted what api to use, only choose dx9 or dx11.<br> <img src="/gh images/the_sims2.png"></a><b> (Sims 4 players choose DX9)</b></p>
<img src="/gh images/dx.png"></a> </p>

<hr>

Next we need to locate the WINEPREFIX where drive_c is at for your Crossover installed game and copy the directory path after the terminal prompt.<br><br>
You can easily find this by using Mac's Finder and going to ```~/Library/Application Support/Crossover/Bottles/```<br><br>
Here is an example of my Crossover bottle (Custom Wine Mac Game):
<img src="/gh images/drivec.png"></a> </p>

<hr>

Next, drag your games bottle folder directly into the terminal prompt, in my example the "Custom Wine Mac Game" bottle folder. This will complete the folder path automatically for you. You can then press enter. <br><img src="/gh images/the_sims2.png"></a><b> (Sims 4 players bottle should be called "Origin" if you installed the game with Origin launcher)</b></p>
<img src="/gh images/drivecpath.png"></a> </p>

<hr>

Next, you will be prompted to find the game's .exe. Locate your games ".exe" within the "drive_c" folder and dag that ".exe" over to the terminal prompt as so. You can now press enter again to complete Gshade install.<br>
<img src="/gh images/the_sims2.png"></a><b> (Sims 4 playes drag the "TS4_x64.exe" file, its should be inside the Sims 4 folder inside Games/Bin)</b></p>

<img src="/gh images/exe.png"></a> </p>

<hr>

<b>Next, we need to set overrides in Crossover</b><br><br>

After install, open wine configuration:</h6>
<br><br>
<p align="center"> 
<img src="https://i.imgur.com/oBp3UPL.png">
</p>

------------------------------------------------------------------------------------------------------------
<h6>Add these overrides and edit their load orders:<b5>
<br><br>

New override for library: d3dcompiler_47 - <b>edit</b> to (native)
  <p align="center"> 
<img src="/gh images/over1.png"></a> 
</p>

New override for library: d3d9 - <b>edit</b> to (native, builtin)
  <p align="center"> 
<img src="/gh images/over2.png"></a> 
</p>

New override for library: d3d11 - <b>edit</b> to (native, builtin)
  <p align="center"> 
<img src="/gh images/over3.png"></a> 
</p>

New override for library: dxgi - <b>edit</b> to (native, builtin)
  <p align="center"> 
<img src="/gh images/over4.png"></a> 
</p>


After these have been overridden, restart crossover. These need to be set prior to running game and after installing Gshade.</h6></div>

<hr>

If you followed the instructions correctly and have all the correct parameters, gshade should now load next time you run the game.<br><br>
Shift+F2 or FN+Shift+F2 on Macbook to enter gshade settings.<br><br>
Preview of Trine 3 (DX9 64-Bit game) running gshade in Crossover Mac: 

<img src="/gh images/trine2.png"></a> </p>

<img src="/gh images/the_sims2.png"></a> <b> (Sims 4 users please continue to next section below!</b></p>

<h2><img src="/gh images/the_sims2.png"></a> Sims 4 extra intructions:</h2><br></p<

Inside Crossover, make sure <b>"DXVK backend for dx11"</b> is turned OFF!<br><br>
<img src="/gh images/sims4.png"></a> </p>

<hr>

<b>Thanks to:</b><br> 
Gshade: https://gposers.com/gshade <br>
Eorn: https://github.com/HereInPlainSight/ for his Linux script<br>
Marzent: https://github.com/marzent for his PR's and making Gshade more Mac friendly<br>
Indriana: https://www.youtube.com/c/Indriana-sims for her wonderful tutorial Sims 4 setup guide.
