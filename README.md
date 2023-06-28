# raspberry-laptop-through-wifi

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
