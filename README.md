# Site
- checkout our official site! https://twortech.wixsite.com/pcmac

# Version Info
This build is compatible up to Big Sur Beta
- Now Compatible with macOS 11
- Please leave feedback with issues or w/o
- Comitted to Updating up to OS 11

# Latest Release Notes
- Fixed Bluetooth and Wifi Stability Issues
- Improved Preformance and Power Managements
- Can Provide Files for Display Overrides
- Additional Patches for 4K Display
- updated for Big Sur
- if using unsupported wifi card disable it in bios
- use config.plist
- FIXED SLEEP WAKE BUG
- Exact same functionality as Catalina

# What Works / Does Not
- Everything works minus headphone jack
- Some displays may be detected as 40hz (working on fix)

# Notes
- Never tested USB C over Display Output, everything else works flawlessly
- USB devices eject on sleep (not really an issue)

# POST

- run sudo pmset -a hibernatemode 0
- If no mouse, install all voodoo kexts using Kext Utility

# Description

- This esentially an ultra-simplistic version that is stable without the use of a deploy or complicated file installations and copies.
- You can easily view all the SSDT patches along with configuration files for the bootloader as they are all documented clearly in the files.
- This does include a copy of Clover, which of course I do not contribute to and am only responsible for the provided files, patches, and kext placements
- This guide provides a working setup with little knowledge of the topic and without "optimization" (because often they can break things). But, it is fully functional and preforms properly and is stable
- Make sure you are using DW1560 for wifi or else KP. If not using remove BRCM kexts from CLOVER>kexts>other.

# BIOS Setup
- Disable Secure Boot

# INSTALL (VERY IMPORTANT)
- Due to structural changes in the setup of apple's Big sur, this EFI cannot boot the installer it can only boot into a system / device that has already been created and setup.
- To do this, you need to install Big Sur to a virtual machine (lots of guides online) and then create an dmg of that system, and restore it onto your HDD using the 'dd' command
- There are various guides online how to get this virtual machine setup complete.
- You can then use the attached EFI folder to boot and use macOS big Sur
- You can use this video to show you how to get your macOS pre-installed onto your hard drive https://www.youtube.com/watch?v=HMU3nhcbWHw
 
 # Boot Entry Setup
 - Due to the fact this BIOS is locked down pretty heavily, reccomended to use Windows to find a free tool to add UEFI boot entries
 
  # Messages and Facetime
 - Gnerate your own Serials, Board Numbers, MLB
 - There are various guides online to do this and as default they're set to essentially Null (Fakeserial)
 - This is fairly straightforward and there is lots of external recourses, or you can contact me for support.
 
 # Headphones and Audio
 - All audio from speakers should work perfectly along with Bluetooth and USB audio
 
 # Finished!
 - Congratulations, there really aren't any more steps that are required. Feel free to contact me with any questions. 

# Donations 
- Send me a coffee lefkotyler@gmail.com
