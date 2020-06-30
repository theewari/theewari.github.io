---
layout: post
title:  "useradd, adduser, addgroup, userdel"
date:   2020-06-30 14:23:45 +0300
categories: Linux
---


`useradd` : Create a new user or update default new user information. `useradd` is a low-level utility for adding users. On Debian, administrators should usually use `adduser`

`adduser` : Add a user to the system.

The only root user has permission to adding users.

```
morty@c137:~$ sudo adduser samar
Adding user `samar' …
Adding new group `samar' (1002) …
Adding new user `samar' (1002) with group `samar' …
Creating home directory `/home/samar' ...
Copying files from `/etc/skel' ...
New password:
Retype new password:
passwd: password updated successfully
Changing the user information for samar
Enter the new value, or press ENTER for the default
    Full Name []: samar
    Room Number []:
    Work Phone []:
    Home Phone []:
    Other []:
Is the information correct? [Y/n] y
morty@c137:~$ ls /home
morty  rick  samar
```

`sudo userdel` : Delete the users.

`sudo addgroup` : Add a group to the system.

```
morty@c137:~$ sudo addgroup beth
Adding group `beth' (GID 1003) ...
Done.
```

`sudo groupdel` : Delete the group.

`sudo usermod -G (group name) (user name)` : Add users to new group.

```
morty@c137:~$ sudo usermod -a -G beth samar
morty@c137:~$ cat /etc/group
beth:x:1003:samar
```

`passwd` : Change password. it's no argument required to the regular user to change password.

`sudo passwd (user name)` : Change the password of another user.


