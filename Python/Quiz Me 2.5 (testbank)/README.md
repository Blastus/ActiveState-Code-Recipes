## [Quiz Me 2.5 (testbank)](https://code.activestate.com/recipes/577531-quiz-me-25-testbank)

**Originally published:** 2010-12-31 21:57:11

**Last updated:** 2011-01-11 00:28:15

**Author:** Stephen Chappell

**Recipe ID:** 577531

Before discovering http://quizlet.com/, the following program was developed for running custom quizzes to help with studying for college courses. The program is not very advanced, but it works reasonably well for what it was designed to do. If the program were developed further, it would need greater capabilities than it currently has and would require a secondary system for actually creating the quizzes (currently, they are hand-typed). Quiz Me could be a starting point for anyone who wishes to actually write a program such as this and inspire others to write much better programs than what this recipe currently offers.

Quizes are stored as XML files and must be parsed and processed for use within the Quiz Me application. BankParser acts as a ContentHandler when used in parsing one of these XML files. It builds a tree of _Nodes, extracts attributes and textual data as needed, and validates the structure of the quiz bank data stream. _Nodes act as an abstract representation of XML elements and have the capability of reconstructing the relevant part of the XML that they encapsulate. Several classes follow that inherit from the _Node class and specify an attribute that node is expected to contain. The parse function takes a filename and returns a TestBank root object if parsing and validation were successful at this stage of a quiz's loading sequence.
