# Challenge Name
Searching For Manuals
## My solve
**Flag:** `pwn.college{w6dD-xwXj1Usqp1WhccOyz145oX.QX1EDO0wSO0EzNzEzW}`

```bash
Connected!
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -k challenge
iwjioinpxm (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man iwjioinpxm
hacker@man~searching-for-manuals:~$ /challenge/challenge  --iwjioi 840
Correct usage! Your flag: pwn.college{8iwjiAoJin_EQpIx4muuEQDFeY0.QX2EDO0wSO0EzNzEzW}
```
## Incorrect tangents I went on
none

## What I learned
complex search in manual
I also learnt that man -k can be used to find string in all short manuals with a match (man -K for all manuals)

## References 
none
