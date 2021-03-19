
IconPlatformNano
Share
Download
Sign in
 
IconPlatformNano

v1.1
Select folder or file to see options
	Filename	
Size
Modified
	IconPlatformNano_v1_1	-	2020-12-06
	IconPlatformNano_v1_1.mst	10.8 KB	2020-12-06
	Readme v1_1.txt	4.7 KB	2020-12-06
3 items
Powered by pCloud
 
This website uses cookies to give you the best, most relevant experience. We do not use cookies to collect Personal Information. Using this website means that you agree with this.Learn more about our cookie policy.Cookie Settings
I Accept
Preview Document: "Readme v1_1.txt"
-------------------- 
Icon Platform Nano 
-------------------- 
by: Mistik (kreativist.si@gmail.com) 

Single channel setup 

Version: v1.1 
Date: 2020-12-06 

Tested and working on: 
CSI version: 1.0 (2020-12-04) 
Icon Platform Nano firmware version: 1.14 

Update history: 

1.1 
- updated .mst and default .zon file, updated example .zon and info 

-------------------- 
INFO 
-------------------- 
This will set up your Icon Platform Nano to work with CSI in single channel mode. 
The provided default .zon file contains predefined controls of the Nano, with basic MCU functionality. 

All Nano's controls are listed for your convenience, including versions with modifiers. 

After installation, you need to edit the .zon file with your custom actions. 

For ideas, you can see how I set up my own Nano in my .zon files at this URL: 
https://e.pcloud.link/publink/show?code=kZxQf7ZKJyiQKjdiGRXiVi8LySlHfhmffk7 

Use the lock button next to the fader on your Nano to prevent unwanted changes to values while the fader is reacting to values when changing tracks / FX parameters. 

-------------------- 
SETUP / INSTALLATION 
-------------------- 

v1.1 Download link: http://e.pc.cd/NWhotalK 

SET UP: 

1. INSTALL CSI 
If you haven't yet, install and set up CSI v1.0 according to the instructions. 
Refer to the CSI wiki here: https://github.com/GeoffAWaddington/reaper_csurf_integrator/wiki 

2. PLACE DEFINITION FILE 
Find the location where you installed CSI. 
Usually it is something like: C:\Users\YOURNAME\AppData\Roaming\REAPER\CSI\ 

Place the "IconPlatFormNano_v1_x.mst" file into the \CSI\Surfaces\Midi\ folder. 

This is the file that defines the control surface capabilities. 
You do not have to edit this file at all, unless you know what you are doing! 

3. PLACE TEMPLATE FILE 
Place the "IconPlatFormNano_v1_x" folder into the \CSI\Zones\ folder 
This is the template folder with a template .zon file. 

The .zon file is what you need to edit to set up the Nano how you like. But first let's finish the setup. 

4. POWER ON PLATFORM NANO 
Turn the platform nano on and start it up in the "MCP" DAW mode. 

You should see the surface under Audio\MIDI devices in reaper preferences. (in my case it was named "PlatformNano V1.14", in your case it might be different). 

Make sure the device is NOT enabled as a MIDI input or output. We will use it with CSI instead. 

5. SET UP THE SURFACE IN CSI 

In Reaper preferences, under Control/OSC/web settings, where you installed CSI, choose Control Surface Integrator and click Edit. 

In CSI, on the left side, add a page and name it whatever you like (e.g. "TCP"). In the options, choose Track control panel. 

On the right side, under surfaces, click Add Midi to add the Nano as a MIDI control surface and set it up like this 

- Name: "IconPlatformNano" or whatever you like: 

- Number of channels, number of sends and number of FX menu: 1 

- Set Midi In and Midi Out to your platform nano device (in my case it was named "PlatformNano V1.14", in your case it might be different). 

- Under Templates, choose the "IconPlatFormNano_v1_x".mst file as the Surface and "IconPlatFormNano_v1_x" as the Zone Folder. 

Click OK to add your Midi surface. 
Click OK again to confirm and close CSI. 

6. TEST 
Test if the surface is now working in reaper. 
The transport controls (play, stop) and the fader should be working. 
If they are working, congrats, you're on the right path! 

If not, please refer to forum for troubleshooting. 
https://forum.cockos.com/showthread.php?t=183143 

7. NOW EDIT THE .ZON FILE TO YOUR LIKING 

Inside my template .zon file, all of the controls/buttons are already listed for you, 
including most combinations with modifiers (Alt, Shift, Control). 

Some basic functionality is already mapped to get you started. 

To set it up to your liking, replace "NoAction" with whatever Reaper or custom action you like. 

Refer to the action reference here: 
https://github.com/GeoffAWaddington/reaper_csurf_integrator/wiki/Action-Reference 


8. OPTIONAL STEP 
For ideas on how to map your Nano, check out my "Mistik" .zon files, 
downloadable at this URL: 
https://e.pcloud.link/publink/show?code=kZxQf7ZKJyiQKjdiGRXiVi8LySlHfhmffk7 

There are some useful reaper functions that you can copy/paste from there and save yourself some time. 

9. FX zones 
You can also set up your nano to control plugin FX parameters of your favourite plugins, by creating a .zon file for each plugin 
where you map the desired parameters to the controls on the nano. 
To learn how, please refer to the wiki: https://github.com/GeoffAWaddington/reaper_csurf_integrator/wiki/FX-Zones 

10. ENJOY! 

For any questions, please post in the forum: 
https://forum.cockos.com/showthread.php?t=183143 


Cheers, 
Mistik 
Close
