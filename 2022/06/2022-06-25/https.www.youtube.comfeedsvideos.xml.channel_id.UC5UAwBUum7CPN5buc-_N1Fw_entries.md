# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## I bought THIS LAPTOP: Tuxedo Stellaris 15 Gen 4 Review
 - [https://www.youtube.com/watch?v=8eRsbv-rsU8](https://www.youtube.com/watch?v=8eRsbv-rsU8)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2022-06-25 00:00:00+00:00

Grab a brand new laptop or desktop running Linux:https://www.tuxedocomputers.com/

👏 SUPPORT THE CHANNEL:
Get access to an exclusive weekly podcast, vote on the next topics I cover, and get your name in the credits:

YOUTUBE: https://www.youtube.com/channel/UC5UAwBUum7CPN5buc-_N1Fw/join

Patreon: https://www.patreon.com/thelinuxexperiment

Or, you can donate whatever you want: https://paypal.me/thelinuxexp?locale.x=fr_FR

🏆 FOLLOW ME ELSEWHERE:
Linux news in Youtube Shorts format: https://www.youtube.com/channel/UCtZp0mK9IBrpS2-jNzMZmoA

Join us on our Discord server: https://discord.gg/xK7ukavWmQ

Twitter : http://twitter.com/thelinuxEXP

Mastodon: https://mastodon.social/web/@thelinuxEXP

Pixelfed: https://pixelfed.social/TLENick

My Gaming on Linux Channel: https://www.youtube.com/channel/UCaw_Lz7oifDb-PZCAcZ07kw

📷 GEAR I USE:
Sony Alpha A6600 Mirrorless Camera: https://amzn.to/30zKyn7
Sigma 56mm Fixed Prime Lens: https://amzn.to/3aRvK5l
Logitech MX Master 3 Mouse: https://amzn.to/3BVI0Od
Bluetooth Space Grey Mac Keyboard: https://amzn.to/3jcJETZ
Logitech Brio 4K Webcam: https://amzn.to/3jgeTh9
LG Curved Ultrawide Monitor: https://amzn.to/3pcTVDH
Logitech White Speakers: https://amzn.to/3n6wSb0
Xbox Controller: https://amzn.to/3BWmIA3
*Amazon Links are affiliate codes and generate small commissions to support the channel*

This video is distributed under the Creative Commons Share Alike license.

#tuxedo #linux #laptop 

00:00 Intro
01:03 Build Quality
02:56 Display
03:58 Webcam and Mic
04:48 Keyboard and Touchpad
06:39 Speakers
07:03 I/O
08:52 Performance and Benchmarks
11:51 Battery Life
12:51 Software Experience
16:10 Why did I buy it?
17:48 Support the channel

Re-enable sound on newer intel chips: 
systemctl --user --now enable pipewire pipewire-pulse

Add the TearFree Option for screen tearing:

Edit or create this file: /etc/X11/xorg.conf.d/20-intel.conf

Add these lines:

Section "Device"
  Identifier "Intel Graphics"
  Driver "intel"
  Option "TearFree" "true"
EndSection


It's made of matte black aluminium, with the backplate being made out of plastic. It's 15.6 inches, and it's 2.6cm thick, at a total weight of 2.2kg.

The chassis is super rigid without any hint of deck flex. You can of course open up the device very easily with a few screws, and upgrade the RAM and the storage.

The display is a 1440p screen, at 2560 by 1440, with a 16:9 ratio. It's a 240hz refresh rate panel, anti-reflective, at 350 nits, and supports 95% of SRGB.

On top of the display, you get a decent webcam, a 1080p one. The microphone is decent.

On to the keyboard. It's the best keyboard I ever used on a laptop.

The touchpad is nice, if not incredible. It's smooth, and feels good for gestures, but it's a bit small for this size of laptop.

On to the speakers, and they're decent. Finally, the I/O. On the left side, you get a full size USB 3.2 Gen 2 port, a mic jack and an audio jack, plus that kensington lock. On the right, you have a full size SD card reader, and 2x USB-A 3.2 Gen1. Finally, on the back, you have a thunderbolt 4 port, an HDMI 2.1 port, a gigabit ethernet jack, and the barrel charger.

The i7 12700H is a monster. It's a 14 core, 20 threads CPU, which goes up to 4.68ghz. On Geekbench 5, it scores 1815 in single core, and 11588 in multi core. It's the most powerful CPU I own, out of all my devices, including my desktop ryzen 7 5800H.

In terms of battery life, of course, it will depend on what you do. Using only the intel graphics card, with a typical workload for me of writing on Nextcloud notes inside of Firefox, listening to music, with wifi on, bluetooth on for my mouse, headphones, and mid brightness, the laptop got up to 7h of use, thanks to the 93 Wh battery.

When using the nvidia dGPU for gaming, though, if you let it run as fast as it can, you can expect something more along the lines of 3 to 4 hours. Video editing lasted about 4 and a half hours for me.

