---
title: MD036 - Emphasis used instead of a header
tags:  [headers, emphasis]
alias: no-emphasis-as-header
---

This check looks for instances where emphasized (i.e. bold or italic) text is
used to separate sections, where a header should be used instead:

    **My document**

    Lorem ipsum dolor sit amet...

    _Another section_

    Consectetur adipiscing elit, sed do eiusmod.

To fix this, use markdown headers instead of emphasized text to denote
sections:

    # My document

    Lorem ipsum dolor sit amet...

    ## Another section

    Consectetur adipiscing elit, sed do eiusmod.

Note: this rule looks for paragraphs that consist entirely of emphasized text.
It won't fire on emphasis used within regular text.


