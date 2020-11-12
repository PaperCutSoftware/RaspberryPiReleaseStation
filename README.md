# PaperCut for Pi: Release Station setup script

This script (`runme`) will install and setup a PaperCut release station onto a copy of Raspian GNU/Linux.

The use of this script is optional. Papercut Provide a pre-created image for download from their website (created using this script).

http://www.papercut.com/tour/raspberry-pi/

This script is published for the curious, or people who wish to build their own PaperCut release station image.

This script works well with the Light download of Raspian from https://www.raspberrypi.org/downloads/raspbian/.
It will also work with the large Raspian download.

Once you have copied the Raspian image to your SD card
you might want to prevent the Raspberry Pi from auto-sizing the disk image to fit the whole SD card.
You can do this by mounting the SD card in your laptop or desktop workstation and editing the file `cmdline.txt`.
Remove the text `init=/usr/lib/raspi-config/init_resize.sh`

Insert the SD card into the Raspberry Pi and boot.

Login as user pi

copy the runme script to the Pi

Run the script `runme -h` to get documentation.

Run the setup script and follow the prompts.

After the SD card image has been created it can be backed up and duplicated.
    Edit the file machine.local (on `/boot`) to configure the network details and
    Edit the file pc-connection.properties to specify the Papercut server details

This script attempts to restrict users from running anything other than the Papercut release station software. To that end:

1. Virtual-Console switching, Ctrl-c, and job control are disabled when the user logs in
2. The papercut user is automatically assigned a secure, unknown password

To configure and maintain the release station you will need to ssh to the Pi. The admin account is `pcadmin` and the password is `password`. The password should be changed, and ideally, all ssh access should be based on ssh keys only.

The default regional configuration (keyboard layout, locale, wifi region, and timezone) is configured for the US west coast. You run the following commands to change this

```shell
sudo raspi-config
```

Note: To modify the hostname or wifi connection edit the file `/boot/machine.local`
