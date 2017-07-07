# oldfiles

    A bash script that helps "find" files of certain age, and explains the "find" command it uses!

# How to use

oldfiles - Find files by time

Usage:

`   [-v...] ([-h|-V|-n] | {[(-a|-u) | (-m|-t) | -c] (-i | -d | -o| -y | -g) N (-\> | -\< | -\=) [-p "pat"]} )`

### Options:

```
Help & Info:
    -h, --help       Show this help.
    -V, --version    Show version.
    -v, --verbose    Turn verbose mode on (cumulative).
    -n, --dry-run    Do not run, just explain how to create a "find" command
Time type (access/use, modification time or changed status):
    -a or -u        access time (or use time)
    -m or -t        modification time (default)
    -c              status change
Time range (where N is a positive integer):
    -i N            minutes (default, with N equal 1 min)
    -d N            days
    -o N            months
    -y N            years
    -g N            N is a DATE (example: "2017-07-06 22:17:15")
Tests:
    -p "pat"        optional pattern to match (example: -p "*.c" to find c files) (default -p "*")
    -\>             file is newer than given range, ie, time modified after it.
    -\<             file is older than given range, ie, time is from before it. (default)
    -\=             file that is exactly N (min, day, month, year) old.
```

### Exit status:

```
    0, if ok.
    1, some error occurred.
```

### Author:

```
(C) Copyright 2017 by Ruben Carlo Benante <rcb@beco.cc>
Date: 2017-07-07
```

