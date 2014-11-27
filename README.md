ShowHide
========

Wiki macros implementation for simple show/hide of a content with some animations.
This version 2.0 is HTML compatible with the old version, so that existing project could continue styling 
with the same kind of CSS rules. However, it is now based on jQuery, and need requireJS, so it require
XWiki 5.x or more.

Usage
=====

Without effect
--------------

    {{showhide showmessage="Show" hidemessage="Hide" style="background-color: #ccc"}}
    Here is some hidden content that can become visible
    Here is some hidden content that can become visible
    Here is some hidden content that can become visible
    Here is some hidden content that can become visible
    {{/showhide}}

With a fade in effect
---------------------

    {{showhide showmessage="Show" hidemessage="Hide" effect="fade"  effectduration="2" style="background-color: #ccc"}}
    Here is some hidden content that can become visible
    Here is some hidden content that can become visible
    Here is some hidden content that can become visible
    Here is some hidden content that can become visible
    {{/showhide}}

Using ``effect="appear"` is still supported and provide the same behavior

With a sliding down effect
--------------------------

    {{showhide showmessage="Show" hidemessage="Hide" effect="slide"  effectduration="0.5" style="background-color: #ccc"}}
    Here is some hidden content that can become visible
    Here is some hidden content that can become visible
    Here is some hidden content that can become visible
    Here is some hidden content that can become visible
    {{/showhide}}

This effect is equivalent to ``effect="blind"`` in the 1.0 macro, so both ``slide`` and ``blind`` effect are now using
the exact same animation.
