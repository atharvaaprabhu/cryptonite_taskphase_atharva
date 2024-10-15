# storing command output

```bash
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out 
and submit it!
hacker@variables~storing-command-output:~$ echo %PWN
%PWN
hacker@variables~storing-command-output:~$ echo $PWN
pwn.college{sxk2X0BxhquDMy5x4n7Cgz9QHWg.dVzN0UDLzATN0czW}
```

used the first line and stored value of flag in variable PWN and then read the value of flag from the variable. (used the % sign by mistake).
