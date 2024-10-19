# killing processes

```bash
hacker@processes~killing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 03:54 ?        00:00:00 /sbin/docker-init -- /nix/va
root           7       1  0 03:54 ?        00:00:00 /run/dojo/bin/sleep 6h
root          71       1  0 03:54 ?        00:00:00 su -c /challenge/.launcher h
hacker        73      71  0 03:54 ?        00:00:00 /challenge/dont_run
hacker        74      73  0 03:54 ?        00:00:00 sleep 6h
hacker        75       0  0 03:54 pts/0    00:00:00 /run/dojo/bin/ssh-entrypoint
hacker        94      75  0 03:55 pts/0    00:00:00 ps -ef
hacker@processes~killing-processes:~$ kill 73
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{o-m4f6-DJD4gGkPvIOn3awXBANW.dJDN4QDLzATN0czW}
```

i used the ps -ef command to find all running programs and located the pid of /dont_run and then used the kill to terminate that particular program and executed /challenge/run
