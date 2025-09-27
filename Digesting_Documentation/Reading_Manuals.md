# Challenge Name
Reading Manuals
## My solve
**Flag:** `pwn.college{EpLzgOHCrAn5uGGMVAlo08uHSoj.QX0EDO0wSO0EzNzEzW}`

```bash
Connected!
hacker@man~reading-manuals:~$ man challenge

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

       --pzgrnu NUM
              print the flag if NUM is 508

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                                            May 2024                                          CHALLENGE(1)

hacker@man~reading-manuals:~$ /challenge/challenge --pzgrnu 508
Correct usage! Your flag: pwn.college{EpLzgOHCrAn5uGGMVAlo08uHSoj.QX0EDO0wSO0EzNzEzW}
```
## Incorrect tangents I went on
none

## What I learned
introduction of man command, first i read the manual for challenge and found out that printing --pzgrnu NUM with NUM=508 would give me the flag
we can quit the manual page by typing q

## References 
none
