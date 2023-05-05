# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Not Getting Hacked
 - [https://www.jefftk.com/p/not-getting-hacked](https://www.jefftk.com/p/not-getting-hacked)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2022-12-21 08:00:00+00:00

<p><span>

A lot of people get hacked or phished, and being completely secure is
somewhere between difficult and impossible, especially if someone
trying hard to hack you in particular.  But there are several simple
things you can do that decrease your risk a lot:

</span>

<p>

</p>

<ul>
<li><p>Use a password manager that fills in fields automatically.
</p></li>
<li><p>Configure 2FA with security keys.
</p></li>
<li><p>Read "sign in with <i>provider</i>" (oAuth) screens carefully.
</p></li>
<li><p>Encrypt your laptop.
</p></li>
<li><p>Be cautious with inbound communication.
</p></li>
</ul>



<p>

Why these things?  You can make computers do stuff random other people
normally can't: transfer your money, post to social media as you, read
your private documents, control your employer's systems, etc.  If an
attacker can trick the right systems into thinking the are you, they
can take your money, exploit your secrets, or use you to get to
others.

</p>

<p>

A strategy of putting in a lot of mental effort to always make the
right security decision in the moment doesn't work well for humans: we
make mistakes, especially when we're doing routine things or are
distracted, tired, hungry, etc.  Instead:

</p>

<p>

</p>

<ul>
<li><p>Use tools so you can't mess up even if you're not paying
       attention.
</p></li>
<li><p>Understand the remaining cases where you do need to take
       special care.
</p></li>
</ul>



<p>

Password managers, laptop encryption, and security keys are
examples of the former, while being careful with 2FA codes, oAuth
screens, and inbound communication are examples of the latter.

</p>

<p>

In the most common attacks someone gets a copy of what the computer
checks to make sure you are you (your "credentials").  For example, if
your email is protected only with a password then if they can get your
password they can log into your email.

</p>

<p>

The most common way for someone to learn your password is using the
same one on multiple sites.  Say you use "<i>hunter2</i>" everywhere and you
create an account on "Joe's Shoes and Wallpaper" to buy sneakers.
They later get hacked, their passwords get cracked, and now the
attacker knows you used "<i>hunter2</i>".  They try this on your email
account, learning your address from Joe's records, and it works. This
is an especially worrying scenario because you probably have a lot of
other accounts that will send password resets to your email, and now
the attacker can control those as well.

</p>

<p>

Remembering passwords for hundreds of sites isn't practical, so you
want something that lets you generate a random password for each site
and then stores it for you: a "password manager".  But this isn't
enough on its own, because the second most common risk to
passwords is fake login pages.  If you click on a link and get:

</p>

<p>

<a href="https://www.jefftk.com/gmail-login-big.png"><img alt="gmail login screen" class="mobile-fullwidth" height="614" src="https://www.jefftk.com/gmail-login.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

You want to enter your username and password if this is
<code>accounts.google.com</code> but not if it's
<code>accounts.google.com.evil</code>.  Closely examining the URL to
make sure it's the right one helps, but humans make mistakes.
Instead, you want a password manager that, in addition to remembering
your passwords, only provides them to login pages on the correct
domain.

</p>

<p>

I use <a href="https://passwords.google.com/">Google's password
manager</a> which is integrated into Chrome and Android; if you're
fully in the Apple ecosystem you might use <a href="https://support.apple.com/guide/mac-help/use-keychains-to-store-passwords-mchlf375f392/mac">Apple's
Keychain</a>.  Firefox also <a href="https://support.mozilla.org/en-US/kb/password-manager-remember-delete-edit-logins">has
one</a>.  Stand-alone password managers include <a href="https://bitwarden.com/">Bitwarden</a> and <a href="https://1password.com/">1Password</a>; if you use one of these
make sure you set up browser integration so you're not pasting
passwords, protecting you against fake login pages.  Use separate
password managers (or separate "vaults" within a single manager) for
work and personal accounts so that when you eventually leave you can
separate them cleanly.

</p>

<p>

Even with an autofilling password manager there will be occasional
times when it doesn't work and you need to copy-paste: be very careful
that the URL is correct when doing that, because this is exactly the
problem you would run into if someone was trying to get your password.

</p>

<p>

Another layer of protection here is ensuring that a password on its
own isn't enough to give access to your account.  This is called
"two-factor authentication" or 2FA.  The most common form of 2FA is to
use a phone number in addition to a password: when you try to log in
from a new device they text you a code which you can use to
demonstrate you have access to the phone number.  This is probably
more secure than not doing it, but it isn't very good:

</p>

<p>

</p>

<ul>

<li><p>An attacker could trick the phone company (or bribe an employee)
into reassigning your number to them. ("<a href="https://en.wikipedia.org/wiki/SIM_swap_scam">simjacking</a>")
</p></li>
<li><p>You could be tricked into giving the code to an attacker.
</p></li>
<li><p>Sometimes sites call a phone number "2FA", but then will let
someone who only controls the phone number reset your password,
meaning it's really just a single factor.
</p></li>
</ul>



<p>

The first two of these can be fixed by using the security key <a href="https://support.google.com/accounts/answer/9289445">built into
your phone</a>. You register your key with a site, and then future
logins it checks that you still have the same key.  If you're on
<code>accounts.google.com.evil</code> your key will send something
that <code>accounts.google.com</code> will reject.

</p>

<p>

But what if you lose your phone, or don't have it with you?  The big
risk with 2FA is that if you lose your second factor you lose access
to your account.  The standard solution here is to have multiple
security keys, so that even if you lose one you still have the others.
You can get additional security keys as little USB things.  They come
in both USB-A and USB-C versions: I like the USB-A ones so I can plug
them into USB hubs.  I've used Yubico's <a href="https://www.yubico.com/product/security-key-nfc-by-yubico/">Security
Key</a> ($25) and Google's <a href="https://store.google.com/us/product/titan_security_key">Titan
Key</a> ($30).  Looking now, Adafruit's <a href="https://www.adafruit.com/product/3363">FIDO2 Key</a> ($10) seems
to be the cheapest option, though it doesn't have NFC (fine for your
computer, annoying for your phone).  Having one at work and one at
home in addition to the one built into your phone would be ideal, so
that even if you lose one and then one breaks, you still have a third.

</p>

<p>

If you lose a device, you do have some work: for every account it was
configured on you need to unregister it and then register a
replacement.  This means you need to keep track of which sites you've
configured 2FA with, because you'll need to repeat that process of
unregistering the old one and registering a new one on each site.  You
don't want to set it up on too many sites: just the ones where the
consequences of getting hacked are large enough to justify the extra
hassle.  I currently use my security keys for five accounts: personal
Google, work Google, GitHub, Facebook, and PyPI.

</p>

<p>

One way to get the protection of security keys on sites without
needing to register your key with them (and the extra work when you
need to change keys) is to use oAuth login.  This looks like "Sign in
with Google", "Sign in with Apple", "Sign in with GitHub", etc.  I'm
pretty happy using Google's oAuth everywhere: my Google account is
well protected and I think Google's security team is very good.

</p>

<p>

One issues this does have is that if you use a single account as the
root of your online identity and then get locked out of that account,
you're in a pretty bad situation.  When I've described this approach
<a href="https://news.ycombinator.com/item?id=33936296">before</a> one
reaction I've gotten is something like "but people do get locked out
of their Google accounts, why would you risk that?" If you look over
the <a href="https://hn.algolia.com/?q=google+account+locked+out">reports
people give</a>, though, they're predominately people who set up 2FA and then
lost the thing they were using as their second factor.  If you make
sure to always have multiple active 2FA methods (like the three
security keys I recommend above), however, I think this risk is very
low.

</p>

<p>

You might sometimes see people talking about "<a href="https://en.wikipedia.org/wiki/Time-based_one-time_password">TOTP</a>"
authentication codes.  These are where you install an app on your
phone (Google Authenticator, Authy, etc) and configure it when setting
up 2FA.  It shows a different code every minute, and the site can see
the same code.  Every time you log in you provide the code, and unless
someone steals or hacks your phone they won't have it.  I don't think
TOTP codes make sense anymore: security keys are better (they protect
you against fake login pages) and all the sites I used to use codes on
now support keys.

</p>

<p>

In a few years I'm hoping all of this will be a lot simpler as the
world moves to <a href="https://blog.chromium.org/2022/12/introducing-passkeys-in-chrome.html">passkeys</a>,
but they're not widely supported yet.

</p>

<p>

Instead of someone getting access to your account with a password,
another big risk is through a lost laptop.  On a normal laptop someone
with a bit of skill can read everything on it, even if you have a
password set.  This means someone could act as you on any site you're
currently logged in to.  Encrypting your laptop fixes this, because
the data stored on your laptop is now gibberish without your password.
On Mac this is <a href="https://support.apple.com/en-us/HT204837">FileVault</a>, on
Windows it's <a href="https://support.microsoft.com/en-us/windows/device-encryption-in-windows-ad5dcf4b-dbe0-2331-228f-7925c2a3012d">BitLocker</a>;
Ubuntu turns it on <a href="https://ubuntu.com/core/docs/uc20/full-disk-encryption">by
default</a>.  This would be an even bigger risk with phones, since
they're smaller and easier to lose, but modern ones are already
encrypted (<a href="https://source.android.com/docs/security/features/encryption">Android</a>,
<a href="https://support.apple.com/guide/security/encryption-and-data-protection-overview-sece3bee0835/web">iOS</a>).

</p>

<p>

Even if someone can't log in as you, or steal your laptop and already
be logged in as you, they might be able to trick you into delegating
control to them.  For example, if you try to use Google
to create a Twitter account you'll see something like:

</p>

<p>

<a href="https://www.jefftk.com/sign-in-with-google-big.png"><img alt="oauth screen asking for email address" class="mobile-fullwidth" height="604" src="https://www.jefftk.com/sign-in-with-google.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

This is fine: this is the "oAuth login" I was talking about above, and
is saying Twitter will get a few pieces of information, but it won't
be able to pull arbitrary things from my Google account.

</p>

<p>

On the other hand, if you click "sign in with Google" on another site
and see:

</p>

<p>

<a href="https://www.jefftk.com/gmail-oauth-read-access-big.png"><img alt="oauth asking to read email" class="mobile-fullwidth" height="768" src="https://www.jefftk.com/gmail-oauth-read-access.png" width="550" /><div class="image-vertical-spacer"></div></a>

</p>

<p>

You should be very alarmed!  This is asking for permission to read
your email, which as we talked about above translates into control
over all the accounts which let you reset your password over email.

</p>

<p>

Small wording differences on these screens can have a very large
effect, and the wording is something security folks at these companies
think really hard about.  For example, someone was <a href="https://news.ycombinator.com/item?id=33917962">recently
tricked</a> into letting an attacker control their GitHub account
where after clicking "Sign in with GitHub" they "clicked through a
bunch of pages because its the same drill every time."

</p>

<p>

The last major place where I think extra care is needed is when
someone else contacts you.  If you get a phone call from your bank,
are you sure it's actually your bank?  If you get an email that it
says it's from your IT department, is it actually?  It's generally
very hard to tell: they can fake the number they're calling from, or
the email address they're sending from.  Or they can just send you
something that looks legitimate enough that you don't think to check.
The safest thing to do here, especially if you're unsure, is to look
up the correct number/address in an external source and initiate
communication yourself.

</p>

<p>

This does still leave some holes, especially around running software
past when it will still get security updates, not installing security
updates, and installing software and browser extensions, but someone
who follows the guidelines above should have a much lower risk of getting
hacked or phished than the typical person.

</p>

<p>

(This is all looking at things from the perspective of what you as an
individual might choose to do to keep your accounts safe.  What sorts
of policies organizations should have, including options for automatic
enforcement, is also an interesting and deep topic, which I'm not
trying to get into here.)

</p>

<p>

<i>Thanks to Taymon Beal for reading a draft and providing feedback.</i>

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid0ptPi9LJbPEvoDLLULXEkC3zkp4awk66GgXhmhndKWkdXBWw9p9ibS5GQmoYKdk2wl">facebook</a>, <a href="https://lesswrong.com/posts/ESp3SsuqWrht7SApu">lesswrong</a>, <a href="https://news.ycombinator.com/item?id=34092956">hacker news</a>, <a href="https://mastodon.mit.edu/@jefftk/109553806777263678">mastodon</a></i></p>

