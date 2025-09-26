# Challenge Name
hidden files
## My solve
**Flag:** `pwn.college{cd3fDu0xjDkngDQ03_ul3w5lA2H.QXwUDO0wSO0EzNzEzW}`

```bash
Connected!
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv             bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-242102506031893  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat /.flag-242102506031893
pwn.college{cd3fDu0xjDkngDQ03_ul3w5lA2H.QXwUDO0wSO0EzNzEzW}
```
## Incorrect tangents I went on
none

## What I learned
hidden files cannot be normally viewed by ls and they start with ".", we put ls -a to view the hidden files 

## References 
none
