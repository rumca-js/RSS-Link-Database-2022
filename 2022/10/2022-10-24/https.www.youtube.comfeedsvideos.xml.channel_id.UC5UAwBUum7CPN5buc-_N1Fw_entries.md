# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## FIX your YOUTUBE EXPERIENCE: no ads, offline video, no algorithm, and more!
 - [https://www.youtube.com/watch?v=t_vmXq_TbQ4](https://www.youtube.com/watch?v=t_vmXq_TbQ4)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2022-10-25 00:00:00+00:00

Make sure your PHP applications stay relevant for longer: https://bit.ly/3VnYqJn
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

#youtube #fixyoutube #linux 

00:00 Intro
00:43 Sponsor: Extend the life of your PHP applications with TuxCare
01:32 Why would you want to "fix" youtube?
03:30 Alternative websites
05:54 Unofficial Youtube websites and apps
07:36 Browser Extensions
09:32 Build your own subscription feed with RSS
10:57 Combine RSS + video downloads with a script to watch on a TV
11:53 Support your creators
12:50 Final Thoughts
13:33 Sponsor: Get a device that runs Linux perfectly
14:51 Support the channel

In the free of charge department, you have Odysee and peertube. These platforms are basically like youtube, but not controlled by a big company.

Of course, their major issue is that they're not exhaustive: you're not going to find everything that's on youtube on these platforms.

Then you have paid alternatives, like nebula or floatplane. These offer high quality content, from big channels and creators, and while you have to pay to view your videos, it helps support craetors a lot more than depending on ad revenue. But these also suffer from the same problem: they don't have everything.

Another way would be to use alternative websites and applications that access youtube content, but don't belong to Google. As such, they can let you watch videos offline, remove ads, sometimes even sponsored segments, and more.

For mobile, you have applications like newpipe, Tubemaster, or Mytube, and a lot of others. They all offer a lot of things, including some youtube premium features, like letting you download videos for offline viewing, watch in picture in picture mode, better privacy, and more.

If you mostly watch youtube on your laptop or desktop, though, you're stuck with the youtube website. Some alternatives exist, but they're either super slow, don't work at all, or don't have all the videos you might want.

Next you have browser extensions. The big one will be Youtube UNHOOK. This one is meant to let you watch what you want, and just what you want. It's on chrome and firefox, and it lets you hide the "related videos" youtube displays next to the one you're watching, you can remove the comments if these annoy you or you don't want to be tempted to engage in yet another flamewar, the suggestions will also vanish, just like the homepage recommendations, the trending tab, and more.

Then there's the very famous return youtube disklibe button, if you want to see this almighty ratio for the videos you watch.

And of course, you can also just use any adblocker or tracker blocker to remove the annoying ads you don't want to see, and stay as private as can be. ANd there's something called sponsorblock, which crowdsources the time codes for sponsored segments and let you skip them automatically during video playback.

But what if you really don't want to use the youtube website? Well, you have a simpler way, a way that transcends the ages and lets you get your new videos in any client of your choice, through the magic of RSS feeds.

Every channel URL that has an ID in it is also an RSS feed, which means you can add it to any RSS client, like Feedly, or a desktop client like NewsFlash for GNOME, or THunderbird.

And if you like watching youtube videos on your TV, but don't want to use the youtube app, there's a convoluted way, but that will work nicely once it's setup.

Basically what you can do is write a script that pulls each new video from your subsciption feed that you recreated using the magic of RSS, downloads them with youtube download, and then stores them in a directory that's used by your plex server or local media center. With that script running as a cron task reglarly, you can do that in the background of your home server, and have access to all your videos when you come home, waiting for you.

https://github.com/darkenvy/youtube-dlp-subscriptions

