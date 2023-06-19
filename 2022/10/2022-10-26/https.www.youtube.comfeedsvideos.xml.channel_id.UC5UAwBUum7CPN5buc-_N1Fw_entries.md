# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## MANJARO has a BIG PROBLEM
 - [https://www.youtube.com/watch?v=oVlD17OjFAc](https://www.youtube.com/watch?v=oVlD17OjFAc)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2022-10-27 00:00:00+00:00

Download Safing's Portmaster, or subscribe to the SPN, and take control of your network traffic: https://safing.io
Grab a brand new laptop or desktop running Linux:https://www.tuxedocomputers.com/en#

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
Instagram: https://www.instagram.com/nick_thelinuxexp/
Mastodon: https://mastodon.social/web/@thelinuxEXP
Pixelfed: https://pixelfed.social/TLENick

This video is distributed under the Creative Commons Share Alike license.

#manjaro #linux 

00:00 Intro
00:41 Sponsor: Monitor and secure your internet connection with Safing
01:45 How Manjaro works
03:39 Security problems
05:20 Packaging non-stable changes without talking with upstream
07:30 AUR integration and issues
09:55 Bad image, and bad decisions
12:43 What's the issue?
14:46 Sponsor: Get a device that's fully Linux compatible with Tuxedo
15:53 Support the channel

The first problem, which might seem small, is in how the company handles very basic stuff, like security certificates.

Manjaro has let their certificates expire 4 times now. It might seem like a very small issue, but it's extremely basic. Renewing certificates is extremely easy, and can be automated. Manjaro's inability to anticipate this or automate it isn't a good sign in terms of how seriously they take their security.

Manjaro also has the habit of trying to release things that aren't ready, without checking with the upstream devs first. One example is with the Asahi Linux project, where Manjaro decided that having Apple Silicon support early would be cool, and shipped a broken kernel.

https://fosstodon.org/web/@calebccff/108645930580968593

https://www.reddit.com/r/linux/comments/xtylya/manjaro_is_shipping_an_unstable_kernel_build_that/

This is what led to the "don't ship it" manifesto from various developers, and probably what led the Bottles developer to also ask distros to not repackage their software without talking to them first.

https://dont-ship.it/

https://usebottles.com/blog/an-open-letter/

Another problem that arose was the use of the AUR in Manjaro. Except the AUR doesn't really work well on Manjaro. Because the AUR assumes you're using the latest Arch software, with the latest versions Arch releases. Which Manjaro doesn't, because they hold back packages for testing. Which means that installing stuff from the AUR can seriously break your Manjaro system if you're not careful.

Manjaro's AUR helper had a bug in it, that sent thousands of requests to the AUR's servers for each Manjaro user. This resulted in an involuntary DDOS attack, short for distributed denial of service

https://www.reddit.com/r/linux/comments/q85t8n/pamac_manjaros_package_manager_gui_has_been/

https://gitlab.manjaro.org/applications/pamac/-/issues/1135

And then there are a few other issues. The project lead wanted to buy a new laptop using Manjaro funds, for about 2000€. The treasurer refused the expense, because it went against Manjaro's policy.

This led to an argument with the project lead, and surfaced other expenses that hadn't been discussed according to Manjaro's Policy, and led the treasurer to leave the company, leaving the project lead in full control of all the community funds.

https://web.archive.org/web/20200807042341/https://forum.manjaro.org/t/change-of-treasurer-for-manjaro-community-funds/154888

Then Manjaro announced that they would be shipping SoftMaker office by default instead of LibreOffice. Replacing an open source component with a proprietary one isn't really something you'd expect from a Linux distribution. 

http://web.archive.org/web/20191210181928/https://forum.manjaro.org/t/testing-update-2019-07-29-kernels-xfce-4-14-pre3-haskell/96690

Manjaro has also often been accused of not contributing to upstream, especially on the mobile front. Someone involved in the Pine64 community points out that the fact that most mobile Pine64 projects are starting to falter is due to the fact that only Manjaro is a supported distribution for the Pinephone, where before there were a myriad of community editions, and that Manjaro doesn't really contribute to supporting the hardware.

https://blog.brixit.nl/why-i-left-pine64/

