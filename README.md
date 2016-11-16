# PaperCut for Pi: Release Station setup script

This script (`runme`) will install and setup a PapeCut release station onto a copy of Raspian GNU/Linux.

Use of this script is optional. Papercut Provide a pre-created image for download form their website created using this script.

http://www.papercut.com/tour/raspberry-pi/

This script is published for the curious, or people who wish to build their own PaperCut release station image.

This scripts works well with the Light download of Raspian from https://www.raspberrypi.org/downloads/raspbian/.
It will also work with the large Raspian download.

Once you have copied the Raspian image to your SD card
you might want to prevent the Raspberry Pi from autosizing the disk image to fit the whole SD card.
You can do this by mounting the SD card in your laptop of desktop workstation and edting the file `cmdline.txt`.
Remove the text #TODO

Insert the SD card into the Raspberry Pi and boot.

Login as user pi

copy the runme scrip to the Pi

Run the script `runme -h` to get documentation.

Run the setup script and follow the prompts.

After the SD card image has been created it can be backed up and duplicated.
    Edit the file machine.local to configure the network details and
    Edit the file pc-connection.properties to specifiy the Papercut server details

This script attempts to restrict users from running anything other than the Papercut release station software. To that end:

1. Ctrl-c and job control are disabled when the user logs in
2. The user is automatically assigned a secure, unknown password

In order to configure and maintain the release station you will need to ssh to the Pi.
