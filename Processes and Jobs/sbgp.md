# starting background processes

```bash
hacker@processes~starting-backgrounded-processes:~$ /challenge/run
You've started me in the foreground! You must start me in the background (by 
appending '&' to the command) to get the flag!
hacker@processes~starting-backgrounded-processes:~$ /challenge/run &
[1] 85



Yay, you started me in the background! Because of that, this text will probably 
overlap weirdly with the shell prompt, but you're used to that by now...

Anyways! Here is your flag!
pwn.college{ckMEZyk8ZqJvjtRmd8nc0btqzIN.dlDN4QDLzATN0czW}
```

executed the /challenge/run with an & sign at the end to run the command in the background and obtained the flag
