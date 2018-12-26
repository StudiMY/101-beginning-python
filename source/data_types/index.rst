===========
Data Types
===========
The Bigger Picture
-------------------
As you know, everything in a computer is represented as **1s and 0s**. If you are not sure how computer works, 
we highly recommend you to watch `this interactive video <https://www.khanacademy.org/computing/computer-science/how-computers-work2/v/khan-academy-and-codeorg-binary-data>`_.

In this topic, we explore **why we need Data Types**. Key question is, if a computer only 
understands binary (1s and 0s), how does a human communicates with it? 

Syntax and Semantics - Learning Python Grammar
----------------------------------------------
Explore on your own for 5 mins on the different data types in Python using ``type()`` built-in function. 

Open up Python IDLE and type away. 

>>> type(10)
<class 'int'>
>>> type("hello world")
<class 'str'>
>>> type(2.13)
<class 'float'>
>>> type(None)
<class 'NoneType'>
>>> type(True)
<class 'bool'>

Problem Solving
---------------
Now try this in IDLE.

>>> num1 = "1"
>>> num2 = "2"
>>> num1 + num2
>>> num1 + 2

1. What is the value of ``num1`` and ``num2`` ? 
2. What happens if you type ``num1`` + ``num2`` ?
3. What happens if you type ``num1`` + 2 ? Why ? 
4. How do you perform math operations on ``num1`` and ``num2`` to produce number 3 ? Try it !

.. topic:: FAQ / Common Issues

    | 1. Help ! I got bunch of errors typing stuff inside ``type()`` built-in function.  
    | It's okay! Try to read and make sense the errors shown. Part of learning is to learn how to read error stack.
    
    | 2. How can I possibly know all the built-in functions and data types in Python?  
    | Refer to :ref:`Quick Resources <quick-resources>` for all the built-in functions and data types available in Python.

Critical Thinking - Discussions
--------------------------------
1. What other types you found besides the common ``int``, ``float``, ``str``, ``bool``, ``None`` type ? 
2. Can you type in Chinese or other languages ? What type is it?
3. If everything in computer is represented by 1s and 0s, how does it represent:-
    
   * 10
   * 3.1243
   * "hello world"
   * "你好"
4. Can you imagine how images, files, sounds and other inputs get represented in Python?
5. Can you appreciate the value of having data types now ? 
6. Can you think of other data types which needs to be represented ?

.. topic:: Fun Facts

    Variables ``num1`` and ``num2`` above are intuitive to us cause we learnt them in Math class. It's simple algebra!

Best Practices
---------------
1. You might already notice by now Python has its documentation stored at https://docs.python.org/3/

Remember
--------
1. Data types help to represent numbers, strings, etc in human readable manner so we can communicate with the machine. In other words, data types is an **interface between human and machine**. 
2. Full list of all Python types are documented. Refer to :ref:`Quick Resources <quick-resources>`  

.. _quick-resources:

Quick Resources
----------------
1. Full list of Python built-in standard data types - https://docs.python.org/3/library/stdtypes.html
2. Full list of Python built-in specialized data types - https://docs.python.org/3/library/datatypes.html
3. Full list of Python built-in functions - https://docs.python.org/3/library/functions.html
