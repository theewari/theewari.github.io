---
layout: post
title:  "Soft Link and Hard Links in Linux"
date:   2020-06-26 12:14:45 +0300
categories: Linux
---

`ln -s` : Soft link

Let's make soft link to the `test` as `test2`

```
morty@c137:~$ ln -s test test2
morty@c137:~$ ls -i
 2759545 test2        2759449 test   
```

1.  Does depend on original file

2.  Soft link has a different inode from inode of original 

3.  Linking file to directory

4.  Linking exist file to new file

5.  Linking between different  file system

6.  Linking a directory to another directory  



`ln` : Hard link

Let's make hard link to the `test` as `test3`

```
morty@c137:~$ ln test test3
morty@c137:~$ ls -i
2759545 test2   2759449 test3   2759449 test                 
 ```
       
1.  Doesn't depend on original file

2.  Hard link has a same inode to the inode of original

3.  Linking file to directory

4.  Linking exist file to new file

5.  Linking in same file system

6.  Hard link can't link directory




