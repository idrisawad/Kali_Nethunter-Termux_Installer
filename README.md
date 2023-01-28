# Kali_Nethunter-Termux_Installer #

This Script will Automated install and Setup, Kali NetHunter Rootless Edition in Termux, in 4 steps, on any stock, unrooted Android device without voiding the warranty.

The Script is simply categorized by the installation steps, and  

### Prerequisite: ### 

 - Android Device (Stock unmodified device, no root or custom recovery required)
 - Termux (from f-Droid because Play Store version is outdated and not supported anymore)
 - VNC Viewer (for using Kali in Desktop mode with GUI)

### Installation: ### 

#### Install from Google PlayStore: ####

 - VNC Viewer 

Install the NetHunter-Store app from [store.nethunter.com](https://store.nethunter.com/)

#### Install from the NetHunter Store: ####

 - Termux 
 - NetHunter-KeX client
 - Hacker’s keyboard 

Note: The button “install” may not change to “installed” in the store client after installation - just ignore it. Starting termux for the first time may seem stuck while displaying “installing” on some devices - just hit enter.

### Download: ### 

 1. ```git clone https://github.com/idrisawad/Kali_Nethunter-Termux_Installer.git ```

### Install: ### 

Run these scripts:

 1. ```bash prepare.sh``` - This command makes the Install files executable

 2. ```./pre-install``` - This will install updates for Termux, Termux-Storage, wget, and Kali NetHunter Rootless Edition files from https://www.kali.org/

 3. ```./install``` - This will install Nethunter Rootles
 
 4. ```./cleanup``` - This will set up NetHunter to Autorun after openning Termux, and removes Termux motd file.

If everything worked fine, Termux has now closed. After Restart you will be in your Kali Linux, Nethunter Terminal.

You can run: ``` apt install neofetch && neofetch``` for verify the Installation was Successful

### Update after Install ###

Run ```sudo apt update && sudo apt full-upgrade -y``` first thing after installation to update Kali.
 If you have plenty of storage space available you might want to run ```sudo apt install -y kali-linux-default``` as well.

(Note: sudo paswword is default: kali/kali)

### For use Kali Linux Desktop GUI ###

 1. type ```kex start```
 2. Quit Termux, but dont close it, and open [VNC Viewer App](https://play.google.com/store/apps/details?id=com.realvnc.viewer.android&hl=de&gl=US)
 3. connect to: `127.0.0.1:5901`
 4. Enjoy!
