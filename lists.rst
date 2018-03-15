List
######################################################################

Enumerated list
**********************************************************************

# character functions as an automatic enumeration:

1. With
2. Numbers

a. With
#. letters

i. Roman
#. numerals

(1) With
(2) Parenthesis

Bulleted list
**********************************************************************
In HTML, they are the same, but in LaTeX they cna differ.

- dashed
- and more dashes

* asterisk
* stars

+ plus
+ and plus

Option list
**********************************************************************
The option list is one meant specifically for documenting the command line arguments of a program. comma space is recognized as a separator for options.

-s, --spam  This is the spam option
--eggs      This is the eggs option


Definition list
*******************************************************************************
spam 
    Spam is a canned port meat product
eggs 
    Is, similar to spam, also food


Nested list
*******************************************************************************
Nesting items is actually not limited to lists and can be done with multiple types of
blocks, but the idea is the same. Just be careful to keep the indenting at the correct level.
If you don't, it either won't be recognized as a separate level or you will get an error.

1. With
2. Numbers
   
    (food) food

        spam 
            Spam is a canned port meat product

        eggs
            Is, similar to spam, also food

    (other) non-food stuff
