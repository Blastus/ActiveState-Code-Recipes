## [Quiz Me 2.5 (quizcore)](https://code.activestate.com/recipes/577528-quiz-me-25-quizcore)

**Originally published:** 2010-12-31 21:53:01

**Last updated:** 2011-01-10 03:55:11

**Author:** Stephen Chappell

**Recipe ID:** 577528

Before discovering http://quizlet.com/, the following program was developed for running custom quizzes to help with studying for college courses. The program is not very advanced, but it works reasonably well for what it was designed to do. If the program were developed further, it would need greater capabilities than it currently has and would require a secondary system for actually creating the quizzes (currently, they are hand-typed). Quiz Me could be a starting point for anyone who wishes to actually write a program such as this and inspire others to write much better programs than what this recipe currently offers.

The classes in this module take a XML node tree of a test/quiz bank and converts it into a definite, usable structure for creating a collection of question and answers that can be asked from different categories. UnitTest, Chapter, and Section represent divisions of a book (such as from history) and specify several different (inflexible) tiers in which questions may be placed. The Category function automatically determines what types of questions are being asked and creates appropriate objects that contain Fact objects from which Questions and Answers are generated. True_Or_False, Multiple_Choice, and Matching questions types are supported.
