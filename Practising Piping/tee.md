# duplicating piped data with tee

```bash
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee output.txt | /challenge/college
cat output.txt
Processing...
WARNING: you are overwriting file output.txt with tee's output...
The input to 'college' does not contain the correct secret code! This code 
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the 
output of 'pwn' and figure out what the code needs to be.
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "EIkKgXXj"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret EIkKgXXj | tee >(cat) | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{EIkKgXXjPhG0IDX6rwCKaAe8DJ9.dFjM5QDLzATN0czW}
```
