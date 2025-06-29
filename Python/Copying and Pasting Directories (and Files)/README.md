## [Copying and Pasting Directories (and Files)](https://code.activestate.com/recipes/440626-copying-and-pasting-directories-and-files)

**Originally published:** 2005-10-02 18:54:25

**Last updated:** 2005-10-02 18:54:25

**Author:** Stephen Chappell

**Recipe ID:** 440626

Here are a few basic fuctions that allow someone to copy a directory (along with its files and sub-directories) and paste it somewhere else. They ignore links and anything else that is not a directory or a file. The data returned from copy_dir()  is in a format that paste_dir() can understand. A design note: what you get back from copy_dir() may be different whether or not you have a path separator at the end of the path; paste_dir() makes use of that feature (whether or not you want the first folder to be created). The fuctions can easily be modified to not include sub-directories in the returned package, and errors caused by accessing to files or directories can also be ignored with some simple editting. Also, note the asserts in the functions; these functions are designed to crash hard so that the calling code has to take care of the errors.
