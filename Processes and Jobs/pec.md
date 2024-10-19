# process exit codes

```bash
hacker@processes~process-exit-codes:~$ touch /challenge/get-code
touch: cannot touch '/challenge/get-code': Permission denied
hacker@processes~process-exit-codes:~$ echo $?
1
hacker@processes~process-exit-codes:~$ /challenge.submit-code
ssh-entrypoint: /challenge.submit-code: No such file or directory
hacker@processes~process-exit-codes:~$ touch challenge/get-code
touch: cannot touch 'challenge/get-code': No such file or directory
hacker@processes~process-exit-codes:~$ touch get-code
hacker@processes~process-exit-codes:~$ /challenge/get-code 
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
93
hacker@processes~process-exit-codes:~$ /challenge/submit-code
You must run /challenge/submit-code with the exit code you retrieved from 
/challenge/get-code as the first argument:

Usage: /challenge/submit-code [EXIT_CODE]
hacker@processes~process-exit-codes:~$ /challenge/submit-code 93
CORRECT! Here is your flag:
pwn.college{w_axE9lT2dDikW-mTwrUokKiInn.dljN4UDLzATN0czW}
```

took some time to figure out which particular file i should touch before executing and finding the exit code. but once that was done i found the exit code using the $? command and executed /challenge/submit-code
