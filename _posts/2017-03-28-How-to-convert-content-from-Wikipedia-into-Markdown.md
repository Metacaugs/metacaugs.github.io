---
layout: post
title:  "How to convert content from Wikipedia into Markdown"
categories: Blog
tags:  
author: Robert Best
---

It's fairly simple to convert Wikipedia content, including the links, into Markdown.

1. View the raw markup for any Wikipedia article by clicking the edit link at the top of the page, then copy the portion of the content that you want.
2. Paste what you copied into this tool: [pandoc](http://pandoc.org/try/), and convert the text from MediaWiki into Markdown. (You will have to find out what type of Markdown is appropriate for your application. I use 'strict' in most cases right now)
3. Edit the output from the previous step, by inserting `https://wikipedia.org/wiki/` before any links that are relative Wikipedia links in the link list at the bottom.
4. Paste the end result from above into your blog post, lexicon item, or wherever else likes to receive Markdown.

Done! (Well, sort of... I'm sure there may be issues relating to your specific context. Also, a bit of trial and error will be required to get what I mean about the link list and relative links)
