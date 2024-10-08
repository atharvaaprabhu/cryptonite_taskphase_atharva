# help for builtins

```bash
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!
    
    Options:
      --fortune		display a fortune
      --version		display the version
      --secret VALUE	prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "wc6x654G".
hacker@man~help-for-builtins:~$ /challenge/challenge --secret
ssh-entrypoint: /challenge/challenge: No such file or directory
hacker@man~help-for-builtins:~$ /challenge/challenge --secret wc6x654G
ssh-entrypoint: /challenge/challenge: No such file or directory
hacker@man~help-for-builtins:~$ challenge --secret wc6x654G
Correct! Here is your flag!
pwn.college{wc6x654GGcFHWQjohWMvT3xSkEk.dRTM5QDLzATN0czW}
```
