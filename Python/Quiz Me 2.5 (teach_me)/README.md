## [Quiz Me 2.5 (teach_me)](https://code.activestate.com/recipes/577530-quiz-me-25-teach_me)

**Originally published:** 2010-12-31 21:55:42

**Last updated:** 2011-01-10 13:45:13

**Author:** Stephen Chappell

**Recipe ID:** 577530

Before discovering http://quizlet.com/, the following program was developed for running custom quizzes to help with studying for college courses. The program is not very advanced, but it works reasonably well for what it was designed to do. If the program were developed further, it would need greater capabilities than it currently has and would require a secondary system for actually creating the quizzes (currently, they are hand-typed). Quiz Me could be a starting point for anyone who wishes to actually write a program such as this and inspire others to write much better programs than what this recipe currently offers.

FAQ (Frequently Asked Questions) is used to generate events that power the quizzing process. The remaining classes represent the different event types. Enter and Exit instances are yielded when entering and exiting different tiers in the quiz structure. Reports are yielded after a tier has been completed and allow whoever is taking a test to review how well the questions have been answered per section, chapter, and complete quiz. Questions are randomly created and yielded and provide a way to easily answer from a list of choices. The Answer class extends the Question interface for getting more information when reviewing incorrectly answered questions.
