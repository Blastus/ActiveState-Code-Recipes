## [dal_1.py](https://code.activestate.com/recipes/492209-dal_1py)

**Originally published:** 2006-04-26 09:45:27

**Last updated:** 2006-04-26 09:45:27

**Author:** Stephen Chappell

**Recipe ID:** 492209

The class presented bellow (Disk Abstraction
Layer 1) is designed to provide a very easy
interface to work with secondary memory
where IO errors may occur and data is
worked with in blocks. DAL1 allows access
to a hard drive (via its driver) so that
it can be accessed in a file-like way.
IO errors are also taken care of at this
level (which can cause problems at extremely
high probabilities of failure.
