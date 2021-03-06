# Changelog

### c1b10e0 Made platform detection portable (use of "uname -m"), updated README.md, added CHANGELOG.md

Replaced `uname -i` to `uname -m` in Makefile for platform detection, since
`uname -i` is not portable across Linux flavors. Also added CHANGELOG.md and
updated README.md. 

### ed4f557 Changed shell from /bin/sh to /bin/bash in all shell scripts

In legacy Linux versions, `/bin/sh` was a link to `/bin/bash`. Nowadays the
two shells differ. The shell scripts from AMD are in `bash` syntax and
therefore the change was necessary. 

### 219a078 Added patch for linux kernel version >= 4.15 Incorporates changes from `init_timer()` to `timer_setup()`

With kernel versions starting from 4.15, the interface for using timers was
changed.

### 97c3f18 Added disclaimer, description and installation instructions

### 7dd9d09 Initial commit
