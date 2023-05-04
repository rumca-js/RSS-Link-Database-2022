# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Mastodon Replies as Comments
 - [https://www.jefftk.com/p/mastodon-replies-as-comments](https://www.jefftk.com/p/mastodon-replies-as-comments)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2022-11-17 08:00:00+00:00

<p><span>

The comment section on most blogs is pretty minimal, with the real
discussion happening elsewhere, but people who come to the post later
won't see that discussion.  One of the more unusual choices I've made
with this blog is that instead of hosting comments here, I pull in and
display comments people make on social media. While this started out
as laziness (who wants to handle accounts for users?) over the years
I've come around to thinking that this is how blog comments should
normally work.

</span>

<p>

The biggest problem with this approach, though, is that it's in
tension with the goals of the social media companies.  Facebook,
Twitter, etc want to keep you on their platform, and aren't especially
interested in serving as the comment section of external blogs.  On the
other hand, this is potentially a really good fit for federated social
media, and I've now made it so that ActivityPub replies to my blog
posts will show up as comments here:

</p>

<p>

<a href="https://www.jefftk.com/mastodon-reply-comments-big.png"><img border="1" class="mobile-fullwidth" height="897" src="https://www.jefftk.com/mastodon-reply-comments.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

For a live example, here's <a href="https://www.jefftk.com/p/mastodon-linking-norms">a post
from last week</a> or you can look at the bottom of this post.

</p>

<p>

Integration was fast: if I fetch
<code>https://[server]/api/v1/statuses/[id]/context"</code> I get all
the publicly visible replies to that status that this server knows
about.  Then it's just a matter of extracting the relevant
information, threading the responses, and fitting that into my
existing comment display infrastructure (<a href="https://github.com/jeffkaufman/webscripts/blob/master/comment_requester_wsgi.py">code</a>).

</p>

<p>

This is a bit of a hack on top of Mastodon, but for blogs to
participate directly in ActivityPub, where you could subscribe and
comment over the protocol, you wouldn't have to implement most of what
Mastodon does.  That would make it much smaller, more efficient, and
more maintainable. It looks like maybe someone has made a <a href="https://wordpress.org/plugins/activitypub/">WordPress plugin</a>
for this?  Has anyone tried it?

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid0t2D1wC9pLmQkTMMJ9Mn1fHxYGkTwYq44WwrhgRnxerHy2PzH3dQDAdC5BFnHcxyFl">facebook</a>, <a href="https://lesswrong.com/posts/sE5wHZCDyzCSuwBxd">lesswrong</a>, <a href="https://mastodon.mit.edu/@jefftk/109360949195245646">mastodon</a></i></p>

