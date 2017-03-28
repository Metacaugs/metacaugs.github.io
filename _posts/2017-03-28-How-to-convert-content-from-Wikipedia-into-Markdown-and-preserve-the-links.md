---
layout: post
title:  "How to convert content from Wikipedia into Markdown and preserve the links"
categories: Blog
tags:  
author: Robert.Best
---

It's fairly simple to convert Wikipedia content, including the links, into Markdown.

1. View source on any Wikipedia page, by clicking the edit link at the top of the page, and then copy the marked up content that you want
2. Paste what you copied into this tool: [pandoc](http://pandoc.org/try/) , and convert the text from MediaWiki into Markdown. ('Strict' is the option I use)
3. Edit the output from the previosu step, by inserting `https://wikipedia.org/wiki/` before any links that are relative Wikipedia links in the link list at the bottom
4. Paste the end result from above into your blog post, Lexicon iten, or wherever else likes to receive Markdown.

Done! 
