Links, references, and labels
######################################################################

Simplest link
**********************************************************************
`Python <http://python.org>`_

Using labels
**********************************************************************
It is more convenient to attach labels to links so they cna be reused and don't clog up the text too much.

The switch to reStructuredText and Sphinx was made with the `python 2.6`_ release.

.. _`python 2.6`: https://docs.python/org/whtsnew/2.6.html

make sure don't have same label in a single document, otherwise lead to an error.

Conjunction with headers
**********************************************************************
Here is an example:

The introduction section
======================================================================

This section contains:

- `chapter 1`_
- `chapter2`_

    1. my_label_

    2. `And a label link with a custom title <my_label>`_

Chapter 1
---------------------------------------------------------------------

Jumping back to beginning of `chapter 1`_ is also possible. or jumping to `Chapter 2 <chapter2>`_

.. _chapter2:

Chapter 2 With a longer title 
---------------------------------------------------------------------

The next chapter.

.. _my_label:

The label points here.

Back to `the introduction section`_

