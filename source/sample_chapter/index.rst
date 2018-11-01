This Is My Sample Chapter
=========================

Ok, here's my sample chapter.

This is another paragraph because of the blank line.

This
is
all
one paragraph. Because there
is
no blank
line.

Here I use *one* paire of asterisks for italics.

I can use **two** pairs of asterisks for bold.

Like lists?

* Start a list with an asterisk.
* Each item gets one.
* Most common mistake, if you need two lines
  don't forget to indent the second line.

  * You can have a list in a list too.
  * Don't forget a blank line between the lists

* Done with lists.

Heading Level 1
---------------

You can create headings with - and = and ~ underlines.

You can create a link by doing `Simpson`_ something like this.

.. _Simpson: http://simpson.edu

You can do sample code easily:

.. code-block:: python
    :linenos:
    :caption: Sample Code

    # Sample program
    print("Hello")

You can make ``monospaced text`` if you surround them with two back-ticks. Back-ticks are the
weird quote thing in the upper-left on your keyboard.

You can include an image by:

.. image:: images/my_image.png
    :width: 50%

Or a labeled image:

.. figure:: images/my_image.png
    :width: 50%

    This is my image caption.

Sample Table
------------

This is a sample table

============ =================
Fruit        Review
============ =================
Apple            3 stars
Pomegranite  5 stars
Grapes       3 stars
Pears        4 stars
Orange       2 stars
Cherries     1 star
============ =================

There are several ways of doing sample tables. The most frequent issue
that people have when making tables is mixing tabs and spaces. In Sublime,
if you select the text of a table, you can see tabs look differently than
spaces. Always use spaces, never tabs.