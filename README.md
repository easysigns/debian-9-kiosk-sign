# debian-9-kiosk-sign
Script that automatically configures a locked-down debian 9 kiosk or digital sign single full screen browser application from minimal iso with chrome (or chromium), unattended updates, sshd and fail2ban 

## Install Debian 9 minimal ISO from bootable USB drive
* Download netboot mini.iso around 40MB from Debian
* Create a bootable USB drive 
* Enter BIOS and boot from USB
* On Language Selection Screen remove USB drive 
* Set root password, create user with userName, set timezone.
* Under Software Selection uncheck all software.
* Once the installation is finished login as root
* Download and run configure script by typing...

```
wget http://go.easysigns.online/configure-kiosk-sign.sh
chmod u+x configure-kiosk-sign.sh
./configure-kiosk-sign.sh userName browserUrl { normal | left | right | inverted }
```
