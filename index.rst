Documentation, how to use Sphinx and reStructuredText
##################################################################

Welcome Chapter
******************************************************************
Documenting code can be both fun and useful! ...

Topics covered in this chapter are as follows:

- The reStructuredText syntax
- Setting up documentation using Sphinx
- Sphinx style docstrings
- Google style docstrings
- NumPy style docstrings

Common syntax Chapter
*****************************************************************
- Emphasis(italic) text: *emphasis for this phrase*.

- Extra emphasis(bold) text: **extra emphasis for this phrase**.

- For lists without numbers, a simple dash with spaces after it:

  - item 1
  - item 2

- For lists with numbers, the number followed by a period and a space:

  1. item 1
  2. item 2

- Interpreted text: These are domian specific. Within Python documentation, the default role is code which means that surround text with back ticks will convert your code to use codetags. For example, `if spam and eggs:`. Different roles can be set through either a role prefix or suffix depending on your preference. For example, :math:`E=mc^2` to show mathematical equations.

- Inline literals: This is formatted with a mono-space font, which makes it ideal for inline code. Just add two back ticks to ``add some code``.

- References: These can be created througg a trailing underscore. They can point to headers, links, labels, and more. The next section will cover more about thest, but the basic syntax is simply `Python <http://python.org>`_  or enclosed in back ticks when the reference contains spaces, `Python reference link`_.

.. _`Python reference link`: http:/python.org

- To escape the prededing characters, the backslash can be used, So if you wish to have an asterisk with emphasis, it's possible to use *\**, quite similar to escaping in Python strings.

Convert reStructuredText to HTML
**********************************************************************
Section 1: Install `docutils`
======================================================================
.. code:: bash
    
    $ pip install docutils
    $ rst2html.py start.rst start.html

Section 2: Create map in vim
======================================================================
If use vim, add this line in `.vimrc` file:

.. code:: vim

    let mapleader = ',' "default is \, but , is better
    nmap <leader>r !rst2html.py % %<.html<cr>  "%< is current filename without extension 

It can convert current `filename.rst` to `filename.html` with a shortcut `, + r`.
