---
layout: post
title: Previewing Markdown Documents from Bash
---

When you are writing a Markdown document (perhaps a README.md for a new gem), you may wish to preview what the rendered document will look like.

One cumbersome option is to push your branch to Github periodically, so you can view the rendered version online.  Here is a bash function that will allow for a faster workflow:

{% highlight bash %}
mdp() {
  local tmpfile='/tmp/markdown-preview.html';
  local srcfile=$1;
  perl ~/bin/Markdown.pl --html4tags $srcfile > $tmpfile;
  open $tmpfile;
}
{% endhighlight %}

You can put this in your .bash\_profile and then run `mdp README.md` to instantly preview your document in a new browser window.

### Requirements:

Download Markdown.pl from [http://daringfireball.net/projects/markdown/](http://daringfireball.net/projects/markdown/) and put it in your ~/bin/ directory (or elsewhere, and update the function to aim correctly at it.)

### Caveats:

No syntax highlighting or other Github-specific niceties.

