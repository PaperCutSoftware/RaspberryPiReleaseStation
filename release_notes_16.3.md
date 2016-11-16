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

