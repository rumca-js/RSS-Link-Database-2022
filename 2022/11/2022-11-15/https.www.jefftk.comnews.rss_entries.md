# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Better Mastodon Aliases
 - [https://www.jefftk.com/p/better-mastodon-aliases](https://www.jefftk.com/p/better-mastodon-aliases)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2022-11-15 08:00:00+00:00

<p><span>

When I </span>

<a href="https://www.jefftk.com/p/trying-mastodon">joined Mastodon</a> I was


<code>@jefftk@schelling.pt</code>.  A few days ago that server had an
incident and I moved to 

<code><a href="https://mastodon.mit.edu">mastodon.mit.edu</a></code>, becoming


<code>@jefftk@mastodon.mit.edu</code>.  This got me thinking about a
wart in the current Mastodon design: while you can normally move
followers with you if you switch instances, this requires the
cooperation of the instance you're leaving.  In this case that
instance couldn't cooperate because its domain name had expired, but I
could also imagine someone having a falling out with their local
admins and getting kicked off in a way that precluded transfer.



<p>

Ideally this would be like email: I send and receive email as
<code>jeff@jefftk.com</code>.  The actual server I use is
<code>gmail.com</code>, but the people I interact with don't need to
know that.  If I ever want to move to a different email server I don't
need Gmail's permission and I don't need to tell my contacts; I can do
it entirely on my end.  Similarly <code>jefftk.com</code> currently
points to a Contabo VPS, but if I had an issue with them I could move
anywhere just by adjusting my domain settings.

</p>

<p>


Current Mastodon is partway there: I
can give out <code>@jeff@jefftk.com</code>, which uses a <a href="https://www.jefftk.com/.well-known/webfinger">webfinger file</a>
(thanks, <a href="https://www.facebook.com/jefftk/posts/pfbid02b41Atb2K5fkRu7a4euHz7DCAJEkgNdMsdC57PD3NrTPU45YV7AxJWE96Wn1HJbHul?comment_id=584624750086568">Chris</a>)
to redirect <code>@[anything]@jefftk.com</code> to
<code>@jefftk@mastodon.mit.edu</code>.  But then the original address
is forgotten, and it only records that they're following my
<code>mastodon.mit.edu</code> account.

</p>

<p>

One way for this to work would be that when following someone you
store both their current account name and a canonical account name.
Almost everything would use the former, but once a day in your
instance would check whether the canonical account still pointed to
the same place and adjust if necessary.

</p>

<p>

(For more discussion along these lines see Issue <a href="https://github.com/mastodon/mastodon/issues/3796#issuecomment-451274118%22">3796</a>.)

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid02T4BvzKwfye7TiHi7FrR5VdzyfY18mBwegMQamZ9SnPGbfnJRkVA9kqHHbgz64ty5l">facebook</a>, <a href="https://mastodon.mit.edu/@jefftk/109347720341123283">mastodon</a></i></p>

