# persmission tweaking practise

this was a rather lengthy code, and to shorten it i will just paste the inputs here, ignoring the outputs.
```bash
/challenge/run
chmod u-rw,g+r,o-rw /challenge/pwn
chmod u+wx,g+wx,o-rwx /challenge/pwn
chmod u+r,g+r /challenge/pwn
chmod o+rw /challenge/pwn
chmod o+x /challenge/pwn
chmod u-r /challenge/pwn
chmod u+r /challenge/pwn
chmod u-r,u-x,o-r,o-x /challenge/pwn
chmod u+r /flag
cat /flag
```
this did take me multiple attempts to figure out how actually i should solve this question and i did take some assistance for this.
