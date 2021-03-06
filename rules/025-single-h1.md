---
title: MD025 - Multiple top level headers in the same document
tags:  [headers]
alias: single-h1
---

This rule is triggered when a top level header is in use (the first line of
the file is a h1 header), and more than one h1 header is in use in the
document:

    # Top level header

    # Another top level header

To fix, structure your document so that there is a single h1 header that is
the title for the document, and all later headers are h2 or lower level
headers:

    # Title

    ## Header

    ## Another header

Rationale: A top level header is a h1 on the first line of the file, and
serves as the title for the document. If this convention is in use, then there
can not be more than one title for the document, and the entire document
should be contained within this header.


