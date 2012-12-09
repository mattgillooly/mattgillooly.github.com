---
layout: post
title: Previewing Markdown Documents from Vim
---

In a recent post, I shared the Bash function that I've been using to [streamline my Markdown editing workflow][my-original-markdown-post].
Soon after, I [was directed][twitter-link] to a [plugin for Sublime Text][st-plugin] which enabled Markdown previewing directly from the editor.
Previewing Markdown from my editor was a compelling idea, so I went in search of a similar plugin for Vim.

[The Vimscript I found][vim-plugin] looks great.
However, I had been meaning to learn Vimscript for some time, and it seemed like this would be a quick first project to get my feet wet.
I started with [hojberg's Vest plugin](https://github.com/hojberg/vest) as a template, and I had implementes my function as a Vim plugin in less than half an hour.

So, I present to you: my [vim-markdown-preview](https://github.com/mattgillooly/vim-markdown-preview) plugin.

It was very easy to get started, and the plugin has already proven handy while writing this post.
I would not be surprised if I soon switch to [swaroopch's more feature-rich plugin][vim-plugin] for my actual day-to-day use, but this has definitely been a worthwhile learning experience.
Next time I want to customize my writing or development workflow, I won't hestitate to hack out some Vimscript to get it done.

As a next step, hojberg recommended that I read [Learn Vimscript the Hard Way][hardway].
It looks like a solid resource, if well beyond the scope of this afternoon's hacking.


[my-original-markdown-post]: http://mattgillooly.github.com/2012/11/28/previewing-markdown-documents.html
[twitter-link]: https://twitter.com/pablo2dot0/status/274934330915164163
[st-plugin]: https://github.com/revolunet/sublimetext-markdown-preview
[vim-plugin]: https://github.com/swaroopch/vim-markdown-preview/blob/master/ftplugin/markdown.vim
[hardway]: http://learnvimscriptthehardway.stevelosh.com/
