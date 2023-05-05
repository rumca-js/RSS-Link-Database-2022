# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Machine Learning Consent
 - [https://www.jefftk.com/p/machine-learning-consent](https://www.jefftk.com/p/machine-learning-consent)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2022-12-07 08:00:00+00:00

<p><span>

For years, researchers have trained machine learning systems on
whatever data they could find. People mostly haven't cared about this
or paid attention, I think because the systems hadn't been very good.
Recently, however, some very impressive systems have come out,
including ones that </span>

<a href="https://en.wikipedia.org/wiki/ChatGPT">answer questions</a>, 

<a href="https://en.wikipedia.org/wiki/GitHub_Copilot">complete
code</a>, and 

<a href="https://en.wikipedia.org/wiki/DALL-E">generate</a> 

<a href="https://en.wikipedia.org/wiki/Midjourney">images</a> 

<a href="https://en.wikipedia.org/wiki/Stable_Diffusion">from prompts</a>.



<p>

Because these are so capable a lot more people are paying attention
now, and there are big questions around whether it's ok that these
systems were trained this way.  Code that I uploaded to GitHub and the
writing that I've put into this blog went into training these models:
I didn't give permission for this kind of use, and no one asked me if
it was ok.  Doesn't this violate my copyrights?

</p>

<p>


The machine learning community has generally assumed that training
models on some input and using it to generate new output is legal, as
long as the output is sufficiently different from the input.  This
relies on the doctrine of "<a href="https://en.wikipedia.org/wiki/Fair_use">fair use</a>", which
does not require any sort of permission from the original author as
long as it is sufficiently "transformative".  For example, if I took a
book and replaced every instance of the main characters name with my
own I doubt any court would consider that sufficiently transformative,
and so my book would be considered a "derivative work" of the original
book.  On the other hand, if I took the words in the book and
painstakingly reordered them to tell a completely unrelated story,
there's a sense in which my book was "derived" from the original one
but I think it would pretty clearly be transformative enough that I
wouldn't need any permission from the copyright holder.

</p>

<p>

These models can be used to create things that are clearly derivative
works of their input. For example, people <a href="https://mobile.twitter.com/mitsuhiko/status/1410886329924194309">very
quickly realized</a> that Copilot would complete the code for <a href="https://www.beyond3d.com/content/articles/15/">Greg Walsh's</a>
<a href="https://en.wikipedia.org/wiki/Fast_inverse_square_root">fast
inverse square root</a> implementation verbatim, and if you ask any of
the image generators for the <a href="https://en.wikipedia.org/wiki/Mona_Lisa">Mona Lisa</a> or <a href="https://en.wikipedia.org/wiki/The_Starry_Night">Starry Night</a>
you'll get something close enough to the original that it's clearly a
knock-off.  This is a major issue with current AI systems, but it's
also a relatively solvable one. It's already possible to slowly check
that the output doesn't excessively resemble any input, and I think
it's likely they'll soon figure out how to do that efficiently.  On the
other hand, all of the examples of this I've seen (and I just did some
<a href="https://www.reddit.com/r/ArtistLounge/comments/xkbd1l/examples_of_ai_plagiarizing_existing_art/">looking</a>)
have been people trying to elicit plagiarism.

</p>

<p>

The normal use case is much more interesting, and more controversial.
While the transformative fair use justification I described above is
widely assumed within the machine learning community as far as I can
tell it hasn't been tested in court. There is currently a <a href="https://www.reddit.com/r/ArtistLounge/comments/xkbd1l/examples_of_ai_plagiarizing_existing_art/">large
class action lawsuit</a> over Copilot, and it's possible this kind of
usage will turn out not qualify.  Speculating, I think it's pretty
unlikely that the suit will succeed, but I've created a <a href="https://manifold.markets/JeffKaufman/will-the-github-copilot-litigation">prediction
market</a> on it to gather information:

</p>

<p>



</p>

<p>

Aside from the legal question, however, there is also a moral or
social question: is it ok to train a model on someone's work without
their permission? What if this means that they and others in their
profession are no longer able to earn a living?

</p>

<p>

On the second question, you could imagine someone creating
a model where they used only data that was either in the public domain
or which they'd purchased appropriate licenses for.  While that's
great for the particular people who agree and get paid, a much larger
number would still be out of work without compensation.  I do think
there's potentially quite a bad situation, where as these systems get
better more and more people are unable to add much over an automated
system, and we get massive <a href="https://en.wikipedia.org/wiki/Technological_unemployment">technological
unemployment</a>.  Now, historically worries here proved unfounded, and
technology has consistently been much more of a human complement than
human substitute.  As the saying goes, however, that was also the case
for horses until it wasn't.  I think a <a href="https://en.wikipedia.org/wiki/Universal_basic_income">Universal
Basic Income</a> is probably the best approach here.

</p>

<p>

On the first question, learning from other people's work without their
consent is something humans do all the time.  You can't draw too
heavily on any one thing you've seen without following a complex set
of rules about permission and acknowledgement, but human creative work
generally involves large amounts of borrowing.  These machine learning
systems are not humans, but they are fundamentally doing a pretty
similar thing when they learn from examples, and I don't see a strong
reason to treat their work differently here.  Because these systems
don't currently understand how much borrowing is ok we do need to
apply our own judgment to avoid technologically-facilitated
plagiarism, but the normal case of creating something relatively
original that pulls from a wide range of prior work is fine for us to
do with our brains and should be equally ok for us to do with our
tools.

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid0zVuJxxMMSMGbSU8hA2hDG88kffHzTJpSY73q6CBNmZaaHwa5CskM22iHmkDtB859l">facebook</a>, <a href="https://lesswrong.com/posts/dqQGrPRYamrtLvdLz">lesswrong</a>, <a href="https://mastodon.mit.edu/@jefftk/109475991749825173">mastodon</a></i></p>

