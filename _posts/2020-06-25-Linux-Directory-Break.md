---
layout: post
title:  "Understanding Details Of Directories"
date:   2020-06-25 13:20:45 +0300
categories: Linux
---

Let's break down details of directories.

```
drwxr-xr-x 2 morty morty 4096 May 17 20:48 Desktop

drwxr-xr-x    - file type and accerce permission
2             - memory block
morty         - owner of file
morty         - user group
4096          - size(bites)
May 17 20:48  - date and time
Desktop       - directory or file name
```

`drwxr-xr-x 2 morty morty 4096 May 17 20:48 Desktop` 
`d` : is for directory

`-rw-rw-r-- 2 morty morty 1147 May 24 12:51 test`
`-` : is for regular files. Like test file, compiled program, video anything

`lrwxrwxrwx 1 morty morty    4 May 25 14:41 test2 -> test`
`l` : is for soft link




