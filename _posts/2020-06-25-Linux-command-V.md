---
layout: post
title:  "Linux Basic Commands - Part V"
date:   2020-06-25 22:14:45 +0300
categories: Linux
---

`vi (already exist file name)` : Go to the edit file. To begin edit we should command `i` or `I` or `o` or `O`

`i` edit begin from end

`I` edit begin from start

`o` edit begin from new line

`O` edit begin after leave one line space

When we finish editing we can click `esc`. After that we are in command mode. Then we should command `:wq` or `:qa!` or `:w`

`:wq` exit while saving

`:qa!` Exit without saving

`:w` save

When we are in command mode we can select text , copy that text and paste. `Shift + v` select (we can go with arrow keys).   Click `y` for copy and `p` for paste

`vi (new file name)` : Creating new file and start edit that file

`cat > file name` : Create a new file

`cat (file name)` : Displays  the file

`head (file name)` : Displays begin part of file 

`tail (file name)` : Displays end part of file

`head -5 (file name)` : Displays first 5 line of file

`less (file name)` : It displays file only screen limit

`echo $PATH` : Displays the contents of variables

`clear` : Clear the screen

`exit` : Exit the shell

`df -h` : Shows all the disk spaces in system

`uptime` : Uptime of my system

`hostname` : My host name

`uname` : What is the operating system

`man (command)` : Details about particular command










