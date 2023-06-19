# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## Should LINUX DISTROS still PACKAGE applications? The problem with UNOFFICIAL packages
 - [https://www.youtube.com/watch?v=j0IhajCNs14](https://www.youtube.com/watch?v=j0IhajCNs14)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2022-07-23 00:00:00+00:00

Try OnlyOffice, the best open source office suite for Linux: https://bit.ly/3IQRWfY

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

#linux #packages #flatpak 

00:00 Intro
00:43 Sponsor: OnlyOffice, the open source office suite with a free personal cloud
01:46 Packaging models: what are unofficial packages?
04:51 Unofficial packages: they're pretty normal on Linux
06:53 Trust Issues
08:48 Bugs and reputation issues
11:15 There are solutions
14:36 Sponsor: Get a laptop or desktop that's fully Linux compatible
15:47 Support the channel


We basically have 3 conflicting models nowadays. We have the old "distro maintained packages" model, the "unofficial flatpaks / snaps / appimages" model, and the "officially supported packages, whatever the format" model.

Unofficial packages are what has allowed so many distros to pop-up: even if you don't count the ones that piggyback on Ubuntu's or Fedora's repos, a lot of distros have their own repositories and sometimes even their own packaging systems. If unofficial packages were not a thing, these distros would basically have no software at all.

And that's one of the main issues here: who do you trust for your software? Distributions are supposed to have teams looking over each new version of each new package, and have a process in place to control the quality of the packaging, as well as its security, so even if the package is not contributed by the original developer, you can ensure that it runs well and doesn't try to do anything shady.

But with official packages, you have to trust the application's developers: do you believe that the app's developers have done a good job, and aren't trying to do anything weird to your system?

In the end, the older "distributions are the one who package apps" model was necessary, because there was simply no way an application developer could service all distros, and all their releases. 

But even if we put the trust issue aside, unofficial packages also have other problems. They're distributing an application under its original name, with its original logo, basically everything that would make a user think that it's a completely official version.

In most cases, it's not an issue. But if the packaging work is sloppy, if dependencies are just thrown in willy nilly and if the resultant app is all buggy, then it's the original developers that will suffer from it.

The end result is bug reports that end up in the application's queue, and that makes the devs waste time. They can either explore the issue, asking questions, and look into it, until they realize it's an issue with the package itself, and tell the user to report that to the distro maintainer. Or they can just say '"we don't support that distro, you're on your own".

There are a few solutions. The first one, that I think should be generalized, is some kind of system to let the user know when the app is maintained by the original developer, and when it's not.

These "official apps" could be filtered in our graphical app stores. And developers could probably also officially endorse packages on various distros so they also have their little checkmark.

And there is, of course, the simple fact that this older packaging model is no longer necessary for most applications. Flatpaks, Snaps, Appimages, they mostly work on every distro, and they allow developers to package once for every single release of every single distro, and they can distribute these packages themselves officially on various repositories, or their own if they prefer.

