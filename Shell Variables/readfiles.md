# reading files

```bash
hacker@variables~reading-files:~$ PWN=$(< /challenge/read_me)
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{YcEH0yylLeAC6Vd_4muXj1Gdf37.dBjM4QDLzATN0czW}
```
it read the content of /challenge/read_me directly into PWN variable
