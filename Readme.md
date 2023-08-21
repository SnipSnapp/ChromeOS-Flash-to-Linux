# How to Jailbreak a Chromebook for an easy Hacktop

## This will probably void your warranty, DO NOT install Windows. It won't work. 

### Enable dev mode on chrome
1. With a terminal driver, open up your chromebook and remove the screw that enables OS verification. Make sure you disconnect the battery when you do this. Reconnect it when you're done.
   https://memcpy.io/images/2017-02-27_wp_screw.jpg
2. Powerwash your chromebook
3. Press [Esc] + [Refresh key] + [Power Button]
       This will bring up an all-white menu. It may say that chrome is missing or damaged, that is fine and normal.
4. Press [CTRL] + [d]
       This will turn on Developer mode. It'll ask if you want to turn OS verification off. If it does, press 'enter'
5. Login to your chromebook.  When it starts updating immediately disconnect your wifi.  This will prevent google's updates from pushing to prevent the next part.
6. Open up a 'crosh' shell by pressing [CTRL] + [ALT] + [t]
7. type 'shell' and hit enter
8. type 'sudo bash' and hit enter
9. type 'enabled_dev_usb_boot' and hit enter
### Flash the firmware
1. run this script: "cd; curl -LO mrchromebox.tech/firmware-util.sh && sudo bash firmware-util.sh"
2. select the option to install/update UEFI Firmware
3. enter: sudo crossystem dev_boot_altfw=1
4. once complete, reboot your chromebook
5. Reboot the system with your bootable USB with your linux flavor of choice.

   
