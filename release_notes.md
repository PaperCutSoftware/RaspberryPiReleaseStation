# Release 19.0.5  (23/May/2019)

1. Upgraded to Rasbian Strech (2019-04-08) http://downloads.raspberrypi.org/raspbian/release_notes.txt
2. Upgraded to latest version of PaperCut 19.0.5 (Build 49683)

# Release 17.3.3  (28/Sept/2017)

1. Upgrade to Rasbian Strech (2017-09-07) http://downloads.raspberrypi.org/raspbian/release_notes.txt
2. After upgrade be more agressive with clean up of downloaded archives (internal change)

# Release 17.2.4 (23/Aug/2017)

1. Upgrade to Rasbian Strech (2017-08-16) http://downloads.raspberrypi.org/raspbian/release_notes.txt
2. Very minor update to README to explain were config files are located
3. Improved display of IP addresses on startup
4. Increased image size to accomodate upgrade of Raspbian
5. Improved partition sizing code (taken from raspi-config script)


# Release 17.0.2 (7/Mar/2017)

1. Versions build using PaperCut 17.x and above now have better support for on screen keyboards
2. PaperCut supplied image now based on Raspbian 2017-03-02, plus any updates
3. Fixed a bug when running the setup script with -f option
4. Fixed a bug that stopped wifi country setup running during config setup



# Release 16.4 (21/Feb/2017)

1. Based on Jan/2017 release of Raspian
2. Fixed problem with help text
3. Fixed problem with boot time wifi setup
4. Added X updates -- should fix problems some people were reporting
5. Upgraded to latest version of PaperCut 16.4 (Build 39159). May not work with previous versions of PaperCut.


# Release 16.4 (11/Jan/2017)

1. Add support for new versions of Raspbian
2. Fix bugs in upgrade process
3. Improve structure of script -- download the installer much earlier
4. Updated for build version 39038


# Release 16.3 (16/Nov/2016)

This version introduces a number of new security features compared to previous
versions.

1. Network Settings can be configured via /boot/machine.local file
2. VT terminal switching is disabled
3. New set-up script (`runme`)
4. Release station display identifies product as "PaperCut for Pi"
5. File system check and repair is run on every reboot
6. The admin login account is NO LONGER pi. Login using credentials pcadmin/password. Because virtual terminal switching is disabled you will need to use ssh for admin access
7. On booting checks for flag file `/boot/prompt4Locale` and prompts user to run raspi-config to set locale etc.

