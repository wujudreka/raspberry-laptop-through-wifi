# raspberry-laptop-through-wifi
this is a simple way for you to connect your laptop as a screen to control your raspberry through local wifi.

##  **prerequisite:**
###  **Hardware:**
Raspberry pi

###  **Software:**
1.  raspberry pi OS image https://www.raspberrypi.com/software/
2.  raspberry pi imager https://projects.raspberrypi.org/en/projects/imager-install

###  **Steps:**
1.  write your image to

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
