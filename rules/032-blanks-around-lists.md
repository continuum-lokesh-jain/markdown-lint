---
title: MD032 - Lists should be surrounded by blank lines
tags:  [bullet, ul, ol, blank_lines]
alias: blanks-around-lists
---

This rule is triggered when lists (of any kind) are either not preceded or not
followed by a blank line:

    Some text
    * Some
    * List

    1. Some
    2. List
    Some text

To fix this, ensure that all lists have a blank line both before and after
(except where the block is at the beginning or end of the document):

    Some text

    * Some
    * List

    1. Some
    2. List

    Some text

Rationale: Aside from aesthetic reasons, some parsers, including kramdown, will
not parse lists that don't have blank lines before and after them.

Note: List items without hanging indents are a violation of this rule; list
items with hanging indents are okay:

    * This is
    not okay

    * This is
      okay

