# Challenge Name
implicit relative path

## My solve
**Flag:** `pwn.college{cb7jBJMtWDAJpLvrCdo7gh0ONWs.QXxUTN0wSO0EzNzEzW}`

```bash
Connected!
hacker@paths~implicit-relative-path:~$ cd /
hacker@paths~implicit-relative-path:/$ ./challenge/run
Incorrect...
You are not currently in the /challenge directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-path:/$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{cb7jBJMtWDAJpLvrCdo7gh0ONWs.QXxUTN0wSO0EzNzEzW}
```
## Incorrect tangents I went on
none

## What I learned
cwd
. as Current Directory in Paths

## References 
none
