# changing file ownership

```bash
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ ls -l
total 28
-rw-r--r-- 1 hacker hacker   4 Oct  9 13:15 COLLEGE
-rw-r--r-- 1 hacker hacker   8 Oct  9 13:44 PWN
-rw-r--r-- 1 root   hacker  58 Oct  4 16:21 a
-rw-r--r-- 1 hacker hacker   0 Oct 19 04:26 get-code
-rw-r--r-- 1 hacker hacker 829 Oct  9 13:35 instructions
-rw-r--r-- 1 hacker hacker  93 Oct  9 13:35 myflag
lrwxrwxrwx 1 hacker hacker   5 Oct  9 17:26 not-the-flag -> /flag
-rw-r--r-- 1 root   hacker  77 Oct  9 13:52 output.txt
-rw-r--r-- 1 hacker hacker 435 Oct  9 13:25 the-flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{ckEvXEHuEF3D5_ZQ0DPPg8L9tQG.dFTM2QDLzATN0czW}
```
i used the chown to change ownership of the file and used ls to list out all files and used cat to read the flag file and obtain the flag.
