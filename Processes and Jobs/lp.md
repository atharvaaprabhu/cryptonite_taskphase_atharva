# listing processes

```bash
hacker@processes~listing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 04:35 ?        00:00:00 /sbin/docker-init -- /nix/va
root           7       1  0 04:35 ?        00:00:00 /run/dojo/bin/sleep 6h
root          68       1  0 04:35 ?        00:00:00 /challenge/11680-run-2388
root          72      68  0 04:35 ?        00:00:00 sleep 6h
hacker        73       0  0 04:35 pts/0    00:00:00 /run/dojo/bin/ssh-entrypoint
hacker        90      73  0 04:39 pts/0    00:00:00 ps -ef
hacker@processes~listing-processes:~$ /challenge/11680-run-2388
Yahaha, you found me! Here is your flag:
pwn.college{4TIEEgHQwVCbqmhHozfXJwVfgEU.dhzM4QDLzATN0czW}
Now I will sleep for a while (so that you could find me with 'ps').
```

i used ps ef to read all the running programs and then saw the challenge/run program which had been renamed and executed it to obtain the flag.
