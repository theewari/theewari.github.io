---
layout: post
title:  "chmod, chgrp, chown"
date:   2020-06-27 17:56:45 +0300
categories: Linux
---

`chmod` : Change mode. It can change user, group and others current permission mode to required permission mode. It can do from two different ways.

I. `chmod  (required party) + (required permission)  file name`

   `chmod  (required party) - (required permission)  file name`
  
required party, like, 
                     
```
u : user 

g : group
                     
o : others
```

required permission like,

```
r : read

w : write

x : executable
```

```
morty@c137:~/newdir/subdir$ ls -l
-rw------- 1 morty morty 43 May 27 19:45 everyone-rw
morty@c137:~/newdir/subdir$ chmod go+rw everyone-rw
morty@c137:~/newdir/subdir$ ls -l
-rw-rw-rw- 1 morty morty 43 May 27 19:45 everyone-rw
```

II. `chmod (decimal number of permissions)  file name`

```
morty@c137:~/newdir/subdir$ ls -l
-rw------- 1 morty morty 43 May 27 19:45 everyone-rw
morty@c137:~/newdir/subdir$ chmod 666 everyone-rw
morty@c137:~/newdir/subdir$ ls -l
-rw-rw-rw- 1 morty morty 43 May 27 19:45 everyone-rw
```

`chgrp` : Change the group.

There is a command `id -Gn` to know what are the groups that we are in. 

```
morty@c137:~$ id -Gn
morty sudo
```    

`chgrp (new group name) file name`

```
morty@c137:~/newdir/subdir$ ls -l
-rw-r----- 1 morty morty 52 May 27 19:53 group-r-only
    morty@c137:~/newdir/subdir$ chgrp sudo group-r-only
    morty@c137:~/newdir/subdir$ ls -l
    -rw-r----- 1 morty sudo  52 May 27 19:53 group-r-only
```

`chown` : Change the owner of the file, we have not permission to change the owner. only root have permission to change owner. Now we have to do sudo commands with `chown`
    
```
sudo chown (new owner name) file name
```

```
morty@c137:~/newdir/subdir$ ls -l
-rw-rw-rw- 1 morty morty 43 May 27 19:45 everyone-rw
morty@c137:~/newdir/subdir$ sudo chown nobody everyone-rw
[sudo] password for morty:
morty@c137:~/newdir/subdir$ ls -l
    -rw-rw-rw- 1 nobody morty 43 May 27 19:45 everyone-rw
```

















