# suspending processes

```bash
/challenge/run
I'll only give you the flag if there's already another copy of me running in 
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root          82      65  0 04:01 pts/0    00:00:00 bash /challenge/run
root          84      82  0 04:01 pts/0    00:00:00 ps -f

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can 
background me with Ctrl-Z or, if you're not ready to do that for whatever 
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in 
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root          82      65  0 04:01 pts/0    00:00:00 bash /challenge/run
root          89      65  0 04:02 pts/0    00:00:00 bash /challenge/run
root          91      89  0 04:02 pts/0    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{41Q1JuU7nl2lgyatvRcqddzDm9V.dVDN4QDLzATN0czW}
```

i executed the /challenge/run command and then suspended using ctrl z and then executed the same program again, obtaining the flag
