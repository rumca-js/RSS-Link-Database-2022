# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## How to use APPLE and iCloud apps and services on LINUX
 - [https://www.youtube.com/watch?v=oWY4D3Gkc3o](https://www.youtube.com/watch?v=oWY4D3Gkc3o)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2022-12-01 00:00:00+00:00

Get 100$ credit for your own Linux and gaming server: https://www.linode.com/linuxexperiment 
Grab a brand new laptop or desktop running Linux:https://www.tuxedocomputers.com/en#

👏 SUPPORT THE CHANNEL:
Get access to a weekly podcast, vote on the next topics I cover, and get your name in the credits:

YouTube: https://www.youtube.com/channel/UC5UAwBUum7CPN5buc-_N1Fw/join
Patreon: https://www.patreon.com/thelinuxexperiment

Or, you can donate whatever you want: https://paypal.me/thelinuxexp?locale.x=fr_FR

🏆 FOLLOW ME ELSEWHERE:
Twitter : http://twitter.com/thelinuxEXP
Instagram: https://www.instagram.com/nick_thelinuxexp/
Mastodon: https://mastodon.social/web/@thelinuxEXP
Pixelfed: https://pixelfed.social/TLENick
I'm also on ODYSEE: https://odysee.com/$/invite/@TheLinuxExperiment:e
And on PEERTUBE: https://tilvids.com/c/thelinuxexperiment_channel/videos

This video is distributed under the Creative Commons Share Alike license.

#apple #linux 

00:00 Intro
00:40 Sponsor: 100$ free credit on your Linux or gaming server
01:40 iCloud Account: email, contacts, calendars
04:27 Notes and Reminders
06:13 Photos and iCloud Drive
07:54 Apple Music
08:48 iMessage
09:41 Managing Devices, AirDrop, storage...
11:55 What's missing
13:23 Sponsor: Get a device that runs Linux perfectly
14:33 Support the channel

 To add your icloud email address to any desktop mail client on Linux, enter these parameters:

The server for receiving email is imap.mail.me.com. It uses SSL, and the port is 993.
The user is your icloud address, and for the password, you'll need to generate an app specific password.

https://support.apple.com/kb/HT204397

As per sending email, the server is smtp.mail.me.com, SSL is needed, and the port is 587. The address and password are the same that you entered for email reception.

For contacts and calendars, the parameters to enter are the following:
As the calendar address, enter https://caldav.icloud.com/ . Your user name is your icloud address, and your password is the app password you generated earlier.
Same goes for contacts, except the address to enter is https://contacts.icloud.com/.

You can access Notes and Reminders through the web portal. They only have the basic features. iWork apps, like Numbers, pages and Keynote are also all accessible.

Now for photos, the web interface is serviceable, you get your albums, a list of pictures, you can upload photos manually and have them show up on all your other devices, but you won't be able to edit them from here.

There is no auto upload app that will let you send pictures from your desktop to your icloud photo library either, you'll have to do manual uploads.

There's a command line utility called icloud photos downloader:

https://github.com/icloud-photos-downloader/icloud_photos_downloader

As per files stored in iCloud drive, this one will also only be accessible through the web interface, you can't mount it as external storage or auto sync files to a Linux desktop, which kinda sucks.

If you use Apple Music, there's a fantastic Linux desktop client, called Cider.
You can install it from flathub,or as a snap, a debian package, and an appimage, as well as from the AUR.

There is simply no way to access your imessages on Linux. No web interface, no app, no third party client. it's a closed source program and protocol, and so unless Apple decides to offer a web interface or to open the protocol, you'll have to keep using your smartphone or tablet to answer these.

## Connecting devices

What if you want to plug in a device and grab its contents on Linux, though? Well, that's supported. By default, when plugging in your iphone or ipad, it will show up as a camera device, provided you accept that access on the popup that appears on your device. It will show up with a DCIM folder.

It will be mounted as read-only, so you can't transfer files to it. 

You can do that using iFuse: https://www.hukot.net/community/en/tutorials/mount-iphone-in-debian-ubuntu-linux

KDE Connect lets you sync stuff between a phone or tablet, and a linux desktop. It should be installed by default on KDE desktops, and on GNOME, you can install the GSConnect extension. Don't forget to reboot your computer afterwards, it never worked right after install for me. 

On iOS, you can share the contents of the clipboard, send photos or videos, send regular files, use the device as a slideshow remote, run commands, or use it as a virtual touchpad. You can also send files to your iDevice, and they'll show up in the Files app, in local files, in the KDE Connect folder.

