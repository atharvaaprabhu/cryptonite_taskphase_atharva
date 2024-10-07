# making directories

```bash
hacker@commands~making-directories:~$ cd /tmp
hacker@commands~making-directories:/tmp$ /pwn
ssh-entrypoint: /pwn: No such file or directory
hacker@commands~making-directories:/tmp$ mkdir pwn
hacker@commands~making-directories:/tmp$ /pwn
ssh-entrypoint: /pwn: No such file or directory
hacker@commands~making-directories:/tmp$ cd /pwn
ssh-entrypoint: cd: /pwn: No such file or directory
hacker@commands~making-directories:/tmp$ cd /tmp/pwn
hacker@commands~making-directories:/tmp/pwn$ touch college
hacker@commands~making-directories:/tmp/pwn$ /challenge/run
Success! Here is your flag:
pwn.college{4-NtGue2E5M5DPhLQqXBIy5_273.dFzM4QDLzATN0czW}
```
