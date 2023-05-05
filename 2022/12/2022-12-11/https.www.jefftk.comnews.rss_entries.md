# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Wider Default Audio Player in Chrome?
 - [https://www.jefftk.com/p/wider-default-audio-player-in-chrome](https://www.jefftk.com/p/wider-default-audio-player-in-chrome)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2022-12-11 08:00:00+00:00

<p><span>

My kids like to listen to story tapes.  Most of them their great
grandmother recorded onto cassettes in the 1980s, their grandmother
digitized in the 2000s, and I reworked for the web in the 2020s.  We
usually use either a tablet or old phone to play them back, and while
the browser mostly works fine for this it's terrible for seeking:

</span>

<p>

<a href="https://www.jefftk.com/default-chrome-audio-player-portrait-big.png"><img class="mobile-fullwidth" height="1191" src="https://www.jefftk.com/default-chrome-audio-player-portrait.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

The bar is so short that it's very hard to seek accurately, especially
when a story is three hours long.

</p>

<p>

You might think that if you turned it sideways you would get a wider
bar offering more precision, but no:

</p>

<p>

<a href="https://www.jefftk.com/default-chrome-audio-player-landscape-big.png"><img class="mobile-fullwidth" height="255" src="https://www.jefftk.com/default-chrome-audio-player-landscape.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

Popping <code>width: 98%</code> on the element in devtools gives a
much more usable display:

</p>

<p>

<a href="https://www.jefftk.com/better-chrome-audio-player-portrait-big.png"><img class="mobile-fullwidth" height="1192" src="https://www.jefftk.com/better-chrome-audio-player-portrait.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

Or, in landscape,

</p>

<p>

<a href="https://www.jefftk.com/better-chrome-audio-player-landscape-big.png"><img class="mobile-fullwidth" height="254" src="https://www.jefftk.com/better-chrome-audio-player-landscape.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

I wonder if this is really a one-line change, and whether Chrome would
be interested in a patch?

</p>

<p>

Firefox is much better, in landscape:

</p>

<p>

<a href="https://www.jefftk.com/default-firefox-audio-player-landscape-big.png"><img class="mobile-fullwidth" height="248" src="https://www.jefftk.com/default-firefox-audio-player-landscape.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

Though about the same in portrait:

</p>

<p>

<a href="https://www.jefftk.com/default-firefox-audio-player-portrait-big.png"><img class="mobile-fullwidth" height="1221" src="https://www.jefftk.com/default-firefox-audio-player-portrait.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

<i>Follow-up: <a href="https://www.jefftk.com/p/zooming-the-chrome-audio-player">Zooming the Chrome Audio Player</a></i>

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid02REvckx8MaJy5UGJwVn8qKKLDPd3vVCtLnSbDAaCoKfg8Tk18LU5DRkB8t4PhYB18l">facebook</a>, <a href="https://lesswrong.com/posts/GKz7aKDwGWmoyNCbw">lesswrong</a>, <a href="https://mastodon.mit.edu/@jefftk/109498569737946397">mastodon</a></i></p>

