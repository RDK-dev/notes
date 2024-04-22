---
title: "Use Regex to Identify and Extract Any Words Enclosed Within Wikilinks"
date: 2024-04-10
date_modified: 2024-04-19
tags:
  - regex
---

I needed to extract any words surrounded by wikilinks format ``"[[ ]]"``. I put together this snippet of regex: \[\[\w+

It is not a fully working solution. This regex will extract two left brackets "[[" and first word of the wikilink.

***

Here is working regex which will match a string between [ ]. `(?<=\[).+?(?=\])`*
Here is a modified version to match a string between double brackets `(?<=\[\[).+?(?=\]\])`

[Source Stack Overflow](https://stackoverflow.com/questions/2403122/regular-expression-to-extract-text-between-square-brackets)
