===================
String Manipulation
===================
The Bigger Picture
------------------

Python 3 strings are sequences of Unicode, not bytes. What is Unicode? Watch `this Tedx Talk <https://www.youtube.com/watch?v=IRdupNXpm8k>`_.

So, what does it means if Python strings uses UTF-8 unicode encoding? 
Hint: Remember we asked earlier in **Data Types** topic how certain symbols like Chinese characters are represented in binary? 

Syntax and Semantics - Learning Python Grammar
----------------------------------------------
Explore on your own to try the grasp how to create string, play with string slices and string methods. 
Also use ``len()`` built-in function to check the string size and ``print()`` to produce readable output. 

Open up IDLE.

>>> 'allows embedded "double" quotes'
>>> "allows embedded 'single' quotes"
>>> '''Three single quotes'''
>>> """Three double quotes"""
>>> ('Put several strings within parentheses '
... 'to have them joined together.')
>>> text = '''this is
... a
... paragraph'''
>>> text
>>> print(text) # notice any difference between using print() and without ?

>>> word = 'Python'
>>> len(word)
>>> some_word = '你好'
>>> len(some_word)

>>> 3 * 'hello' + 'world'
>>> word = 'Python'
>>> word[0]
>>> word[5]
>>> word[-1]
>>> word[0:5]
>>> word[5]
>>> word[2:5]

>>> for letter in word:
...    print(letter)
...

Critical Thinking - Discussions
-------------------------------
1. What did you notice is the difference when displaying ``text`` vs. ``print(text)`` above? 
2. What did you discover when applying math operator to string data type?
3. What happens if you slice ``word[2:10]`` ? Why?
4. If we can slice string like ``word[2:5]``, what do you think a string contains? Hint: Refer to `The Bigger Picture` section above.
5. What does the ``for`` loop do? 
6. What does the ``in`` operator do?

Problem Solving
---------------

Now try this in IDLE.

>>> s1 = 'hello'
>>> s2 = s1.replace('l', 'p')
>>> s1
>>> s2

1. What is this ``replace`` method? Hint: Refer to :ref:`Quick Resources <quick-resources>`.
2. Referring to **Variable, Statement and Expression** topic earlier, is string mutable or immutable? How do you prove it? Hint: Use ``id()`` built-in function.
3. What does it means when we try to alter the value of strings like using ``replace()`` ?  Is the ``id()`` the same?
4. Work on this `assignments <https://repl.it/data/classrooms/share/9c0e9a152b02097c659ba3c75d4e04dd>`_ using the built-in string methods. In the assignments, you'll learn how to search, count and perform string comparison.

Best Practices
--------------
1. Standardize using ` or " throughout your program for code readability. Stick to one way.

Remember
--------
1. Python 3 strings are sequence of Unicode. This means you can store all the symbols of Unicode supports in strings like Chinese characters!
2. Since string is a sequence of Unicode, you can access a specific character / symbol by slicing it. For example, ``"hello"[0:2]`` will return ``he``.
3. You can traverse a string using ``for`` loop and ``in`` operator. More on this in **Looping** topic.
4. There are tonnes of built-in string methods you can use to manipulate string.  

.. _quick-resources-strings:

Quick Resources
---------------
1. Python Text Sequence - https://docs.python.org/3/library/stdtypes.html#text-sequence-type-str
2. Python Strings & Methods - https://docs.python.org/3/tutorial/introduction.html#strings
3. String Processing Operations - https://docs.python.org/3/library/text.html#stringservices

