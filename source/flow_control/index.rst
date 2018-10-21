============
Flow Control
============
The Bigger Picture
------------------
Program executes from top-down approach but what if you want to take control of how it flows?

This topic focuses on Python control flow statements.

* ``if...elif...else`` - we'll focus on this
* ``for`` - looping topic
* ``while`` - looping topic
* ``break`` - looping topic
* ``continue`` - looping topic

We'll learn the first one which is very useful for making decisions in programs.

It has a strong co-relation with what we learnt earlier on ``statement`` and ``expression``. 
Do you still remember what they are?

Syntax and Semantics - Learning Python Grammar
----------------------------------------------
Explore on your own to try the grasp how these flow statements work. Open up IDLE.

>>> a, b = 10, 3 
>>> if a > b:
...    print("yippie, a is greater than b!")
...
>>> if a > b: print("yippie, a is greater than b!") # one-liner !
>>> a = 1
>>> if a > b:
...    print("yippie, a is greater than b!")
... else:
...    print("Ooops")
...
>>> print("yippie, a is greater than b!") if a > b else print("Ooops ... ") # one-liner !
>>> a, b, c = 20, 30, 40
>>> if a < b and a < c:
...    print("a is the youngest!")
... elif b < a and b < c:
...    print("b is the youngest!")
... else:
...    print("c is the youngest!")
 
Critical Thinking - Discussions
-------------------------------
1. How do you form a condition ?
2. Is the ``if...elif`` condition a statement or expression ? Why ?
3. Can you identify all the different operators used ? 
4. What are ``<``, ``>``, ``and``, ``or`` operators? Hint: Refer to :ref:`Quick Resources <quick-resources-control-flow>` for full Python list operators.

Problem Solving
---------------
Speaking of condition, some values are inherently ``True`` or ``False``. Explore on your own with the built-in function ``bool()``.

Now try this in IDLE. 

>>> bool(0)
>>> bool(100)
>>> bool("True")
>>> bool("False")
>>> bool("")
>>> bool(0.1)
>>> bool(0.0)
>>> bool(True)
>>> bool(False)

1. What did you notice about the behaviour of certain data types? Hint: Refer to :ref:`Quick Resources <quick-resources-control-flow>` for Python truth value testing.
2. Can you try to code this chained conditionals (``if...elif...else``) ?
    .. image:: images/chained_condition.png
        :width: 50%
3. Can you try to code this nested conditioanls ? 
    .. image:: images/nested_condition.png
        :width: 70%

.. topic:: FAQ / Fun Facts

    | 1. I kept getting indentation errors!
    | Spaces and tabs are invisible to Python. It's extremely important that you standardize your indentation to 4 spaces. Refer to :ref:`Quick Resources <quick-resources-control-flow>` for Python style guide.

    | 2. What is this multi-assignment of ``a, b = 10, 3`` ?
    | It is called tuple unpacking. We'll learn about this in Data Structure later.

    | 3. What are those one liner ``if`` statement?
    | Ternary operator or aka conditional expression. This normally does not support more complex conditional ``if...elif...else`` statement.

Best Practices
--------------
1. Code one liner ``if`` statement for simple condition.
2. Code the traditional ``if...elif...else`` code block for more complex ones for readability sake.
3. Write more succinct condition if you know truthy and falsy (Python truth value).

Remember
--------
1. ``if..elif..else`` statement requires a condition expression that evaluates to boolean value. 
2. Use comparison (i.e. ``>``, ``<=``, ``==``) and logical (i.e. ``not``, ``and``, ``or``) to form condition.
3. Everything after ``:`` is a block of code belongs to the ``if...elif...else`` statement. Use indentation to indicate the block of code.

.. _quick-resources-control-flow:

Quick Resources
---------------
1. Python Control Flow - https://docs.python.org/3/tutorial/controlflow.html
2. Python Style Guide - https://www.python.org/dev/peps/pep-0008/#indentation
3. Full list of Python operator - https://docs.python.org/3/library/operator.html
4. Python Truth Value Testing - https://docs.python.org/3/library/stdtypes.html#truth-value-testing
