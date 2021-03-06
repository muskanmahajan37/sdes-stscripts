------
Script
------



+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ Show the "Title" slide }}}                                                   | Hello friends and welcome to the tutorial on,                                    |
|                                                                                  | 'Getting started with TDD'                                                       |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ Show "Objectives" slide }}}                                                  | At the end of this tutorial, you will be able to,                                |
|                                                                                  |                                                                                  |
|                                                                                  |  1. Understand basics of Test Driven Development.                                |
|                                                                                  |  #. Understand the use test cases.                                               |
|                                                                                  |  #. Write simple tests for a function.                                           |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ Switch the "Pre-requisite" slide }}}                                         | Before beginning this tutorial, we would suggest you to complete the             |
|                                                                                  | tutorial on "Getting started with functions".                                    |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ show "What is TDD?" slide }}}                                                | Test-driven development is a software development process that relies on the     |
|                                                                                  | repetition of a very short development cycle.                                    |
|                                                                                  |                                                                                  |
|                                                                                  | The basics of Test Driven Development are,                                       |
|                                                                                  |                                                                                  |
|                                                                                  | 1. Decide the new feature you want to implement & the methodology to test it.    |
|                                                                                  | #. Write tests for the new feature decided upon.                                 |
|                                                                                  | #. Just write enough code so that the test can run, but, it fails.               |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ show "What is TDD?.." slide }}}                                              | #. Modify the code so that all the current tests & the previous tests pass.      |
|                                                                                  | #. Run tests to see if all the tests pass successfully.                          |
|                                                                                  | #. Refactor the code - optimize the algorithm, remove duplication &              |
|                                                                                  |    documentation, etc.                                                           |
|                                                                                  | #. And finally run the tests again to see if all the tests pass.                 |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ show "First test - fibonacci" slide }}}                                      | To illustrate TDD, lets take a simple program. Consider a function "fibonacci",  |
|                                                                                  | that takes one argument and returns the nth number of fibonacci series.          |
|                                                                                  | As shown in the example, c will contain the 3rd digit of the fibonacci series    |
|                                                                                  | that starts counting from 0(zero).                                               |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ show "Test Cases" slide }}}                                                  | To test any function it is important to have enough test cases & their expected  |
|                                                                                  | outputs before you start writing the test cases. Test cases are expected         |
|                                                                                  | outputs for a given set of inputs. So, to test fibonacci function,               |
|                                                                                  | we need test cases. As shown in this slide, our test cases are, when 'n=3', '2'  |
|                                                                                  | is the expected output from the fibonnaci series. Similarly, when 'n=4', '3'     |
|                                                                                  | is the expected output.                                                          |
|                                                                                  | Test cases can either be true or false depending on their actual behaviour       |
|                                                                                  | against the expected behaviour.                                                  |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ show "Test cases-Code" slide }}}                                             | The sample code for test cases is shown here. Observe that if any "if"           |
|                                                                                  | statement is executed, test aborts after printing the error message.             |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ show the "Stubs" slide }}}                                                   | Now, the fibonacci function is written just enough so that the tests can run.    |
|                                                                                  | But, obviously the tests are going to fail.                                      |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ show "fibonacci.py" slide }}}                                                | We will now combine the fibonnaci stub function we just wrote & the test cases   |
|                                                                                  | together in "fibonacci.py" file. Note that the test cases should be added        |
|                                                                                  | after "name=main" idiom.                                                         |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ show the "first run" slide }}}                                               | Now, let us run the fibonacci.py file. To do this, switch to the terminal &      |
| {{{ Run the fibonacci.py in terminal and show the error output & switch back to  | type "python fibonacci.py".                                                      |
| slide }}}                                                                        |                                                                                  |
| >>> python fibonacci.py                                                          |                                                                                  |
|                                                                                  | The tests fail as we just have a stub "fibonacci" function and no meaningful     |
|                                                                                  | code in it. Our next step is to write just minimum code to pass our tests.       |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ show "Fibonnaci" slide }}}                                                   | Modify the fibonacci stub function with given code & save the file. Now, switch  |
| {{{ switch to terminal }}}                                                       | to terminal and run it again as "python fibonacci.py".                           |
| >>> python fibonacci.py                                                          |                                                                                  |
|                                                                                  | {{{ pause }}}                                                                    |
|                                                                                  | Observe that, there will be no errors, as the test passes successfully.          |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ Show "Fibonacci - Recursive" slide }}}                                       | Finally, the same "fibonacci" function is modified to make it more readable      |
|                                                                                  | and easy to understand using recursion.                                          |
|                                                                                  | Pause this video here. Replace the "fibonacci" function with recursive one.      |
|                                                                                  | Run the modified "fibonacci.py" file. The test should pass again without any     |
|                                                                                  | errors. After successfully achieving this result, you can resume the video.      |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ show "Summary" slide }}}                                                     | This brings us to the end of the tutorial. In this tutorial,  we have learnt,    |
|                                                                                  |                                                                                  |
|                                                                                  |  1. The basic steps involved in Test driven development.                         |
|                                                                                  |  #. How to use test cases.                                                       |
|                                                                                  |  #. How to write simple tests for a function.                                    |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ show "Evaluation" slide }}}                                                  | Here are some self assessment questions for you to solve,                        |
|                                                                                  |                                                                                  |
|                                                                                  |  1. Design a TDD approach for a factorial function.                              |
|                                                                                  |  2. Design a TDD approach for an armstrong function.                             |
|                                                                                  |                                                                                  |
|                                                                                  | Try out the excercises for yourself & resume the video for solutions.            |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ show "Factorial" slide}}}                                                    | Given here is a TDD approach to a factorial function.                            |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ show "Armstrong" slide}}}                                                    | Given here is a TDD approach to an armstrong function.                           |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ Show the SDES & FOSSEE slide }}}                                             | Software Development techniques for Engineers and Scientists - SDES, is an       |
|                                                                                  | initiative by FOSSEE. For more information, please visit the given link.         |
|                                                                                  |                                                                                  |
|                                                                                  | Free and Open-source Software for Science and Engineering Education - FOSSEE, is |
|                                                                                  | based at IIT Bombay which is funded by MHRD as part of National Mission on       |
|                                                                                  | Education through ICT.                                                           |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ Show the ``About the Spoken Tutorial Project'' slide }}}                     | Watch the video available at the following link. It summarises the Spoken        |
|                                                                                  | Tutorial project.If you do not have good bandwidth, you can download and         |
|                                                                                  | watch it.                                                                        |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ Show the `` Spoken Tutorial Workshops'' slide }}}                            | The Spoken Tutorial Project Team conducts workshops using spoken tutorials,      |
|                                                                                  | gives certificates to those who pass an online test.                             |
|                                                                                  |                                                                                  |
|                                                                                  | For more details, contact contact@spoken-tutorial.org                            |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ Show the Acknowledgements slide }}}                                          | Spoken Tutorial Project is a part of the "Talk to a Teacher" project.            |
|                                                                                  | It is supported by the National Mission on Education through ICT, MHRD,          |
|                                                                                  | Government of India. More information on this mission is available at the        |
|                                                                                  | given link.                                                                      |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
| {{{ Show the Thankyou slide }}}                                                  | Hope you have enjoyed this tutorial and found it useful.                         |
|                                                                                  | Thank you!                                                                       |
+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
