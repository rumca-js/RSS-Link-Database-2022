# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Localhost Security Messaging
 - [https://www.jefftk.com/p/localhost-security-messaging](https://www.jefftk.com/p/localhost-security-messaging)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2022-12-31 08:00:00+00:00

<p><span>

Browsers these days either mark sites with a padlock
(</span>

<code>https://</code>) or "not secure" (

<code>http://</code>).  This
warns the users that without the protection of "

<code>https://</code>"
your communications could be read or modified by any network your
packets travel over.  But how should "

<code>http://localhost</code>"
be marked?  That's your own computer so it's secure, but the
connection isn't encrypted so a padlock would be misleading.



<p>

It turns out that the browsers have three options for the url bar, not
just secure and insecure.  Here's what they look like in Firefox:

</p>

<p>

<a href="https://www.jefftk.com/firefox-https-jefftk-big.png"><img class="mobile-fullwidth" height="32" src="https://www.jefftk.com/firefox-https-jefftk.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

<a href="https://www.jefftk.com/firefox-http-neverssl-big.png"><img class="mobile-fullwidth" height="32" src="https://www.jefftk.com/firefox-http-neverssl.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

<a href="https://www.jefftk.com/firefox-http-localhost-big.png"><img class="mobile-fullwidth" height="32" src="https://www.jefftk.com/firefox-http-localhost.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

Chrome:

</p>

<p>

<a href="https://www.jefftk.com/chrome-https-jefftk-big.png"><img class="mobile-fullwidth" height="28" src="https://www.jefftk.com/chrome-https-jefftk.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

<a href="https://www.jefftk.com/chrome-http-neverssl-big.png"><img class="mobile-fullwidth" height="28" src="https://www.jefftk.com/chrome-http-neverssl.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

<a href="https://www.jefftk.com/chrome-http-localhost-big.png"><img class="mobile-fullwidth" height="28" src="https://www.jefftk.com/chrome-http-localhost.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

Safari:

</p>

<p>

<a href="https://www.jefftk.com/safari-https-jefftk-big.png"><img class="mobile-fullwidth" height="31" src="https://www.jefftk.com/safari-https-jefftk.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

<a href="https://www.jefftk.com/safari-http-neverssl-big.png"><img class="mobile-fullwidth" height="31" src="https://www.jefftk.com/safari-http-neverssl.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

<a href="https://www.jefftk.com/safari-http-localhost-big.png"><img class="mobile-fullwidth" height="31" src="https://www.jefftk.com/safari-http-localhost.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

Despite the unusual URL bar treatment, the major browsers do now all treat this
configuration as a <a href="https://developer.mozilla.org/en-US/docs/Web/Security/Secure_Contexts">secure
context</a> (<a href="https://www.w3.org/TR/secure-contexts/#localhost">spec</a>),
which means you can use features that <a href="https://developer.mozilla.org/en-US/docs/Web/Security/Secure_Contexts/features_restricted_to_secure_contexts">require
secure contexts</a>, like <a href="https://developer.mozilla.org/en-US/docs/Web/API/Web_Crypto_API">crypto</a>,
<a href="https://developer.mozilla.org/en-US/docs/Web/API/Web_MIDI_API">MIDI</a>,
or <a href="https://developer.mozilla.org/en-US/docs/Web/API/Geolocation">geolocation</a>.

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid0wWvj6DgTvt9MJt9oE26tDQJo3MV29NRrEecNxGFTrfiDWkLpY8oCNZtLHWtu4qA4l">facebook</a>, <a href="https://mastodon.mit.edu/@jefftk/109611527318800371">mastodon</a></i></p>

