# Source:Snazzy Labs, URL:https://www.youtube.com/feeds/videos.xml?channel_id=UCO2x-p9gg9TLKneXlibGR7w, language:en-US

## 25 Mac Settings You Have to Change
 - [https://www.youtube.com/watch?v=psPgSN1bPLY](https://www.youtube.com/watch?v=psPgSN1bPLY)
 - RSS feed: https://www.youtube.com/feeds/videos.xml?channel_id=UCO2x-p9gg9TLKneXlibGR7w
 - date published: 2022-07-12 00:00:00+00:00

It's time to fix macOS' wacky default settings. With over 20 years of Mac usage, I show you how 𝕀 setup 𝕞𝕪 new Macs.

**************************************
Terminal commands (paste the entire string)
**************************************
𝗙𝗮𝘀𝘁𝗲𝗿 𝗗𝗼𝗰𝗸 𝗛𝗶𝗱𝗶𝗻𝗴: defaults write com.apple.dock autohide-delay -float 0; defaults write com.apple.dock autohide-time-modifier -int 0;killall Dock
𝗙𝗮𝘀𝘁𝗲𝗿 𝗗𝗼𝗰𝗸 𝗛𝗶𝗱𝗶𝗻𝗴 𝗨𝗻𝗱𝗼: defaults write com.apple.dock autohide-delay -float 0.5; defaults write com.apple.dock autohide-time-modifier -int 0.5 ;killall Dock

𝗔𝗱𝗱 𝗗𝗼𝗰𝗸 𝗦𝗽𝗮𝗰𝗲𝗿 (paste for each spacer): defaults write com.apple.dock persistent-apps -array-add '{tile-data={}; tile-type="spacer-tile";}' && killall Dock
𝗔𝗱𝗱 𝗛𝗮𝗹𝗳-𝗛𝗲𝗶𝗴𝗵𝘁 𝗗𝗼𝗰𝗸 𝗦𝗽𝗮𝗰𝗲𝗿 (paste for each): defaults write com.apple.dock persistent-apps -array-add '{"tile-type"="small-spacer-tile";}' && killall Dock

𝗗𝗶𝘀𝗮𝗯𝗹𝗲 𝗔𝗻𝗻𝗼𝘆𝗶𝗻𝗴 𝗗𝗶𝘀𝗸 𝗪𝗮𝗿𝗻𝗶𝗻𝗴 (must restart Mac to take effect): sudo defaults write /Library/Preferences/SystemConfiguration/com.apple.DiskArbitration.diskarbitrationd.plist DADisableEjectNotification -bool YES && sudo pkill diskarbitrationd
𝗥𝗲-𝗘𝗻𝗮𝗯𝗹𝗲 𝗔𝗻𝗻𝗼𝘆𝗶𝗻𝗴 𝗗𝗶𝘀𝗸 𝗪𝗮𝗿𝗻𝗶𝗻𝗴: sudo defaults delete /Library/Preferences/SystemConfiguration/com.apple.DiskArbitration.diskarbitrationd.plist DADisableEjectNotification && sudo pkill diskarbitrationd
𝗔𝗹𝘁𝗲𝗿𝗻𝗮𝘁𝗲𝗹𝘆, 𝗱𝗼𝘄𝗻𝗹𝗼𝗮𝗱 𝗘𝗷𝗲𝗰𝘁𝗶𝗳𝘆: https://ejectify.app

𝗖𝗵𝗮𝗻𝗴𝗲 𝗦𝗰𝗿𝗲𝗲𝗻𝘀𝗵𝗼𝘁 𝗗𝗲𝗳𝗮𝘂𝗹𝘁 𝘁𝗼 𝗝𝗣𝗚 (replace with png to undo): defaults write com.apple.screencapture type jpg

𝗠𝗮𝗸𝗲 𝗛𝗶𝗱𝗱𝗲𝗻 𝗔𝗽𝗽𝘀 𝗧𝗿𝗮𝗻𝘀𝗽𝗮𝗿𝗲𝗻𝘁: defaults write com.apple.Dock showhidden -bool TRUE && killall Dock

**************************************
Follow me on Twitter - http://twitter.com/snazzyq
Follow me on Instagram - http://instagram.com/snazzyq
**************************************

00:00 - General Anger
00:30 - Spelling Correction Hate
01:25 - Fix Share Sheet
2:00 - Make Siri Tolerable
3:15 - Your Dock is An Abomination
5:48 - Bonus: System Preferences in Dock
6:10 - Spicy Corners
07:18 - A-B-Cystem Preferences (I'm Sorry)
8:08 - Oodles of Finder Tips (and a God-Tier AirDrop Tip)
14:03 - TERMINAL TIME!
14:42 - Dock Hide Delay and Transition Speed
16:14 - Dock Spacers
16:51 - Don't Let Your Mac Boss You Around!
18:40 - Stop Substantial Screenshots
19:52 - Hide Ur Pecker

