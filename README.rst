==================================
Demo of Embedded Hyperlink Aliases
==================================

`Embedded Aliases`_ in hyperlinks do not currently render correctly on github.
For example, the following source::

    `This <that_>`_ should link to the same place as that_.

    .. _that: https://github.com/

renders as

    `This <that_>`_ should link to the same place as that_.

.. _that: https://github.com/

Currently on GitHub, *this* does not link to the same place as *that*.
(Rst2html.py from Docutils==0.12 does render this correctly.)

.. _embedded aliases:
   http://docutils.sourceforge.net/docs/ref/rst/restructuredtext.html#embedded-uris-and-aliases
