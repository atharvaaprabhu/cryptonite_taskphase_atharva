# crackign passwords

```bash
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
0g 0:00:00:21 1% 2/3 0g/s 257.0p/s 257.0c/s 257.0C/s ncc1701d..1022
0g 0:00:00:22 1% 2/3 0g/s 256.7p/s 256.7c/s 256.7C/s Johnson..buzz
aardvark         (zardus)
1g 0:00:00:22 100% 2/3 0.04395g/s 255.9p/s 255.9c/s 255.9C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ --show
ssh-entrypoint: --show: command not found
hacker@users~cracking-passwords:~$ su zardus
Password: 
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{kebIoH-F7dqkqbSv9AMIjFwq-D-.ddTN0UDLzATN0czW}
```
