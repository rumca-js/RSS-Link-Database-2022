# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## ELECTRON: why people HATE it, why devs USE it
 - [https://www.youtube.com/watch?v=G1K0Mb-rLBU](https://www.youtube.com/watch?v=G1K0Mb-rLBU)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2022-07-09 00:00:00+00:00

Download the open source best practices report here: https://meet.tuxcare.com/idc-peerscape-study
Grab a brand new laptop or desktop running Linux:https://www.tuxedocomputers.com/


👏 SUPPORT THE CHANNEL:
Get access to a weekly podcast, vote on the next topics I cover, and get your name in the credits:

YouTube: https://www.youtube.com/channel/UC5UAwBUum7CPN5buc-_N1Fw/join
Patreon: https://www.patreon.com/thelinuxexperiment

Or, you can donate whatever you want: https://paypal.me/thelinuxexp?locale.x=fr_FR

📹 MORE VIDEOS FROM ME
Linux news in Shorts format: https://www.youtube.com/channel/UCtZp0mK9IBrpS2-jNzMZmoA
Gaming on Linux: https://www.youtube.com/channel/UCaw_Lz7oifDb-PZCAcZ07kw
I'm also on ODYSEE: https://odysee.com/$/invite/@TheLinuxExperiment:e

🏆 FOLLOW ME ELSEWHERE:
Twitter : http://twitter.com/thelinuxEXP
Mastodon: https://mastodon.social/web/@thelinuxEXP
Pixelfed: https://pixelfed.social/TLENick
Discord: https://discord.gg/xK7ukavWmQ

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

#linux #electron #webdevelopment 


00:00 Intro
00:33 Get a free study on open source best practices
01:38 How electron works
02:47 Why developers like electron
06:37 System integration isn't good
10:15 Disk usage and performance
13:03 Linux needs electron
14:54 Get a laptop or desktop that runs Linux out of the box
16:00 Support the channel


Discord issues with electron: https://theevilskeleton.gitlab.io/2022/05/29/a-letter-to-discord-for-not-supporting-the-linux-desktop.html

OMGUbuntu list of electron apps: https://www.omgubuntu.co.uk/2019/02/best-electron-apps



So, what IS electron, exactly?

electron is a framework that lets developers create applications using web technologies, like javascript, HTML or CSS. It's open source, and it's cross platform, meaning that apps built with electron run on Windows, Mac and Linux.
ectly inside of the app, instead of being accessed on the internet.

So why do developers go the electron route?

Developing apps using native technologies on all platforms takes a long time, a different set of skills and knowledge for each platform, and so you need more developers, more time, and more money.

Electron lets you develop ONCE.

Second reason: debugging code for web technologies like javascript is pretty easy compared to lower level languages like C, C++, or objective C. Javascript is interpreted line by line, so noticing where the error is is way easier.


Another reason is that electron apps can auto update very easily: all you have to do is make sure that your electron app can detect when the code for your website has changed, and download the new files on your computer, a quick reload of the page, and you're up to date. 

But, electron has a bunch of issues as well. 

First, electron doesn't integrate really well with the operating system: it's just a web browser displaying a website that is stored on your computer instead of being stored on a server. This means that if electron doesn't support a specific feature of your operating system, the apps using it also won't.

A bigger problem, though, is the fact that developers often don't update the electron base, or not often enough. Electron, using CHromium, needs to be as up to date as any web browser you'd use everyday, to ensure that security flaws are patched.

That's often not the case. And it gets worse when you take into consideration operating system integration. An example is Discord on Linux. It uses an older version of electron, that doesn't support Wayland very well. electron does have wayland support, and good support at that, but Discord, by not updating the electron version they use, deprive users of that support.

And then there's the performance and resource usage. Since electron apps ship basically the whole of chromium's codebase, they aren't small. Discord, for example, once installed, weighs more than 700 MB. Almost a gigabyte. Even the most basic of Hello World applications would take about 100MB, just to display a line of text.

And there's the performance impact: chromium isn't a lighweight browser at all. Discord, again, on my system, with all its processes, uses about 480 MB. And that RAM usage is the same whether the app is minimized to the tray or fully open. GIMP, when opening a new blank document, uses 500MB.

And still, specifically for us Linux users, electron means we get applications on Linux that we wouldn't have had otherwise.

