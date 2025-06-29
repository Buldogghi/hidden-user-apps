# hidden-user-apps
A repo tutorial to hide user apps (applications installed with user priviliges) from the add/remove programs settings menu (and the control panel uninstall sub-menu). It's worth mentioning that this tutorial is for **Windows only**.

Now let's look at how to hide, for example, roblox:
  1. open regedit as user -> you can use the open-registry.bat script, it's literally one line and just works (from https://superuser.com/a/981202)
  2. go to Computer\HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Uninstall
  3. export the roblox-player key as a .reg file in the desktop for example (optional but really recommended because you can't undo reg edits without a backup)
  4. delete the roblox-player key from the registry
  5. voila! the app is gone from the add/remove programs list!

Also keep in mind that if the application updates it may recreate the key, i don't really know but be sure to check the key after an update.
