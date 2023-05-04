# Source:Luke Smith, URL:https://lukesmith.xyz/rss.xml, language:en-US

## Based.Cooking has become more grandma-usable.
 - [https://lukesmith.xyz/updates/based-cooking-hugo-search/](https://lukesmith.xyz/updates/based-cooking-hugo-search/)
 - RSS feed: https://lukesmith.xyz/rss.xml
 - date published: 2022-05-27 12:32:47+00:00

<p>Over the past month, I&rsquo;ve taken some off-time to tinker with
<a href="https://based.cooking">Based.Cooking</a>, the cooking site I/we made a year or so
ago as a proof of concept for a simple and unintrusive recipe website. There
have been over 250 recipes submitted, but the hobbled-together static site
generator originally used proved unable to keep up and with all the
submissions, there was a big issue of content organization.</p>
<p>There have been two big changes. Firstly, I ported the entire site to use Hugo,
which I believe I mentioned already. Hugo is just a very fast static site
generator written in Go, and I particularly liked it for the ease of tagging
articles. Originally, the only content sorting on Based.Cooking was a tagcloud
at the top of the main page and &ldquo;Related&rdquo; pages at the bottom of each page.</p>
<p>Secondly, there had been a PR a while ago to add a search filter for the
mainpage with a few lines of Javascript. I think it&rsquo;s actually a fantastic
illustration of the few actually useful times to use scripting in a webpage,
and it allows users to instantaneously to search existing recipes by title and
tag without extra page loads and with handy responsive CSS.</p>
<p>Note also that tags now can be assigned emojis (via CSS, weirdly enough). I&rsquo;m
just playing around with this. It might be visually jarring for some, so I
might change it.</p>
<p>I might make some more strides to make the site more normie-friendly, since I
see it more than a proof-of-concept. Keep in mind that the <a href="https://github.com/lukesmithxyz/based.cooking">Github repo is
here</a> if you want to add recipes
or suggest other changes. I had said earlier that I wanted to cut down on the
acceptance of new recipes for fear of crowding the main page. This is less of
an issue with the search filter, so feel free to submit whatever you think it
worthy.</p>
<p>If you cook something on the site without a photo (or at least without a <em>good</em>
one), feel free to submit that as well.</p>

