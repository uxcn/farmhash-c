# farmhash-c #

C99 translation of Geoff Pike's and Jyrki Alakuijala's FarmHash.

### some notes... ###

This version of FarmHash is translated from the code available via
[github](https://github.com/google/farmhash) (1.1).  For quality and performance
metrics, please see Reini Urban's [smhasher](https://github.com/rurban/smhasher)
fork.

The code is meant to be platform agnostic, excluding some compiler intrinsics.
Note, `byte swap` and `rotate right` are used.  I've confirmed the included
versions optimize correctly with x86 and Clang (3.7), however there may be
platforms or compilers they don't optimize correctly on.
