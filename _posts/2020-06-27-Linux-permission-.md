---
layout: post
title:  "Permissions in Linux"
date:   2020-06-27 16:16:45 +0300
categories: Linux
---

```
d rwx rwx rwx
```

1st `rwx` owner

2nd `rwx` group 

3rd `rwx` everybody else

`r` : Permission to read,    `w` : Permission to write,    `x` : Permission to executable,
 

There are some possible permission combinations we can change. Each combination has three digit of binary number. That three digit make an decimal number. Those numbers are 0 to 7.

```
---   000   0

--x   001   1

-w-   010   2

-wx   011   3

r--   100   4

r-x   101   5

rw-   110   6

rwx   111   7
```

We want to memorise only three combinations and decimal  numbers of those combinations. They are,

```
--x   001   1

-w-   010   2

r--   100   4
```

Then we can calculate others.

```
r--   +   -w-  +    --x = rwx
 4    +    2   +     1  =  7

r--   +   -w-   =   rw-
 4    +    2    =    6

r--   +   --x   =   r-x
 4    +    1    =    5 

-w-   +   --x   =   -wx
 2    +    1    =    3
```

There are one special permission. The permission to set the permission. It always belongs to the owner of the file.





















