# sneaky-local-apps
A repo tutorial to hide local apps from the add/remove programs windows setting.
Also worth to mention, for local apps i mean user apps

How to hide, for example, roblox:
  1. open regedit as user -> you can use the open-registry.bat script, it's literally one line and just works (from https://superuser.com/a/981202)
  2. go to Computer\HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Uninstall
  3. export the roblox-player key as a .reg file in the desktop for example
  4. delete the roblox-player key from the registry
  5. voila! the app is gone from add/remove programs in windows
