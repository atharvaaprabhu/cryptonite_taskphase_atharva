# epic file quest

```bash
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
SNIPPET  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin      challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cd SNIPPET
ssh-entrypoint: cd: SNIPPET: Not a directory
hacker@commands~an-epic-filesystem-quest:/$ cat /SNIPPET
Yahaha, you found me!
The next clue is in: /usr/lib/x86_64-linux-gnu/avahi
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/lib/x86_64-linux-gnu/avahi
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/avahi$ ls
TRACE  service-types.db
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/avahi$ cat /TRACE
cat: /TRACE: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/avahi$ cat /service-types.db
cat: /service-types.db: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/avahi$ c /TRACE
ssh-entrypoint: c: command not found
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/avahi$ cat /trace
cat: /trace: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/avahi$ ls /TRACE
ls: cannot access '/TRACE': No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/avahi$ cat TRACE
Yahaha, you found me!
The next clue is in: /opt/radare2/shlr/capstone/suite/MC/SystemZ
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/avahi$ cd /opt/radare2/slr/capstone/suite/MC/SystemZ
ssh-entrypoint: cd: /opt/radare2/slr/capstone/suite/MC/SystemZ: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/avahi$ cd /opt/radare2/shlr/capstone/suite/MC/SystemZhacker@commands~an-epic-filesystem-quest:/opt/radare2/shlr/capstone/suite/MC/SystemZ$ ls
BLUEPRINT  insn-good-z196.s.cs  insn-good.s.cs  regs-good.s.cs
hacker@commands~an-epic-filesystem-quest:/opt/radare2/shlr/capstone/suite/MC/SystemZ$ cat BLUEPRINT
Yahaha, you found me!
The next clue is in: /usr/share/doc/libpcap0.8-dev
hacker@commands~an-epic-filesystem-quest:/opt/radare2/shlr/capstone/suite/MC/SystemZ$ cd /usr/share/doc/libpcap0.8-dev
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libpcap0.8-dev$ ls
CLUE  changelog.Debian.gz  copyright
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libpcap0.8-dev$ cat CLUE
Tubular find!
The next clue is in: /usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/STIX

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libpcap0.8-dev$ cd /usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/STIX
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/STIX$ LS
ssh-entrypoint: LS: command not found
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/STIX$ ls
General      IntegralsUp    NonUnicode   SizeFourSym   SizeTwoSym       fontdata-beta.js
IntegralsD   IntegralsUpD   POINTER      SizeOneSym    Variants         fontdata-extra.js
IntegralsSm  IntegralsUpSm  SizeFiveSym  SizeThreeSym  fontdata-1.0.js  fontdata.js
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/STIX$ cat POINTER
Tubular find!
The next clue is in: /usr/share/racket/pkgs/games/paint-by-numbers/compiled

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/STIX$ cd /usr/share/racket/pkgs/games/paint-by-numbers/compiled
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/games/paint-by-numbers/compiled$ ls -a
.       all-problems_rkt.dep  gui_rkt.zo    paint-by-numbers_rkt.dep  problem_rkt.zo
..      all-problems_rkt.zo   info_rkt.dep  paint-by-numbers_rkt.zo   solve_rkt.dep
.ALERT  gui_rkt.dep           info_rkt.zo   problem_rkt.dep           solve_rkt.zo
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/games/paint-by-numbers/compiled$ cat .ALERT
Great sleuthing!
The next clue is in: /opt/radare2/libr/arch/p/bf

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/games/paint-by-numbers/compiled$ cd /opt/radare2/libr/arch/p/bf
hacker@commands~an-epic-filesystem-quest:/opt/radare2/libr/arch/p/bf$ ls -a
.  ..  .BRIEF  plugin.c  plugin.d  plugin.o
hacker@commands~an-epic-filesystem-quest:/opt/radare2/libr/arch/p/bf$ cat .BRIEF
Tubular find!
The next clue is in: /etc/apache2/conf-available
hacker@commands~an-epic-filesystem-quest:/opt/radare2/libr/arch/p/bf$ cd /etc/apache2/conf-available
hacker@commands~an-epic-filesystem-quest:/etc/apache2/conf-available$ ls
MESSAGE       localized-error-pages.conf    php7.4-cgi.conf  serve-cgi-bin.conf
charset.conf  other-vhosts-access-log.conf  security.conf
hacker@commands~an-epic-filesystem-quest:/etc/apache2/conf-available$ cat MESSAGE
Great sleuthing!
The next clue is in: /usr/share/bug/mime-support

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/etc/apache2/conf-available$ cat /usr/share/bug/mime-support
cat: /usr/share/bug/mime-support: Is a directory
hacker@commands~an-epic-filesystem-quest:/etc/apache2/conf-available$ ls /usr/share/bug/mime-support
README-TRAPPED  presubj
hacker@commands~an-epic-filesystem-quest:/etc/apache2/conf-available$ cat /usr/share/bug/mime-support/README-TRAPPED
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{oC57npkiF102Zr1xHHA0T5BIkEd.dljM4QDLzATN0czW}
```
