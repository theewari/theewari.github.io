---
layout: post
title:  "Understanding Linux Basic Commands - Part I"
date:   2020-06-22 11:23:45 +0300
categories: Linux
---

Basic commands in Linux.


`pwd` : It shows present working directory 


```
morty@c137:~$ pwd
/home/morty
```


`cd` , `cd ~` : Change current directory to your home directory

```
morty@c137:~/Documents$ cd
morty@c137:~$
```

```
morty@c137:~/Documents$ cd ~
morty@c137:~$
```

`cd /` : Change current directory to root directory

```
morty@c137:~$ cd /
morty@c137:/$
```

`cd /(directory name)` : Change your current directory to naming directory in root

```
morty@c137:~$ cd /home
morty@c137:/home$
```

`cd (directory name)` : Change current directory to naming directory in your account
     
```
 morty@c137:~$ cd Documents
 morty@c137:~/Documents$
 ```

`cd (directory name)/(directory name)` : Navigating through multiple directories

```
morty@c137:~$ cd Pictures/Wallpapers
morty@c137:~/Pictures/Wallpapers$
```

`cd ..` : Moving up one directory level

```
morty@c137:~/Pictures/Wallpapers$ cd ..
morty@c137:~/Pictures$ cd ..
morty@c137:~$
```

`cd .` : Current directory level

```
morty@c137:~$ cd Pictures/Wallpapers
morty@c137:~/Pictures/Wallpapers$ cd ..
morty@c137:~/Pictures$ cd .
morty@c137:~/Pictures$
```




