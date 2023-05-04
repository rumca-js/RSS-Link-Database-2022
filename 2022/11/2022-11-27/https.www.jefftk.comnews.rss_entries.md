# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Mastodon's Dubious Crawler Exemption
 - [https://www.jefftk.com/p/mastodons-dubious-crawler-exemption](https://www.jefftk.com/p/mastodons-dubious-crawler-exemption)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2022-11-27 08:00:00+00:00

<p><span>

When you share a link on social media the platform fetches the page
and includes a preview with your post:

</span>

<p>

<a href="https://www.jefftk.com/link-preview-bot-when-allowed-big.png"><img class="mobile-fullwidth" height="516" src="https://www.jefftk.com/link-preview-bot-when-allowed.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

Even though this happens automatically the system doesn't obey the
robots.txt exclusion rules (<a href="https://www.rfc-editor.org/rfc/rfc9309.html">RFC 3909</a>): I have
<code>/test/no-robots</code> excluded in my <a href="https://www.jefftk.com/robots.txt">robots.txt</a> but that doesn't stop it:

</p>

<p>

<a href="https://www.jefftk.com/link-preview-bots-ignore-robots-txt-big.png"><img class="mobile-fullwidth" height="515" src="https://www.jefftk.com/link-preview-bots-ignore-robots-txt.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

I don't even see a request for <code>robots.txt</code> in my logs.
But that's actually ok!  The robots exclusion standard is for
"crawlers", or automated agents.  When I share a link I want the
preview to be included, and so the bot fetching the page is acting as
my agent.  This is the same reason why it's fine that <a href="https://www.webpagetest.org/">WebPageTest</a> and <a href="https://pagespeed.web.dev/">PageSpeed Insights</a> also ignore
<code>robots.txt</code>: they're fetching specific pages at the user
s request so they can measure performance.

</p>

<p>

This puts Mastodon in an awkward situation.  They do want to include
previews, because they're trying to do all the standard social network
things, and if they respected <code>robots.txt</code> many sites
you'd want to be able to preview won't work.  They also <a href="https://github.com/mastodon/mastodon/issues/4486">don't want</a>
the originating instance to generate the preview and include it in the
post, because it's open to abuse:

</p>

<p>

<a href="https://www.jefftk.com/abusing-link-previews-big.png"><img class="mobile-fullwidth" height="230" src="https://www.jefftk.com/abusing-link-previews.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

You can trust <code>mastodon.mit.edu</code> about what
<code>@jefftk@mastodon.mit.edu</code> says, but not about what
<code>newyorktimes.com</code> says.

</p>

<p>

The approach Mastodon has gone with is to have each instance generate
link previews for each incoming link.  This means that while having a
link shared on Twitter or Facebook might give you one automated
pageview for the preview, on Mastodon it gives you one for each
instance the link is federated to.  For a link shared by a
widely-followed account this might mean thousands of link-preview
requests hitting a server, and I'd also now consider this traffic to
be from an automated agent.

</p>

<p>

I'm not sure what the right approach is for Mastodon.  Making the link
preview fetcher respect <code>robots.txt</code> (<a href="https://github.com/mastodon/mastodon/issues/21738">Issue
21738</a>) would be a good start. [1] Longer term I think including
link previews when composing a post and handling abuse with
defederation seems like it should work as well as the rest of
Mastodon's abuse handling.

</p>

<p>

(<a href="https://mastodon.mit.edu/@crschmidt@better.boston/109412294728438003">context</a>)

</p>

<p>
<br />

[1] Wouldn't that just add an extra request and increase the load on
sites even more?  No: everyone builds sites to make serving
<code>robots.txt</code> very cheaply.  Serving HTML, however, often
involves scripting languages, DB lookups, and other slow
operations.

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid02qSNmuy5B6mJumtcgh9h8mzFicwcHEMRBxqGFGjpT46apJsqcxuyUwVRsVLFrhETLl">facebook</a>, <a href="https://mastodon.mit.edu/@jefftk/109416209502343043">mastodon</a></i></p>

