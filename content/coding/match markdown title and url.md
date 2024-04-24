---
title: "Match Markdown Title and Url Using Regex"
date: 2024-04-24
tags:
  - regex
---

It can be useful to extract only the title of a Markdown URL by using the following regex pattern: `(?<=\[).+?(?=\])`.

The second part involves matching content between parentheses: `(?<=\().+?(?=\))`.

Another version of this is to match content with parentheses, not only within them: `\((.*?)\)`.

Although this is usually the Markdown syntax for a URL, this regex pattern will match any content between parentheses, regardless of whether it contains 'http' or 'https'.

Here is a combined version to match the entire Markdown link syntax (both title and URL): `\[(.+?)\]\((.+?)\)`.

****

If you want more examples with explanation, take a look at this article about [Advanced regular expression features to match Markdown links](https://www.michaelperrin.fr/blog/2019/02/advanced-regular-expressions).
