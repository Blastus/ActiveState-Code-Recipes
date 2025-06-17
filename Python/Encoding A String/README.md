## [Encoding A String](https://code.activestate.com/recipes/440627-encoding-a-string)

**Originally published:** 2005-10-02 19:02:00

**Last updated:** 2005-10-02 19:02:00

**Author:** Stephen Chappell

**Recipe ID:** 440627

The main purpose of these functions are to allow encoding a string from base 256 to a special base 255. The function view the strings as numbers and simply change what base they are written in. This is not recommended for very long strings; otherwise, the encoding and deconding process can take a very long time to complete.
