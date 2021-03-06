.. Objectives
.. ----------
   
   .. At the end of this tutorial, you will be able to:
   
 .. Understand the use of persistent test cases.
 .. Write doctest and unittest for any given function.
 .. Understand the use of nosetest.

.. Prerequisites
.. -------------

..   1. Test driven development - Part 1

 
Script
------

.. L1

{{{ Show the  first slide containing the title, name of the production
team along with the logo of MHRD }}}

.. R1

Hello friends and Welcome to the tutorial on 
'Test driven development - Part 2'.

.. L2

{{{ Show slide with objectives }}} 

.. R2

At the end of this tutorial, you will be able to,

 1. Understand the use of persistent test cases.
 #. Write doctest and unittest for any given function.
 #. Understand the use of nosetest.

.. L3

{{{ Switch to the slide3, pre-requisite slide }}}

.. R3

Before beginning this tutorial,we suggest you to complete the 
tutorial on "Test driven development-part 1".

.. R4

To test ``fibonacci`` function, we have used two test cases.
It is inconvenient to repeatedly change the test conditions in
the fibonacci.py file. Each time a new test case is added, it
introduces an 'if' statement too.
So, it is a good practice to write the test cases in a separate file.
This file contains multiple lines, each line representing a test case.
Each line consists of two comma separated values in which the 
first column is the integer value that has to be passed to the function.
 The second column is the return value from the function.



.. L4

{{{ Switch to slide4 ,Persistent test cases, (after 3 seconds) show the
fibonacci_testcases.dat file}}}


.. R5

Let us open the fibonacci.py file which we have used in our 
previous tutorial. Now, change the code to use 'fibonacci_testcases.dat'
file for test cases.


.. L5

{{{ Switch to slide5, Modify fibonacci.py , show the modified
fibonacci.py file}}}

.. R6 

Save the fibonacci.py file. Switch to terminal and run 
``python fibonacci.py``. It should pass all the tests.


.. L6

{{{ Switch to terminal and run}}}
::

    python fibonacci.py

.. R7

So far we have used simple repetitive tests.
Now, let us see how ``Python testing frameworks`` does the
same job efficiently.
Python provides two frameworks for testing code: unittest and
doctest.

.. L7
 
{{{ Switch to slide6, Python testing framework }}}

.. R8

First, let us see how doctest works. 
A docstring is used to document function. Along with the 
description, interactive interpretor session's input and 
output are also added.
When executed, the doctest module picks up all such interactive 
examples, executes them and determines if the code runs
as documented.

.. L8

{{{switch to slide7 for 3 seconds and move to slide8,
 Doctest for fibonacci.py}}}

.. R9

To initiate doctest, we need to import the doctest module.
Testmod automatically picks all sample sessions, executes
them and compares with the documented output.
Doctest doesn't give any output when all the tests pass,
it complains only when any test fails.

.. L9

{{{ Switch to slide9, doctest for fibonacci.py }}}

.. R10

Let us run doctest by typing ``python fibonacci.py``.
As all tests pass, doctest doesn't give any output.
For detailed information, we may run the file with -v argument.
Run as ``python -v fibonacci.py``.

.. L10

{{{ Run the fibonacci.py in terminal .}}}
::
     
    python fibonacci.py
    python fibonacci.py -v

.. R11

So far we have seen doctest, which is simple to use. But when
it comes to automate the process, unittest is better.
Unittest initializes code and data, it aggregates 
tests into collections and improves reporting.

.. L11

{{{ Switch to slide-11(stay for 5 seconds) and switch to slide 12 }}}

   
.. R12

To run unittest on our fibonacci function let us create a
new file ``test_fibonacci.py``. This new file will host the
test code.
To begin unittesting let us subclass the TestCase class 
in unittest. We need fibonacci.py and fibonacci_testcases.py
files too.


.. L12

{{{ Show slide13(stay for 3 seconds) and switch to slide14 }}}


.. R13

The ``setUp`` function will read all the test data and store
it in a list test_cases. The ``test_fibonacci`` function 
consists the actual test code. And the third  function ``tearDown``
deletes the data from test_cases 
and closes ``fibonacci_testcases.dat`` file.

.. L13

{{{ Show slide 15, test_fibonacci.py }}}


.. R14

Individual unittests and doctests may not be fiseable to use when
multiple files are to be tested. For this purpose we have a python
utility called Nose. Nose test aggregates unittests and doctests. Nose
test utility can be installed by using the following command 
``$ easy_install nose``. It can be run by issuing the command ``$ nosetests``
in the root level of the directory containing all your python files to be tested.

.. L14

{{{ Show slide15(for 5 seconds), nose tests }}}

{{{ Follow the commands in terminal. }}}

::

    $ easy_install nose
    $ nosetests
    
.. R15    


This brings us to the end of the tutorial.In this tutorial,
we have learnt to,
 
 1. Understand the basic steps involved in Test driven development.
 #. Design a Test driven approach for a given ``fibonacci`` function.


.. L15

{{{ switch to slide-17,Summary }}}

.. R16

Here are some self assessment questions for you to solve
 1.

 2. 

.. L16

{{{ switch to slide-18, Evaluation }}}

.. R17

And the answers are,
 1.

 2.

.. L17

{{{ switch to slide-19 ,Solutions}}}

.. R18

Hope you have enjoyed this tutorial and found it useful.
Thank you!

.. L18

{{{ Switch to slide-20, Thank you}}}

