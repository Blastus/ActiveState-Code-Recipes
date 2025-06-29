## [Quiz Me 2.5 (XML example)](https://code.activestate.com/recipes/577541-quiz-me-25-xml-example)

**Originally published:** 2011-01-11 00:36:56

**Last updated:** 2011-01-11 00:51:24

**Author:** Stephen Chappell

**Recipe ID:** 577541

Before discovering http://quizlet.com/, the following program was developed for running custom quizzes to help with studying for college courses. The program is not very advanced, but it works reasonably well for what it was designed to do. If the program were developed further, it would need greater capabilities than it currently has and would require a secondary system for actually creating the quizzes (currently, they are hand-typed). Quiz Me could be a starting point for anyone who wishes to actually write a program such as this and inspire others to write much better programs than what this recipe currently offers.

This is an example testbank file for Quiz Me. The questions and answers were created from a book used in a "HI 101" college class. What is presented here is a small sample of what would more likely be a much larger bank of question and answers used for automated quizzing or testing purposes. The XML shown here is formatted correctly dictated by an unwritten specification that the testbank (parsing) module requires. It is the quizcore module that takes the data through its final transformation and also builds questions and answers based on the material available. Once the .build() method has been called on classes inheriting from the _Category class, public attributes (QnA) become available on the _Category objects containing enough information for asking questions with provided answers. Fact objects also have .build() methods; once called, public Q2A and A2Q attributes can be used to find valid mappings of questions to answers and answers to questions.
