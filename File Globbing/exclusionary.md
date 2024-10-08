# exclusionary globbing

```bash
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run file_[!pwn]
Error: your argument is too long! It must be 8 characters or less.
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run
Error: you did not use a square bracket glob...
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run file_[^pwn]
Error: your argument is too long! It must be 8 characters or less.
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{QKsLp-l5urYC_0xShQ2OYjUPiX4.dZjM4QDLzATN0czW}
```
