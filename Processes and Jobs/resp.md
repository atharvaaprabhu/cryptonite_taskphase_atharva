# resuming processes

```bash
hacker@processes~resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with 
the 'fg' command! Or just press Enter to quit me!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg
/challenge/run
I'm back! Here's your flag:
pwn.college{Iqw_Foh0lPhxpWMPh-KmEHgsKTG.dZDN4QDLzATN0czW}
Don't forget to press Enter to quit me!

Goodbye!
```

i executed the /challenge/run command and then suspended using ctrl z and then resumed it using fg to obtain the flag
