# hp16500c
All system files from HDD to rebuild OS for the HP16500C

you can use these files to recover an HP16500C with a failed HDD.

Buy this drive from HSC-US:	http://www.hsc-us.com
I talked to Moto:

3.5" 40-pin PATA SSD, 1GB
ADG3-CFMS01

Remove the failed rive from the bottom (the screws are accessable from the hole left after you take off the fan.)

Stick in the flash unit where the HDD was. The one listed fits perfectly. 

Copy these files to a floppy
* \system\disc\hard\system\system
* \system\disc\hard\system\system.map
* \system\disc\hard\system\sys_001
* \system\disc\hard\system\sys_004

Then boot the HP16500C from the floppy. (put in the floppy and power it up)

set the IP address to an unused address on your network.
Set the gateway to the router address.
Connect the analyser to your ethernet network.

Use filezilla to connect, (use whatever IP address you assigned, "control" as the user name, and no password.  select "settings:transfers:amximum simultaneous transfers (1).

Build the directory structure exactly as in this repository. You may not actually need all of them. I just copied everything and it worked perfectly. It is a bit tedious. Trying to copy a directory will make the '500c crash. If that happens, just power cycle it. 

move the files one directory at a time. once the files are qued in file zilla, disconnect and the transfers will start. 

I had to close and repoen filezilla after each directory of files was done being transferred. I was using 3.24.1 on windows 7. 

disconnect. power down the HP16500C, power it up with the floppy out of the drive, and it should be ready 2 go! 

I built this proceedure from pieces of all of these Excellent references: Thank you all!!!

* https://www.philpem.me.uk/elec/testgear/hp16500b/reinstall/
* http://spurtikus.de/2016/03/30/hp-16500c-logic-analyzer-information/
* http://www.ko4bb.com/doku2015/doku.php?id=test_equipment:hard_drive_conversion_to_cf_for_hp16500
* http://s5397.blogspot.com/2010/03/hp16500c-logic-analyzer-x-client.html
