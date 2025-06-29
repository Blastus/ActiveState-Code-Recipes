## [Expression Evaluator](https://code.activestate.com/recipes/576790-expression-evaluator)

**Originally published:** 2009-06-02 12:01:47

**Last updated:** 2009-06-02 23:57:44

**Author:** Stephen Chappell

**Recipe ID:** 576790

After reading a portion of the book "The C# Programming Language: Third Edition," I found a section in the introduction that introduced abstract classes and methods that involved an example that included the concept of expression trees. The code was easy to implement since it just had to be copied out of the book. After playing around with the program a little and extending it, I thought that it would be fun to write a program in C# that could (interactively) evaluate expressions and display the results. Not knowing C# quite as well as Python led to the following program written and tested in Python 3.0 (not sure about previous languages).

The first section of the code includes  port of the program from the aforementioned book along with extra code that allows for further features not originally included in the C# version. Those sections are clearly marked as being new code written by yours truly. The second area of the program has six functions that are profusely documented so as to explain how they go about parsing and processing expressions entered for evaluation. For those wishing to use the code, the "run" function should be all that you need. The final part of the module contains a test program that can be used to check the validity of the how well the program works.

The parser is not very complicated and will except expressions that are both normal to Python and completely illegal in Python. The main features are its ability to (1) identify simple assignment and mathematical operations, (2) identify constant floating point numbers, and (3) identify variables that would otherwise have no  other meaning to the program. A limited number of error messages are given when appropriate but may leave one guessing what the problem really is. Mathematical operations are evaluated from left to right without regards to precedence, and assignment statements are evaluated from right to left.
