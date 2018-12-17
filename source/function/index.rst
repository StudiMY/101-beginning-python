=========
Functions
=========
The Bigger Picture
------------------
Problem solving is about **breaking down problem into mind-size bites** - decomposing. Function allows us to essentially do 
just that - divide the code into smaller chunks. What comes to mind when it comes to ``functions`` ? Hint: You 
learn it in school! 

.. topic:: Functions in Math

    .. image:: images/function_in_math.png


Syntax and Semantics - Learning Python Grammar
----------------------------------------------
Explore on your own for 5 mins on how to create functions. Pay attention to the indentation and syntax.

Open up Python IDLE and type away. 

>>> nyc = 75
>>> sf = 61
>>> london = 59

>>> print("Temperature in NYC is {}ªF".format(nyc))
>>> print("Temperature in NYC is {}ªC".format((nyc - 32) * 5/9 ))
>>> print("Temperature in SF is {}ªF".format(sf))
>>> print("Temperature in SF is {}ªC".format((sf - 32) * 5/9 ))
>>> print("Temperature in London is {}ªF".format(london))
>>> print("Temperature in London is {}ªC".format((london - 32) * 5/9 ))

>>> def to_celsius(temp_fahrenheit):
>>> ... return (temp_fahrenheit - 32) * 5/9

>>> print("Temperature in NYC is {}ªF".format(nyc))
>>> print("Temperature in NYC is {}ªC".format(to_celsius(nyc)))
>>> print("Temperature in SF is {}ªF".format(sf))
>>> print("Temperature in SF is {}ªC".format(to_celsius(sf)))
>>> print("Temperature in London is {}ªF".format(london))
>>> print("Temperature in London is {}ªC".format(to_celsius(london)))

Critical Thinking - Discussions
-------------------------------
1. What is the problem of using the approach before creating ``to_celcius`` function?
2. Can you think of some reasons how ``to_celcius`` is better?
3. Did you notice how do we call a function?
4. What is the parameter or argument being passed to the ``to_celcius()`` function?
5. What does ``to_celcius()`` function returns?
6. ``print()`` is also a function, a built-in function from Python. Now, what does it return?
7. Have you thought of how function is represented in binaries? Hmmm...

Problem Solving
---------------
Recall **mutable vs immutable** in `variable_statement_expression` topic? Here, we will explore a little more on 
how it behaves when passed to a function.

**Warning**: This can be confusing. It's considered as advanced topic.

>>> def mutable_argument_func(a_list):
>>> ... a_list.append(42)
>>> ... print(a_list) 

>>> answer_list = []
>>> mutable_argument_func(answer_list)
>>> print(answer_list) 

>>> def immutable_argument_func(a_string):
>>> ... a_string = 'new value'
>>> ... print (a_string)

>>> answer_string = 'old value'
>>> immutable_argument_func(answer_string)
>>> print(answer_string)

1. What is the result of ``print(a_list)`` and ``print(answer_list)`` ?
2. What is the result of ``print(a_string)`` and ``print(answer_string)`` ?
3. How does this help you to understand the behaviour between mutable vs immutable argument when it's passed to a function ? 

Best Practices
--------------
1. Give meaningful name for a function. For example, ``to_celsius()`` is very intuitive. 
2. Refer to :ref:`Quick Resources <quick-resources-functions>` for function name and arguments good practices.

Remember
--------
1. Function is like a **mini program within a program**.
2. It allows us to:-

   * Reuse Code
   * Abstract Functionality
   * Divide code (Think in smaller chunks)
   * Encapsulate
   * Make our code easier to test
3. Python rules (semantics):-

   * Create function with ``def`` keyword, followed by function name and colon(``:``)
   * Call functions using parentheses () and passing zero or more arguments / parameters
   * Optional - assign return values to a variable with ``return`` keyword.
4. Be mindful of the indentation!

.. _quick-resources-functions:

Quick Resources
---------------
1. Python built-in functions - https://docs.python.org/3/library/functions.html
2. Function Definition - https://docs.python.org/3/reference/compound_stmts.html#function
3. PEP 8: Function and Variable Names - https://www.python.org/dev/peps/pep-0008/#function-and-variable-names
4. PEP 8: Function and Method Arguments - https://www.python.org/dev/peps/pep-0008/#function-and-method-arguments