---
title: "Match Sentences Using Regex"
date: 2024-04-26
tags:
  - regex
---

## Match All Sentences

The following regex matches any sentence ending with a period ".". If a sentence ends with a question mark "?" or an exclamation mark "!", it will be matched as part of the nearest sentence that ends with a period.

`([A-Z].+?(?=(?:\. {1,2}[A-Z])|[\.?!]$)[\.?!])`

## Match Sentences Containing a String

It is often more useful to match sentences containing specific words. Replace the placeholders «string1» and «string2» with the needed words.

`[A-Z][^\\.;]*(string1|string2)[^\\.;]*`

[Source](https://www.sitepoint.com/community/t/regex-to-extract-whole-sentences-that-contain-a-certain-word/5408/2)  
