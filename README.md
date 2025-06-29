# Overview
A github repository tutorial to hide ***user-wide installed apps*** from the add/remove programs settings menu (and the control panel uninstall sub-menu). For user-wide installed apps i mean applications that don't require elevated permissions to install (like discord, spotify or roblox for example) and if you're wondering, this tutorial is for ***Windows only***, specifically Windows 10/11, i don't think it works in previus versions but who knows, well i don't.

# How to hide app
Now let's look at how to hide, for example, roblox:
  1. open regedit as user, download and execute the [open-registry.bat](https://github.com/Buldogghi/hidden-user-apps/blob/main/open-regedit.bat) script (made thanks to https://superuser.com/a/981202), and if you don't trust me just look at the file, it's really just one line
  2. go to "Computer\HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Uninstall", 
  3. export the roblox-player key as a .reg file (with right click on the item) in the desktop for example (make sure to do this step, registry tweaks are non reversible!)
  4. delete the roblox-player key from the registry
  5. voila! the app is gone from the add/remove programs list!

Also keep in mind that if the application updates it may recreate the key, i don't really know but be sure to check it after an update.

# Show the app again
To show the app again you need to have the .reg file made in step 3, and to restore it you just need to open regedit and on the top left click "File > import", that's it!
