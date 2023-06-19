# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## How to run Windows apps on Linux with Bottles
 - [https://www.youtube.com/watch?v=VqDgrHCPWG8](https://www.youtube.com/watch?v=VqDgrHCPWG8)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2022-04-10 00:00:00+00:00

Download Safing's Portmaster, or subscribe to the SPN, and take control of your network traffic: https://safing.io/portmaster

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
00:58 Sponsor: Secure your internet connection with Safing
01:53 What is WINE
04:36 Bottles: a GUI for WINE
06:07 Creating a Bottle
08:07 Automated Installers
09:14 Manual installs and configurations
12:31 Parting Thoughts
13:56 Sponsor: Get a Linux laptop or Desktop from Slimbook
14:37 Support the channel


Wine is basically an almost complete reimplementation of multiple Windows APIs in a format that Linux can understand. So you're not running a virtual machine, or emulating the system, you HAVE a whole windows environment, except it's not developed by Microsoft, and you don't need a copy of windows to use it.

Wine creates a fake C drive inside your home directory, in the .wine hidden folder, and stores everything here.

Do note that Wine does NOT protect you from viruses. Ransomware and other weird malware can still access your fake C drive, and sometimes even the regular folders in your /home directory on Linux, so don't use it to try some weird stuff you downloaded off the internet, cause it's still not safe.
 
Bottles is a graphical user interface that sits on top of Wine. It lets you handle each program in its own "Bottle", a bottle being a wine prefix, with different rules, dependencies, libraries, and settings, so each app can run optimally without risking breaking the other ones you're using. It also lets you use Proton to run games that aren't available on Steam, for example, or if you have boxed copies of various games.

The first step to install anything will be to create a bottle to run the application in. The "+" button lets you do that, and you'll get a nice graphical window to let you pick between a Gaming focused bottle, which will have a lot of tweaks specifically for running games, an Application Bottle, with improvements for running desktop apps, or a custom one that has no specific tweaks, so you can experiment yourself. Just select the appropriate Bottle type, enter its name, and click the "Create" button that appeared in the top right corner.

Once the Bottle is created, you can either straight up select an executable you'd have downloaded yourself, and run it, or you can go into more detail.

For now, Bottles only has a few installers that are mostly gaming related, but that list can expand, as anyone can contribute one of these, so I'd be surprised if we didn't see a lot of installers appearing pretty soon, especially for the most used windows apps.

These installers all have a rating, from platinum to bronze, letting you know how well the program will run, just like what you could find on protonDB. Platinum means it should run exactly as on Windows, and Bronze means it will run, but expect a few glitches here and there or some performance problems.

If your favorite program doesn't have an automatic installer script yet, you can configure your own Bottle manually. Just create a Custom Bottle, and head over the the details page.

Here, you'll find a ton of stuff you can configure or install.

Link to article about MS Office on Linux: https://ruados.github.io/articles/2021-05/office365-wine

