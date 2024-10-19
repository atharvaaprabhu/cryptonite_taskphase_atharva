# becoming root with su

```bash
hacker@users~becoming-root-with-su:~$ su
Password: 
root@users~becoming-root-with-su:/home/hacker# cat /flag
pwn.college{8Zaip1AfE9-T0sVq3alXMghP4aG.dVTN0UDLzATN0czW}
```

i used su and then entered the password, took some time to figure out that i can't see the password when im entering it, thought the terminal wasnt working. but then i entered and then read the file using the cat command and obtained the flag
