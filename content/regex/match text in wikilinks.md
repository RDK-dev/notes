---
title: "Use Regex to Identify and Extract Any Words Enclosed Within Wikilinks"
date: 2024-04-10
tags:
  - regex
---

I needed to extract any words surrounded by wikilinks format ``"[[ ]]"``. I put together this snippet of regex: \[\[\w+

It is not a fully working solution. This regex will extract two left brackets "[[" and first word of the wikilink.
