step 1 : unlock bootloader
step 2 : flash TWRP
step 3 : flash Supersu


install htc mobile driver
copy Unlock_code.bin and extracted TWRPX9 file to Minimal ADB fastboot directory, ie in Program Files (x86)
copy SuperSU zip file to sd card


adb devices : check device
adb reboot download : reboot to download mode
adb reboot bootloader : reboot to bootloader mode
fastboot devices : show fastboot devices
fastboot flash unlocktoken Unlock_code.bin
fastboot flash recovery [filename.img] - flash #filename.img is TWRP
fastboot boot [filename.img] - boot # may stuck- just restart and check a recovery [boots TWRP] option in bootloader mode

#####################################################################################################################

To get Unlock_code.bin :

fastboot oem get_identifier_token # use in bootloader mode

<<<< Identifier Token Start >>>>
	Token
<<<<< Identifier Token End >>>>>

submit generated code in https://www.htcdev.com/
a mail with unlock code will receive

#Username: Book
#Password: Book
