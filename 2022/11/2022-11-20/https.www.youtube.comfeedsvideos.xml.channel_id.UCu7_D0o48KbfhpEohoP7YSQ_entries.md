# Source:Andreas Spiess, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UCu7_D0o48KbfhpEohoP7YSQ, language:en-US

## I found an Excellent Raspberry Pi Replacement for Home Assistant / IOTstack (incl. Proxmox)
 - [https://www.youtube.com/watch?v=rXc_zGRYhLo](https://www.youtube.com/watch?v=rXc_zGRYhLo)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UCu7_D0o48KbfhpEohoP7YSQ
 - date published: 2022-11-20 08:00:18+00:00

Raspberry Pi boards are hard to get, but probably also next year. So we have to have a strategy to survive without new Raspberry boards. Sometimes, a problem can be a chance. This is what we will see today. Stay tuned if you want to get a cheaper, faster, and prettier Raspberry replacement. Spoiler alert: It will be “Back to the future.”

Links:
Fujitsu: https://ebay.us/VyIeAz
I5 Lenovo: https://ebay.us/ZtXI7G or https://amzn.to/3gj6MlH
I7 Lenovo: https://ebay.us/j0R7sl
i3 Lenovo: https://amzn.to/3Aoae5p
mSATA Adapter: https://s.click.aliexpress.com/e/_DeYJ9lz (not tried)
HA Installation: https://youtu.be/1Un4zJJWUTE
Debian installation: https://youtu.be/OUC7DMBfR3Y

Commands and links:
Debian Live
https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-11.5.0-amd64-gnome.iso
Home Assistant
https://github.com/home-assistant/operating-system/releases/download/9.3/haos_generic-x86-64-9.3.img.xz

sudo apt-get update -y
sudo apt-get install -y efibootmgr
sudo efibootmgr -c -l /EFI/BOOT/BOOTx64.EFI -L HomeAssistant
su
sudo usermod -aG sudo pi
sudo service ssh start
exit

~/PiBuilder/boot/scripts/01_setup.sh
~/PiBuilder/boot/scripts/02_setup.sh
~/PiBuilder/boot/scripts/03_setup.sh
~/PiBuilder/boot/scripts/04_setup.sh
~/PiBuilder/boot/scripts/05_setup.sh
cd ~/IOTstack
./menu.sh

lsusb
ls /dev/ttyA*
nano ~/IOTstack/docker-compose.yml

https://github.com/Paraphraser/PiBuilder
Proxmox helpers: https://tteck.github.io/Proxmox/

