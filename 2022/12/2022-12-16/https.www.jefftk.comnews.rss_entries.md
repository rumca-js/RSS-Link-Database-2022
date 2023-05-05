# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Introducing Shrubgrazer
 - [https://www.jefftk.com/p/introducing-shrubgrazer](https://www.jefftk.com/p/introducing-shrubgrazer)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2022-12-16 08:00:00+00:00

<p><span>

Since starting using Mastodon a month ago, a few different things
haven't been a good fit for how I like to use social media:

</span>

<p>

</p>

<ul>

<li><p>I'm relatively free with following people, but there are some
people whose posts I don't want to miss.  I'd like these to go <a href="https://www.jefftk.com/p/user-controlled-algorithmic-feeds">at the top of my feed</a>.

</p></li>
<li><p>Fediverse replies logically form a tree, but Mastodon just
shows you a list. This isn't good for reading complex branching
discussions.  When I set up replies on my blog <a href="https://www.jefftk.com/p/mastodon-replies-as-comments">as comments</a> I made them be
a tree, and I like this a lot better.

</p></li>
</ul>



<p>

I decided to write a custom client that does both of these the way I'd
prefer, and also fixes some other problems I've had with social media
historically:

</p>

<p>

</p>

<ul>

<li><p>On Facebook, it's reasonably common that you saw something but
<a href="https://www.jefftk.com/p/cleaning-a-spoon-is-complex">can't find it again</a>. In
my client there's a history page that shows you everything you've
looked at in reverse chronological order.

</p></li>
<li><p>Traditional algorithmic feeds have weights but you can't
interact with them directly. Instead you just notice that it's showing
you a lot of posts by someone you happened to have a few interactions
with, while never showing you posts by many other people.  The weights
for this feed are directly exposed in the UI, and there is a page
where you can make any changes you want.

</p></li>
<li><p>Your behavior only changes weights when you make a conscious
choice to change them.  There are various things that I will interact
with (TikTok style shorts, angry discussions) that, on reflection,
aren't how I would like to spend my time.  When interacting with an
opaque algorithm there's no way to say "I know I just spent a while
looking at that distracting flashy thing, but it isn't actually what I
want you to show me more of".

</p></li>
</ul>



<p>

If you were to visit you'd be asked to log in:

</p>

<p>

<a href="https://www.jefftk.com/screenshot-shrubgrazer-welcome-big.png"><img class="mobile-fullwidth" height="144" src="https://www.jefftk.com/screenshot-shrubgrazer-welcome.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

It won't actually let you log in because the list of allowed users is
currently just me, but let's imagine you're me.  On logging in you'd
see a feed, which is a series of posts sorted first by the weight I've
assigned to the author and then in reverse chronological order.

</p>

<p>

<a href="https://www.jefftk.com/screenshot-shrubgrazer-mobile-feed-big.png"><img class="mobile-fullwidth" height="1200" src="https://www.jefftk.com/screenshot-shrubgrazer-mobile-feed.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

If you click on a post you get a forum-style threaded view:

</p>

<p>

<a href="https://www.jefftk.com/screenshot-shrubgrazer-mobile-discussion-big.jpg"><img class="mobile-fullwidth" height="1148" src="https://www.jefftk.com/screenshot-shrubgrazer-mobile-discussion.jpg" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

It also works on desktop, where you have a bit more space:

</p>

<p>

<a href="https://www.jefftk.com/screenshot-shrubgrazer-showing-children-big.png"><img class="mobile-fullwidth" height="1038" src="https://www.jefftk.com/screenshot-shrubgrazer-showing-children.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

If you open a post that has both children and parents it shows the
parents above and then threads the children below.  This means even
when exploring a large discussion you can still see your context.

</p>

<p>

<a href="https://www.jefftk.com/screenshot-shrubgrazer-showing-post-with-children-and-parents-big.png"><img class="mobile-fullwidth" height="999" src="https://www.jefftk.com/screenshot-shrubgrazer-showing-post-with-children-and-parents.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

You can favorite posts by clicking the star.  You can also reply to
them inline by clicking the "up and then left" reply icon:

</p>

<p>

<a href="https://www.jefftk.com/screenshot-shrubgrazer-example-reply-big.png"><img class="mobile-fullwidth" height="251" src="https://www.jefftk.com/screenshot-shrubgrazer-example-reply.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

The hamburger menu in the upper left gives additional options:

</p>

<p>

<a href="https://www.jefftk.com/screenshot-shrubgrazer-hambuger-menu-big.png"><img class="mobile-fullwidth" height="305" src="https://www.jefftk.com/screenshot-shrubgrazer-hambuger-menu.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

The client has only just gotten to where it's usable, and there are
still several key features where you need to fall back to the standard
UI (notifications, following, boosting).  Still, if it's something
you'd like to play with, the client is open source (<a href="https://github.com/jeffkaufman/shrubgrazer">github</a>) and is a
python wsgi app with no dependencies. I could also temporarily add you
as a guest on my instance if you wanted to try it without running
code.

</p>

<p>

There are a lot of other things I'd like to do with this, like <a href="https://github.com/jeffkaufman/shrubgrazer/issues/2">integrating
notifications into the feed</a>, <a href="https://github.com/jeffkaufman/shrubgrazer/issues/6">threading
related posts in the feed</a>, and <a href="https://github.com/jeffkaufman/shrubgrazer/issues/8">showing
context on recent entries</a>.  You can see the <a href="https://github.com/jeffkaufman/shrubgrazer/issues?q=is%3Aopen+is%3Aissue+label%3Aenhancement">full
list</a> on GitHub, and feel free to suggest more either in a comment
or as a <a href="https://github.com/jeffkaufman/shrubgrazer/issues/new">new
issue</a>.

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid0bTcUkhT89Gh3bpwqX2n1QE76TaSSAXXSsvJzMMtpSJgt63nnp7m4iqkNagZpxFVDl">facebook</a>, <a href="https://lesswrong.com/posts/Doj5zwgdTouuTGNiA">lesswrong</a>, <a href="https://mastodon.mit.edu/@jefftk/109523900751872891">mastodon</a></i></p>

