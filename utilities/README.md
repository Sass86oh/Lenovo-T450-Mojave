# Tools For Lenovo T450 Hackintosh Setup

This folder contains a number of different useful tools I find helpful with setting up the full macOS system on the Lenovo ThinkPad T450 Ultrabook. You may not find them useful but they're here for anyone to checkout and use if they want.

#

### Audio Configuration

- Contains 2 separate methods for successfully getting proper system audio functionality with with this configuration. (Credit JCSNIDER for ALC3232 Method and ACIDANTHERA for AppleALC Lilu Plugin)

#

### HD Graphics 5500

- Different monitor configurations for my personal setup. HIDPI is enabled and working very well. The clarity is very impressive, other tools for configuring proper DVMT options on systems with locked BIOS configurations.

#

### Hot Patching

- All of my current files used for HotPatching Lenovo ThinkPad T450 and a bunch of other ".dsl" files which can be used as well. 

#

### TrackPad

- Contains different TrackPad configuration options including VoodooPS2Controller, ApplePS2SmartTouchPad, a Preference Pane for extra trackpad control which works with both Voodoo and ApplePS2 setups. Also includes a way for people who have installed the Lenovo T440 TrackPad Synaptic UltraNav ClickPad to automatically remove VoodooController and associated files and replaces them with ApplePs2SmartTouchPad and it's files.

#

### Tools

- Different folders for different purposes like installing useful binaries to the /usr/local/bin folder which can be very helpful with Hackintosh computers.

#

# Command Scripts

### !clover_scripts.command

- Installs the clover startup scripts and daemons found inside of the "Tools/Library/" folder present which is part of the utilities folder. The purpose of these scripts is to ensure Clover services startup at boot when the OS loads. Also is key for the startup of the Clover Preference Pane services and update settings in system settings. Also installs the RC Scripts found in "Tools/etc/" folder.

#

### !gatekeeper.command

- Disables macOS Gatekeeper configuration. Gatekeeper is a fail safe program which is built in to macOS with the purpose of preventing the possibility of third party apps from loading up when they are executed normally by double clicking their respective icons. Instead you must right click the icon and select open from the context menu which will then allow the app to load. This script disables that and allows the normal execution of all applications no matter where they come from.

#

### !install_tools.command

- Installs binaries and other tools for hackintosh builds which can be found in the "Tools/usr/" directory and they include a number of different binary apps which can. be executed from the terminal including "patchmatic", "iasl", "lscpi", "gfxutil", "hda-verb", "plistbuddy", "mnt", "sleepwatcher", and a number of other useful tools which are beneficial in setting up a fully working system with the proper tools needed to keep things running smooth. Just execute this script and enter the password for your account and the binaries will be installed to "/usr/local/bin/" folder automatically.  

#

### !kextcache.command

- Repairs and rebuilds kextcache and system kext permissions in "/System/Library/Extensions/" and "/Library/Extensions/" folders respectively. This is helpful if you've install a kernel extension (kext) file yourself by copying and pasting the file directly in to one of these folders as it requires the proper permissions be in place for all system kexts and so this script ensures that the kexts in those folders are all properly configured with the correct permission levels and then it rebuilds the systems kextcache which will allow any new kext files to load correctly upon rebooting the system.

#

### !sleepwatcher.command

- Installs sleepwatcher commands which looks out for the systems configurations before entering sleep mode in order to make some quick changes just before it takes place which allows certain hardware to still be present and useable upon waking up the system following the sleep mode being activated automatically.

