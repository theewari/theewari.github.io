---
layout: post
title:  "Understanding Linux Basic Commands - Part III"
date:   2020-06-25 16:41:45 +0300
categories: Linux
---

`mkdir (directory name)` : Creating a directory 

```
morty@c137:~$ mkdir newdir
morty@c137:~$ ls
bin      Documents  IdeaProjects  newdir    Public  Templates
Desktop  Downloads  Music         Pictures  snap    Videos
```

`mkdir (directory name)/(directory name)` : Creating sub directories

```
morty@c137:~$ mkdir newdir/subdir
morty@c137:~$ ls newdir
subdir
```

`mkdir -p newdir2/subdir2` : Creating another directories and sub directories if they do not already exist

```
morty@c137:~$ mkdir newdir2/subdir2
mkdir: cannot create directory ‘newdir2/subdir2’: No such file or directory
```
In that time we can command
```
morty@c137:~$ mkdir -p newdir2/subdir2
morty@c137:~$ ls newdir2
subdir2
```

`rmdir (directory name)` : Removing directory, but only empty directory

`rm -rf (directory name)` : Removing directory, empty or not
