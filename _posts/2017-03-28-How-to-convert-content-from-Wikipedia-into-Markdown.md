---
layout: post
title:  "How to convert content from Wikipedia into Markdown"
categories: Blog
tags:  
author: Robert.Best
---

It's fairly simple to convert Wikipedia content, including the links, into Markdown.

1. View the raw markup for any Wikipedia article by clicking the edit link at the top of the page, then copy the portion of the content that you want.
2. Paste what you copied into this tool: [pandoc](http://pandoc.org/try/), and convert the text from MediaWiki into Markdown. (You will have to find out what type of Markdown is appropriate for your application. I us 'strict' in most cases right now)
3. Edit the output from the previous step, by inserting `https://wikipedia.org/wiki/` before any links that are relative Wikipedia links in the link list at the bottom
4. Paste the end result from above into your blog post, Lexicon item, or wherever else likes to receive Markdown.

Done! (Well sort of, I'm sure there may be issues relating to your specific context)


Here is some example MediaWiki markup, and the Markdown that worked well for me with only a little bit of trial and error:

Raw MediaWiki: ( [Source](https://en.wikipedia.org/wiki/Metacognition) )
```
'''Metacognition''' is "[[cognition]] about cognition", "thinking about thinking", or "knowing about knowing" and higher order thinking skills. It comes from the root word {{'}}'''[[meta]]'''{{'}}, meaning beyond.<ref name="Metcalfe">Metcalfe, J., & Shimamura, A. P. (1994). Metacognition: knowing about knowing. Cambridge, MA: MIT Press.</ref> It can take many forms; it includes knowledge about when and how to use particular strategies for learning or for problem solving.<ref name="Metcalfe" /> There are generally two components of metacognition: knowledge about cognition, and regulation of cognition.<ref name="Schraw 1998 113–125">{{cite journal|last=Schraw|first=Gregory|title=Promoting general metacognitive awareness|journal=Instructional Science|year=1998|volume=26|pages=113–125|doi=10.1023/A:1003044231033}}</ref>
```

End result in Markdown:
```
**Metacognition** is “[cognition] about cognition”, “thinking about
thinking”, or “knowing about knowing” and higher order thinking skills.
It comes from the root word **[meta]**, meaning beyond.[1] It
can take many forms; it includes knowledge about when and how to use
particular strategies for learning or for problem solving. [1] There are
generally two components of metacognition: knowledge about cognition,
and regulation of cognition.[1]

[1] Metcalfe, J., & Shimamura, A. P. (1994). Metacognition: knowing
about knowing. Cambridge, MA: MIT Press.
[cognition]: https://wikipedia.org/wiki/cognition "wikilink"
[meta]: https://wikipedia.org/wiki/meta "wikilink"
```
