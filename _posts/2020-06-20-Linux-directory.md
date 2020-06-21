---
layout: post
title:  "Linux directory structure"
date:   2020-06-20 22:30:45 +0300
categories: Linux
---

Directory structure explained here.

```
/                       : root of the file system
        bin             : binary program applications
        boot            : it contains everything that OS system need to boot
        dev             : devices, hardware
        etc             : system configuration files
        home            : use home
        lib             : libraries
        lost + found    : recovered files
        media           : mount point for removable media (cdrom)
        mnt             : mount point for temporary file system
        opt             : third party software (Applications that are not part of the base OS, can be installed in "/usr/local" or "/opt")
        srv             : data for the special provide by system
        tmp             : temporary storage space
        usr/            : unique system resource, user application source, image, etc..
            local       : app install for local user
            share       : configuration files, graphic for user files
            bin         : user command
            sbin        : essential system app
            lib         : shared library
        var/            : variable data use by system
            run         : information about current boot sesion
            lock        : lock files
            log         : log files
            tmp         : long term or large temporary files
```

`tree /` is command to get tree of root, `tree / -L 1` is command to get level 1 of root. just `tree` is command to get tree of your account.

```console
$ tree / -L 1
/
├── bin -> usr/bin
├── boot
├── cdrom
├── dev
├── etc
├── home
├── lib -> usr/lib
├── lib32 -> usr/lib32
├── lib64 -> usr/lib64
├── libx32 -> usr/libx32
├── lost+found
├── media
├── mnt
├── opt
├── proc
├── root
├── run
├── sbin -> usr/sbin
├── snap
├── srv
├── swapfile
├── sys
├── tmp
├── usr
└── var

24 directories, 1 file
```
