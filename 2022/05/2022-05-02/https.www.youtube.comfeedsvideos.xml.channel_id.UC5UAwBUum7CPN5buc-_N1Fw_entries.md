# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## Running Android apps on Linux: It's very close, but...
 - [https://www.youtube.com/watch?v=dV7zFHIWxBU](https://www.youtube.com/watch?v=dV7zFHIWxBU)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2022-05-03 00:00:00+00:00

Download the State of Enterprise Linux Security Management Report here: https://tuxcare.org/ponemon_report

Get your Linux desktop or laptop here: https://slimbook.es/en/


👏 SUPPORT THE CHANNEL:
Get access to an exclusive weekly podcast, vote on the next topics I cover, and get your name in the credits:

YOUTUBE: https://www.youtube.com/channel/UC5UAwBUum7CPN5buc-_N1Fw/join

Patreon: https://www.patreon.com/thelinuxexperiment

Or, you can donate whatever you want: https://paypal.me/thelinuxexp?locale.x=fr_FR

You can also protect your privacy by using this extension from Startpage, each install helps the channel with a small commission: https://add.startpage.com/en/protection/?campaign=4&source=aff 

🏆 FOLLOW ME ELSEWHERE:
Linux news in Youtube Shorts format: https://www.youtube.com/channel/UCtZp0mK9IBrpS2-jNzMZmoA

Join us on our Discord server: https://discord.gg/xK7ukavWmQ

Twitter : http://twitter.com/thelinuxEXP

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

00:00 Intro
00:46 Sponsor: Get some free insight on the Security of Linux
01:49 What is Waydroid, and how to install it?
06:22 How to install applications
08:50 Add Google Apps and Services
11:25 Why run Android apps on Linux?
13:55 Sponsor: Get a Linux laptop or desktop from Slimbook
14:30 Support the channel


💡 USEFUL LINKS FOR WAYDROID
Install instructions: https://docs.waydro.id/usage/install-on-desktops
F-Droid website: https://f-droid.org/en/packages/
Aurora Store Website: https://auroraoss.com/
Script to flash Gapps: https://pythonawesome.com/script-to-add-gapps-and-other-stuff-to-waydroid/



Running Android apps on another system than Android requires a container, like what Waydroid implements. Waydroid is based on LineageOS, based on Android 10, and can access any needed hardware. It can run Android apps on x86 or ARM cpus, it's fully open source, it can add your Android apps to your menu, it can display apps in their own windows or fullscreen, it can display the Android Ui for navigation, and has near native performance.

Waydroid lets you install .APK applications, which you can download online relatively easily, but to begin with, you might want to get an app store, which will make this process a lot simpler. Let's go with F Droid, which has tons of open source applications for Android, that will also work on Waydroid.

waydroid app install and then the path to your APK file, and hit enter.

You'll then have to restart the system service for Waydroid, using 

sudo sysctemctl start waydroid-container

Your app should now be added to your applications menu, and you can open it through there. From F-Droid, you can install any application you want, and they'll also get automatically added to your applications menu. Of course, at first install, you'll need to enable installing applications from an untrusted source, like on a "real" android device.

You can also add the Google Apps and the Play Services.

I left a link to the install instructions, it's not an easy, one click install by any means, and you'll have to run multiple command lines, install a few packages on your distro, register your "fake device" with Google, clear the Play Store cache, install magisk and more. Once that's done, though, you do get a fully functional Android system, complete with Google apps, and the Google Play Store. You can login with your Google account, and use Waydroid as a full Android system.

App apps that require the Google Play Services will also work, including youtube, Google Maps, Gmail, and a lot more. You'll also be able to download apps you might already have purchased in the Play Store on an Android device, if you so choose.

I couldn't find certain apps in the Play Store, though, like Netflix for example, which might be a country-related issue. Some apps would also crash at startup, like Amazon prime Video. 

Xbox Game Pass worked, I could navigate the UI and launch a game with Xcloud, but after that, games would just not display anything, sticking to a black window, which I had to quit to resume using Waydroid. My banking app also failed with an error message telling me the service wasn't available.

Twitter worked perfectly, Duolingo also did, although in Portrait mode.

