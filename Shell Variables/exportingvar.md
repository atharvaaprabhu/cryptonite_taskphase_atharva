# exporting variables

```bash
hacker@variables~exporting-variables:~$ PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ export PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ sh
sh-5.2$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great 
job! Here is your flag:
pwn.college{MSFUfl-xVW3Gc9a3HepJ_J9H0cT.dJjN1QDLzATN0czW}
```

i assigned both variables :PWN and COLLEGE, their respective values. then i exported PWN using 'export' command and changed shell using sh and ran /challenge/run to obtain the flag
