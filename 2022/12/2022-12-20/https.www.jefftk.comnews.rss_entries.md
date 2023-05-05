# Source:Jeff Kaufmann, URL:https://www.jefftk.com/news.rss, language:en-US

## Logging Shell History in Zsh
 - [https://www.jefftk.com/p/logging-shell-history-in-zsh](https://www.jefftk.com/p/logging-shell-history-in-zsh)
 - RSS feed: https://www.jefftk.com/news.rss
 - date published: 2022-12-20 08:00:00+00:00

<p><span>

By default most shells don't log your history in a detailed durable
way, which gives up one of the big advantages of working on the
command line.  Good history lets you look back at things you did
months or years ago, in a searchable and skimmable fashion, so you can
answer questions like "how did I generate this number?", "what was
that trick I used?", or "if I'm doing something similar now what
should I recall from last time?"

</span>

<p>

I use <code>bash</code> as my shell and have <a href="https://www.jefftk.com/shell-history-and-the-value-of-text-only-environments">long</a>
<a href="https://www.jefftk.com/p/you-should-be-logging-shell-history">used</a>:

</p>

<p>

</p>

<pre>
.bashrc:
  promptFunc() {
    echo "$(date +%Y-%m-%d--%H-%M-%S) $(hostname) $PWD $(history 1)" \
      &gt;&gt; ~/.full_history
  }
  PROMPT_COMMAND=promptFunc
</pre>



<p>

I was recommending this to folks at work, but they use
<code>zsh</code>.  In <code>zsh</code> you can get a lot of the way
here by setting <code>INC_APPEND_HISTORY</code> (append to history
immediately instead of waiting for the shell to exit),
<code>SAVEHIST=1000000000</code> (effectively don't limit the history
size on disk), and <code>EXTENDED_HISTORY</code> (to store timestamps
with history entries).  But you risk losing most of your history if you
ever accidentally invoke <code>zsh</code> without these set, and it
doesn't write the directory you ran the command in (which is metadata
I reference a lot).

</p>

<p>

<a href="https://mikemc.cc/">Mike</a> tweaked my snippet to run in
<code>zsh</code>:

</p>

<p>

</p>

<pre>
.zshrc:
  precmd() {
    echo "$(date +%Y-%m-%d--%H-%M-%S) $(hostname) $PWD $(history -1)" \
      &gt;&gt; ~/.full_history
  }
</pre>



<p>

The two changes are that <code>zsh</code> uses <code>precmd</code>
instead of <code>PROMPT_COMMAND</code>, and that you need
<code>history -1</code> instead of <code>history 1</code>.

</p>

<p>

You can still use the same <code>histgrep</code> command on both:

</p>

<p>

</p>

<pre>
function histgrep {
  local n_lines=10
  if [[ "$1" =~ ^[0-9]*$ ]]; then
    n_lines="$1"
    shift
  fi
  grep "$@" ~/.full_history | tail -n "$n_lines"
}
</pre>



<p>

Note that this doesn't replace your shell's built-in history tooling,
and I wouldn't recommend turning that off.  This just a very cheap
additional layer of logging with additional metadata and less risk of
accidental deletion.

  </p>

<p><i>Comment via: <a href="https://www.facebook.com/jefftk/posts/pfbid0FGzTeUeQ9dzTifJn25J8pZyHuA6iJrrokK2FuRTkH6DCkpYPnj6doxwjPWKiL4UHl">facebook</a>, <a href="https://lesswrong.com/posts/6WGyKKQnfaGa3YtMn">lesswrong</a>, <a href="https://mastodon.mit.edu/@jefftk/109549552545020538">mastodon</a></i></p>

