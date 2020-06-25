---
layout: post
title:  "Understanding Linux Basic Commands - Part IV"
date:   2020-06-25 19:08:45 +0300
categories: Linux
---

`touch (directory name/directory name)/(file name)` : Creating file.

```
morty@c137:~$ touch newdir/subdir/testfile
morty@c137:~$ ls newdir/subdir
testfile
```

`touch file name{1..10}` : Creating files how much we want in current directory.

```
morty@c137:~/newdir/subdir$ touch testfile{1..5}
morty@c137:~/newdir/subdir$ ls
testfile1  testfile2  testfile3  testfile4  testfile5
```

`rm (directory name/directory name)/(file name)` : Removing file.

`rm -i (directory name/directory name)/(file name)` : Request permission before remove the file.in that time we should command `y`

```
morty@c137:~$ rm -i newdir/subdir/testfile
rm: remove regular empty file 'newdir/subdir/testfile'? y
morty@c137:~$ ls newdir/subdir
morty@c137:~$
```

rm -i *
    Removing all files from the current directory, but ask for the permission one by one.
    morty@c137:~/newdir/subdir$ rm -i *
rm: remove regular empty file 'testfile1'? y
rm: remove regular empty file 'testfile2'? y
rm: remove regular empty file 'testfile3'? y
rm: remove regular empty file 'testfile4'? y
rm: remove regular empty file 'testfile5'? y
morty@c137:~/newdir/subdir$

`mv rm -f *` : Removing all files from the current directory without asking.

`mv (directory or file name) (new location)` : Moving file from current location to naming location.

`mv (path to new location) (file or directory name)` : Move back to previous place.

`mv (path to new location) . ` : Move back to previous place.

`/(new location) mv (directory or file name) ../` : Move back to previous place.

`mv (directory name or file name) (new name)` : Rename file.



















