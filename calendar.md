---
layout: page
title: Calendar
description: Listing of course modules and topics.
---

# Calendar

- Previous offerings: [Fall 2023](nyu-cs2590.github.io/fall2023/) [Spring 2023](nyu-cs2590.github.io/spring2023/)
- The schedule below is tentative and subject to change.
- All course materials can be found on [Github](https://github.com/nyu-cs2590/course-material).
- We do not have a reference textbook, but some lectures follow materials from [Speech and Language Processing](https://stanford.edu/~jurafsky/slp3/) (JM below) and [Dive into Deep Learning](https://d2l.ai) (D2L below).

{% for module in site.modules %}
{{ module }}
{% endfor %}
