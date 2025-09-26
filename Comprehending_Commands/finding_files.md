# Challenge Name
finding files
## My solve
**Flag:** `pwn.college{MVGD7opNOkrUsqkz51jbnkiSQDR.QXyMDO0wSO0EzNzEzW}`

```bash
Connected!
hacker@commands~finding-files:~$ find / -name flag
find: ‘/tmp/tmp.4mK6TfTSUV’: Permission denied
find: ‘/etc/ssl/private’: Permission denied
/usr/lib/python3.8/ensurepip/flag
/usr/local/lib/python3.8/dist-packages/pwnlib/flag
find: ‘/var/cache/apt/archives/partial’: Permission denied
find: ‘/var/cache/ldconfig’: Permission denied
find: ‘/var/cache/private’: Permission denied
find: ‘/var/lib/apt/lists/partial’: Permission denied
find: ‘/var/lib/mysql-files’: Permission denied
find: ‘/var/lib/private’: Permission denied
find: ‘/var/lib/mysql’: Permission denied
find: ‘/var/lib/mysql-keyring’: Permission denied
find: ‘/var/lib/php/sessions’: Permission denied
find: ‘/var/log/private’: Permission denied
find: ‘/var/log/apache2’: Permission denied
find: ‘/var/log/mysql’: Permission denied
find: ‘/run/mysqld’: Permission denied
find: ‘/run/sudo’: Permission denied
find: ‘/root’: Permission denied
/opt/pwndbg/.venv/lib/python3.8/site-packages/pwnlib/flag
^C
hacker@commands~finding-files:~$ cat /usr/lib/python3.8/ensurepip/flag
pwn.college{MVGD7opNOkrUsqkz51jbnkiSQDR.QXyMDO0wSO0EzNzEzW}
```
## Incorrect tangents I went on
none

## What I learned
we use the find command to find files, further we can use find / -name filename to find a specific file filename

## References 
none
