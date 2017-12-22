==================================
Demo of Embedded Hyperlink Aliases
==================================

`Embedded Aliases`_ in hyperlinks :strike:`do not` currently render correctly on github.
For example, the following source::

    `This <that_>`_ should link to the same place as that_.

    .. _that: https://github.com/

renders as

    `This <that_>`_ should link to the same place as that_.

.. _that: https://github.com/

Currently on GitHub, *this* does :strike:`not` link to the same place as *that*.
(Rst2html.py from Docutils==0.12 does render this correctly.)

2014-10-13: I’ve opened `github/markup#382 <https://github.com/github/markup/issues/382>`_ on this issue.

2017-03-22: Github upgraded to a recent version of docutils, fixing the problem.  Hyperlink aliaes now work correctly.

.. _embedded aliases:
   http://docutils.sourceforge.net/docs/ref/rst/restructuredtext.html#embedded-uris-and-aliases
