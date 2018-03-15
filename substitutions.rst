Substitutions
#####################################################################

When writing documentation, it often happens that constructs are being repeated, the links have their own labelling system but there are more ways within reStructuredText. The substitution definitions make it possible to shorten directives so they can easily be re-used.

Let's assume we have a logo that we use quite often within a bit of text. Instead of typing the entire `.. image:: <url>` it would be very handy to have a shorthand to make it easier.

.. |python| image:: python.png
    :scale: 20

The Python programming language uses the logo: |python|


.. |author| replace:: Wang Xin

This page was written by |author|.
