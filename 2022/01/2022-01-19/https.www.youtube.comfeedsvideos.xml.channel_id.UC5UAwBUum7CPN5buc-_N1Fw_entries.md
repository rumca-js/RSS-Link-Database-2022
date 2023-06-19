# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## FLATPAK is the FUTURE of LINUX application distribution
 - [https://www.youtube.com/watch?v=zs9QpPKDw74](https://www.youtube.com/watch?v=zs9QpPKDw74)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2022-01-19 00:00:00+00:00

Get 100$ credit for your own Linux server: https://www.linode.com/linuxexperiment 

Get your Linux desktop or laptop here: https://slimbook.es/en/

👏 SUPPORT THE CHANNEL:
Get access to an exclusive weekly podcast, vote on the next topics I cover, and get your name in the credits:

YOUTUBE: https://www.youtube.com/channel/UC5UAwBUum7CPN5buc-_N1Fw/join

Patreon: https://www.patreon.com/thelinuxexperiment

Or, you can donate whatever you want: https://paypal.me/thelinuxexp?locale.x=fr_FR

🏆 FOLLOW ME ELSEWHERE:
I also do a Gaming Podcast: https://www.youtube.com/channel/UCbRPZ11S1quJ4ESoj42A3ug

Join us on our new Discord server: https://discord.gg/xK7ukavWmQ

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
00:36 Sponsor: Get 100$ off your own Linux server
01:48 Why older packages don't work anymore
05:55 How is Flatpak any better?
09:47 Why not Snaps or AppImages?
11:25 Flatpak is NOT the future?
12:51 Sponsor: Get a shiny Linux device
13:15 Support the channel

The Flatpak is not the future blogpost: https://ludocode.com/blog/flatpak-is-not-the-future

Why do we need flatpak?

Well, first, there's the dependency hell. You might have recently seen one example of that through the Linus Tech Tips challenge: installing Steam removed the desktop environment entirely.
That's an extreme example, but a very recent one, and other, smaller ones happen very often. 

Second is app distribution. These good old packages need to be made for every distro, for every release, for every architecture.
Just Ubuntu alone will net you tens of packages to make, for every update.

PPA's, introduce more dependency hell, as they can contain library updates, that might break other apps that don't come from this PPA.

There's the fact that installing a package is super insecure, as the package basically has full root control when being installed, so you better trust that install source 100%

But is Flatpak really any better?

First Flatpak is universal. This means that you can install the same package on any distro that has the flatpak base installed, which is mostly everyone but Ubuntu these days. Developers package once, and distribute everywhere.

Second, Flatpak doesn't require root to install. Flatpak apps are sandboxed, and use portals to interact with the system, handled through permissions. These permissions are managed by the user, and they can choose to disable them.

Flatpak is also decentralized: anyone can host their own flatpak remote, which is the equivalent to a repository, and anyone can have access to flathub.

Flatpak also integrates with your desktop and app store. You can install apps directly from GNOME Software, Discover, Pamac, the APpCenter, and more. You can then manage them from here. THey'll add menu entries, work with the dock, or taskbar, they're just normal citizens.

Some people will say that Flatpak isn't space efficient, but that's not really true: flatpak ships libraries as runtimes, and these get reused by the various apps that need them.

These runtimes have also been accused of using more RAM, but they don't use more RAM than if you had loaded the corresponding libraries if they were installed as packages.

Why not other solutions?

Snap will never be a favorite for most people. It's made by Canonical. Snap also has a proprietary store backend, which annoys people, and it has clearly been designed for server and iOT first, and desktop second.

There's also appimages. These are self contained, as in each app carries all the libraries they need to run. They're portable, you can drop them in a folder somewhere and take them from distro to distro, and they'll run. Super handy.

Except that this takes a lot more space than the approach Flatpak went with, because there is no reuse of common components, and that these appimages generally look completely out of place with the rest of your system.

In the end though, what matters is what distros start shipping. And they're not turning to snap, or to appimages they're turning to flatpak, because a lot of them want an out from the old packages that put a huge burden on them in terms of time to maintain, udpate, test, upgrade and generally fix all the dependency hell.

