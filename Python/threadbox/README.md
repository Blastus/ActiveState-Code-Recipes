## [threadbox.py](https://code.activestate.com/recipes/578152-threadboxpy)

**Originally published:** 2012-06-05 02:42:37

**Last updated:** 2012-10-09 22:40:09

**Author:** Stephen Chappell

**Recipe ID:** 578152

Provide a way to run instance methods on a single thread.

This module allows hierarchical classes to be cloned so that their instances
run on one thread. Method calls are automatically routed through a special
execution engine. This is helpful when building thread-safe GUI code.
