# adding commands
```bash
hacker@path~adding-commands:~$ cd windir
hacker@path~adding-commands:~/windir$ ls
win
hacker@path~adding-commands:~/windir$ nano
hacker@path~adding-commands:~/windir$ nano win
hacker@path~adding-commands:~/windir$ echo $PATH
/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
hacker@path~adding-commands:~/windir$ PATH="/usr/bin:/home/hacker/windir
> chmod +x win
> /challenge/run
> 
> ^C
hacker@path~adding-commands:~/windir$ PATH="/usr/bin:/home/hacker/windir"
hacker@path~adding-commands:~/windir$ chmod +x win
hacker@path~adding-commands:~/windir$ /challenge/run
Invoking 'win'....
pwn.college{ALPAfFtG2Zs3hAfpS_pItM4C_nG.dZzNyUDLzATN0czW}
```
first i used cd to change my working directory to windir, as windir had already been created from a previous execution. then i used nano to add cat /flag into the file.
then i used echo $PATH to find out where cat was saved. then i saw that cat was in /usr/bin so i set the path as "/usr/bin:/home/hacker/windir".
i used chmod +x to make the file executable and then executed /challenge/run and obtained the flag.

this question was infact quite tricky and took me quite a while to solve as well as some assistance from a few friends.
