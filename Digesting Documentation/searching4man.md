# searching for manuals

```bash
hacker@man~searching-for-manuals:~$ man man
MAN(1)                                            Manual pager utils                                           MAN(1)

NAME
       man - an interface to the system reference manuals

SYNOPSIS
       man [man options] [[section] page ...] ...
       man -k [apropos options] regexp ...
       man -K [man options] [section] term ...
       man -f [whatis options] page ...
       man -l [man options] file ...
       man -w|-W [man options] page ...

DESCRIPTION
       man  is the system's manual pager.  Each page argument given to man is normally the name of a program, utility
       or function.  The manual page associated with each of these arguments is then found and displayed.  A section,
       if  provided,  will direct man to look only in that section of the manual.  The default action is to search in
       all of the available sections following a pre-defined order (see DEFAULTS), and to show only  the  first  page
       found, even if page exists in several sections.

       The table below shows the section numbers of the manual followed by the types of pages they contain.

       1   Executable programs or shell commands
       2   System calls (functions provided by the kernel)
       3   Library calls (functions within program libraries)
       4   Special files (usually found in /dev)
       5   File formats and conventions, e.g. /etc/passwd
       6   Games
       7   Miscellaneous (including macro packages and conventions), e.g. man(7), groff(7)
       8   System administration commands (usually only for root)
       9   Kernel routines [Non standard]

       A manual page consists of several sections.

       Conventional  section  names  include  NAME,  SYNOPSIS,  CONFIGURATION, DESCRIPTION, OPTIONS, EXIT STATUS, RE‐
       TURN VALUE, ERRORS, ENVIRONMENT, FILES, VERSIONS, CONFORMING TO, NOTES, BUGS, EXAMPLE, AUTHORS, and SEE ALSO.

       The following conventions apply to the SYNOPSIS section and can be used as a guide in other sections.

       bold text          type exactly as shown.
       italic text        replace with appropriate argument.
       [-abc]             any or all arguments within [ ] are optional.
       -a|-b              options delimited by | cannot be used together.
       argument ...       argument is repeatable.
       [expression] ...   entire expression within [ ] is repeatable.

       Exact rendering may vary depending on the output device.  For instance, man will usually not be able to render
       italics when running in a terminal, and will typically use underlined or coloured text instead.

       The  command  or function illustration is a pattern that should match all possible invocations.  In some cases
       it is advisable to illustrate several exclusive invocations as is shown in the SYNOPSIS section of this manual
       page.

EXAMPLES
       man ls
           Display the manual page for the item (program) ls.

       man man.7
           Display  the manual page for macro package man from section 7.  (This is an alternative spelling of "man 7
           man".)

       man 'man(7)'
hacker@man~searching-for-manuals:~$ man -k challenge
ofkjttvsfd (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man ofkjttvsfd

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

       --ofkjtt NUM
              print the flag if NUM is 349

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                                            May 2024                                          CHALLENGE(1)
hacker@man~searching-for-manuals:~$ /challenge/challenge -ofkjtt 349
Incorrect usage! Please read the challenge man page!
hacker@man~searching-for-manuals:~$ /challenge/challenge --ofkjtt 349
Correct usage! Your flag: pwn.college{oTGV34fk_GjCt9tv4sVfZdQ0GeF.dZTM4QDLzATN0czW}
```
