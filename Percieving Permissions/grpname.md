# fun with group names

```bash
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp26414) groups=1000(grp26414)
hacker@permissions~fun-with-groups-names:~$ ls -l
total 28
-rw-r--r-- 1 hacker grp26414   4 Oct  9 13:15 COLLEGE
-rw-r--r-- 1 hacker grp26414   8 Oct  9 13:44 PWN
-rw-r--r-- 1 root   grp26414  58 Oct  4 16:21 a
-rw-r--r-- 1 hacker grp26414   0 Oct 19 04:26 get-code
-rw-r--r-- 1 hacker grp26414 829 Oct  9 13:35 instructions
-rw-r--r-- 1 hacker grp26414  93 Oct  9 13:35 myflag
lrwxrwxrwx 1 hacker grp26414   5 Oct  9 17:26 not-the-flag -> /flag
-rw-r--r-- 1 root   grp26414  77 Oct  9 13:52 output.txt
-rw-r--r-- 1 hacker grp26414 435 Oct  9 13:25 the-flag
hacker@permissions~fun-with-groups-names:~$ chgrp 1000 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{sztwiZ2bMVBOc7gTQfci1BkwPYH.dJzNyUDLzATN0czW}
```

used id to see available groups and then used ls to find list of files, saw that /flag was part of group 26414 and then i changed my group using its group if and used cat to read the file and obtain the flag
