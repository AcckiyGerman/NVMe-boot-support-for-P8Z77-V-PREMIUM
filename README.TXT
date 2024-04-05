# Boot from NVMe on ASUS Motherboard P8Z77-V-PREMIUM 

The NVMe boot driver was added to the BIOS using [this tutorial](https://winraid.level1techs.com/t/howto-get-full-nvme-support-for-all-systems-with-an-ami-uefi-bios/30901)

I was able to successfully install and boot the Windows 11 from the NVMe drive on my motherboard.
Many thanks to the guys from the Winraid forum.

# Files

- P8Z77-V-PREMIUM-ASUS-2104.CAP - latest official bios firmware from ASUS
- P8Z77-V-PREMIUM-ASUS-2104-NVME.CAP - same bios with NVME boot driver integrated
- Z77VPR.CAP - a copy of P8Z77-V-PREMIUM-ASUS-2104-NVME.CAP, renamed following ASUS "Renaming Rules" (where a firmware file name depends of the motherboard version)

# how to flash the bios

You cannot flash this BIOS using Asus update software, because it is unofficially modified and is not signed.

Instead, use "Bios Flashback" feature:

1. format a usb flash card with FAT32 filesystem
2. copy the Z77VPR.CAP file on the flashcard.
3. insert the flashcard into the USB port with a green frame (flashback port)
4. shutdown the PC
5. press "Bios flashback" button for 3 seconds.
6. The flashing process starts and the button starts to blink.
7. After 1-2 minutes the blinking will stop and you can power on the PC.

Now you can start the OS install and the installer should see the NVMe Disks, if you've connected any.

# License

The official support for P8Z77-V-PREMIUM Asus Motherboard has been ended, however the Bios software for the Motherboard belongs to ASUS.

# No Responsibility Disclaimer 

I share this BIOS with the hope to save time for P8Z77-V-PREMIUM Asus Motherboard owners, who need to boot from NVMe.

However I cannot guarantee it will work for you. A virus on my PC might have infected the BIOS during the repack or I may be a FSB/CIA/NSC/Nibiru agent who put a keylogger into it, or Asus may activate the CPU self-destroy programm, when the modified BIOS starts... thus I disclaim all responsibility and liability for any damage or losses arising directly or indirectly as a result of the use of this modified BIOS.