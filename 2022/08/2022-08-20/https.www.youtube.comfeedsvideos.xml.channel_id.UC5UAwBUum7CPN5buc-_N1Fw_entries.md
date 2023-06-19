# Source:The Linux Experiment, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw, language:en-US

## THE GAMING ON LINUX GUIDE: How to play anything: Steam, Epic, Ubisoft, Origin, Battle.net, GoG...
 - [https://www.youtube.com/watch?v=v9tb1gTTbJE](https://www.youtube.com/watch?v=v9tb1gTTbJE)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UC5UAwBUum7CPN5buc-_N1Fw
 - date published: 2022-08-21 00:00:00+00:00

Get 100$ credit for your own Linux and gaming server: https://www.linode.com/linuxexperiment 
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

This video is distributed under the Creative Commons Share Alike license.

#linux #gaming #steam

USEFUL LINKS:
GE- PROTON: https://github.com/GloriousEggroll/proton-ge-custom
Heroic Games Launcher: https://heroicgameslauncher.com/
Lutris: https://lutris.net/
MangoHud: https://github.com/flightlessmango/MangoHud
GameMode: https://github.com/FeralInteractive/gamemode
vkBasalt: https://github.com/DadSchoorse/vkBasalt

00:00 Intro
00:56 Sponsor: 100$ free credit to start your own Gaming or Linux server
01:53 Basic Notions for Linux Gaming
03:41 Choosing a distribution and installing drivers
06:08 Steam, Proton, and custom Proton versions
10:32 Epic Games Store
12:56 Ubisoft Connect and Origin / EA
15:08 Battle.net and Blizzard Games
15:54 GoG
16:28 FSR: Same quality, better FPS
19:34 Sponsor: Get a laptop or desktop that runs Linux perfectly
20:32 Support the channel


Steam is in your software center, just install it from there. You'll want to tick the "Enable steamplay for all other titles" checkbox in the settings, Steamplay tab.

To check for compatibility, just go to protonDB.com, search for the game you want, and look at the rating.
Just by looking at user reports that have similar hardware to yours, so in general the same kind of GPU, you can get all the tweaks you might need to run the game.

If it's a launch argument,  you can just add it by right clicking a game in your library, going to Properties, and pasting that argument in the launch options line.

If it's a specific version of Proton, you can change that version in the "COmpatibiity" tab, by ticking the "force the use of a specific version" checkbox. 

To install Proton GE, you can head over to the GE Proton Github page.

There, you click on the releases box, and you can just download the version you need.
Extract it in your .steam/steam/compatibilitytools.d folder (create it if needed)

What about the Epic Games Store? Well, we have an amazing solution here as well. The best one on Linux is using an unofficial client called Heroic.

TO install Heroic, either search your software store, or, if it doesn't appear there, head over to their website to grab one of the versions they offer.

Now, let's move on to Origin, and Ubisoft connect. These other launchers are best handled through Lutris.

To get started with adding your Origin or Ubisoft games, just click the Origin, or Ubisoft icon in the sidebar, and then the small "user" icon next to it. You'll get a login window, and once you're singed in, your list of games will appear in the main window.

Click a game, and then the install button in the bottom of the app to install it.

Then there's battle.net. This one doesn't have an unofficial client, and doesn't have easy integrations like what Lutris offers, but you can still install it easily, through Lutris itself.

Just click the main menu, and then "Add Game". Click "search lutris" and then type Battle.net, and then click install, and follow the prompts.

For GoG, you can just use the Heroic Games Launcher I already mentioned. It supports using your GoG account, by clicking on the Manage Accounts button in the sidebar.

And then, there's FSR. This is a tool from AMD, but you can use it on any GPU, and it lets you render a game at a lower resolution, and upscale it to the native resolution of your display, so you're saving some GPU and CPU power, but the end result looks pretty close to the real thing. For example, you could play a Tomb Raider game, rendering it at 720p, but it would be upscaled to 1080p to mach your monitor.

With Linux, you can add FSR support to basically every game, even the ones that don't support it natively.

FOr Steam, you'll need to use GE Proton, and add this argument:

WINE_FULLSCREEN_FSR=1 %command% 

You can just add it in the game's properties, in the launch options box

For Heroic, use GE Proton, and check the "Enable FSR" box in the game's settings, in the Other tab.

On Lutris, just check the "Enable AMD FidelityFX super resolution" switch in the Runner Options.

