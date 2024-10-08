# reading manuals 

```bash
hacker@man~reading-manuals:~$ man challenge

CHALLENGE(1)                                      Challenge Commands                                     CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --ugolcx NUM
              print the flag if NUM is 742

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                                            May 2024                                          CHALLENGE(1)
hacker@man~reading-manuals:~$ /challenge/challenge
Incorrect usage! Please read the challenge man page!
hacker@man~reading-manuals:~$ cat /challenge/challenge
cat: /challenge/challenge: Permission denied
hacker@man~reading-manuals:~$ cat --ugolcx 742
cat: unrecognized option '--ugolcx'
Try 'cat --help' for more information.
hacker@man~reading-manuals:~$ /challenge/challenge --printfile --ugolcx 742
Incorrect usage! Please read the challenge man page!
hacker@man~reading-manuals:~$ /challenge/challenge --ugoclx 742
Incorrect usage! Please read the challenge man page!
hacker@man~reading-manuals:~$ /challenge/challenge --ugolcx 742
Correct usage! Your flag: pwn.college{IEYug7VC4QolcxlxnT2J8CKf3yC.dRTM4QDLzATN0czW}
```
