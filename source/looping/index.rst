=======
Looping
=======
The Bigger Picture
-------------------
Continue from where we left off in `Flow Control` topic, we'll learn about looping in this topic. 

From the word `looping` itself, you can guess how your program will flow.

.. topic:: Looping In a Nutshell - David Baumgold

    A loop is a **method of programming** that allows you to **repeat the same action or idea** over and over **without repeating code.**

Syntax and Semantics - Learning Python Grammar
----------------------------------------------
Explore on your own for 5 mins on the different ``while``, ``for``, ``break`` and ``continue`` statements in Python. 

Open up Python IDLE and type away. 

>>> arrive = False
>>> while not arrive:
...    print("Are we there yet?")
...    arrive = True
>>> print("We are here !")

>>> words = ['cat', 'window', 'defenestrate']
>>> for w in words:
...     print(w, len(w))
>>> for i in range(5):
...     print(i)
>>> for n in range(2, 10):
...     for x in range(2, n):
...         if n % x == 0:
...             print(n, 'equals', x, '*', n//x)
...             break
...     else:
...         print(n, 'is a prime number')
>>> for num in range(2, 10):
...     if num % 2 == 0:
...         print("Found an even number", num)
...         continue
...     print("Found a number", num)


Problem Solving
---------------
1. When should you choose to use ``while`` and ``for`` since both are looping methods?
2. What happens if we do not set ``arrive = True`` inside the ``while`` loop?
3. There are other Python built-in functions in the code example above. Can you identify them?
4. In the ``for`` loop example, ``words`` and ``range()`` are considered iterables. What are iterables? 
5. Can you give another examples of iterables?

Critical Thinking - Discussions
--------------------------------
Type some code examples below in IDLE. Some are good examples, some are not. Compare them and think about 

>>> food_list = ['bread', 'milk', 'eggs']
>>> i = 0
>>> while i < 3:
...   food = food_list[i]
...   print(food)
...   i += 1

>>> for food in food_list:
...   print(food)

>>> food_list = ['bread', 'milk', 'eggs']
>>> people = ['alice', 'bob', 'carol']
>>> for person, food in zip(people, food_list):
...   print(person + "likes " + food )

1. Which is a bad example ? Which is a good example?
2. Why is using ``in`` operator a better practice compared to using index (i.e. food_list[i]) ? 
3. What does ``zip()`` built-in function does here?


Best Practices
---------------
1. Use operators (i.e. ``is``, ``is not``, ``in``, ``not in``, ``and``, ``or``) to form readable condition when using ``while`` or ``for`` loop.
2. Use ``in`` operator to loop through iterables when using ``for`` loop. Do not use index, let Python handles it.
3. Make full use of Python built-in functions! Check them out at :ref:`Quick Resources <quick-resources_looping>`.

Remember
--------
1. Use ``while`` when you need to keep going until you figured out it's time to stop.
2. Use ``for`` when you know exactly how many times you need to loop.
3. Use ``continue`` to skip the rest of the body, and go on to the next iteration of the loop.
4. Use ``break`` to end the loop entirely, and move on with the program.

.. _quick-resources_looping:

Quick Resources
----------------
1. Python Flow Control - https://docs.python.org/3/tutorial/controlflow.html#
2. Python Compound Statements - https://docs.python.org/3/reference/compound_stmts.html#
3. Python Built-In Function - https://docs.python.org/3/library/functions.html
