# raspberry-laptop-through-wifi
this is a simple way for you to connect your laptop as a screen to control your raspberry through local wifi.

##  **prerequisite:**
###  **Hardware:**
Raspberry pi

###  **Software:**
1.  raspberry pi OS image https://www.raspberrypi.com/software/
2.  raspberry pi imager https://projects.raspberrypi.org/en/projects/imager-install
3.  VNC Viewer https://www.realvnc.com/en/connect/download/viewer/

###  **Basic Steps:**
1.  write your image to your SD card dont forget before that, you have to format your SD card into FAT32
2.  put two file wpa_supplicant and ssh into boot directory, dont forget to change country ID, ID wifi, and the password
3.  load the sd card into your raspberry
4.  activate your SSH (see activating SSH section below)
5.  open VNC viewer, enter your raspberry IP, connect and input default id:"pi" pass:"raspberry"
6.  if your VNC doesnt work and only showing "cannot currently show the desktop", try to change the boot mode into desktop
7.  if changing the boot mode doestn work try to install ligthdm by using command "sudo apt-get install lightdm"

### Activating SSH
You can activate ssh through command line through putty.
1. open putty
2. input hostName/raspberry IP address, you can know this from you smartphone if you do thetering, or you can find it using software advance IP scanner
3. choose connection type SSH then open
4. login raspberry using default id:"pi" pass:"raspberry"
5. type "sudo raspi-config"
6. choose interface options
7. then enable ssh
8. also select VNC and install
9. if the VNC install doesnt work try to update the raspberry OS using command "sudo apt update"

### Useful things to know
|Component label	|  LED color	Meaning
|-----------------|--------------------
|OK/ACT           |  Green	SD-Card Activity
|PWR              |  Red	  Power
|FDX              |  Green	Full-Duplex connection
|LNK              |  Green	LNK/Activity

|Red Light Status      |Reason for Lighting
|----------------------|--------------------
|Consistent Blinking   |Low power source
|Light goes out        |“brownout” detected
|Consistently Lit      |Adequate power received

See the other reasons your green ACT light may be flashing in the table below!

|Light Pattern          |Status
|-----------------------|-------------------------------------
|Constantly Lit         |SD card connected
|Flashing Consistently  |Reading or Writing Code
|Three Flashes	Generic |failure to boot
|Four Flashes           |start*.elf not found
|Seven Flashes          |Kernal image (kernel.img) not found
|Eight Flashes          |SDRAM failure
|Nine Flashes           |Insufficient SDRAM
|Ten Flashes            |in HALT state
