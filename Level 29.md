# Level 29

## Objetivo
There is a git repository at ssh://bandit29-git@localhost/home/bandit29-git/repo. The password for the user bandit29-git is the same as for the user bandit29.

Clone the repository and find the password for the next level.

## Datos de acceso
**bandit.labs.overthewire.org**
**bandit28**

## Solución

```bash
bandit29@bandit:/tmp/tmp.Qjbad6ocpi/repo$ git checkout dev
Branch dev set up to track remote branch dev from origin.
Switched to a new branch 'dev'
bandit29@bandit:/tmp/tmp.Qjbad6ocpi/repo$ ls -la
total 20
drwxr-sr-x 4 bandit29 root 4096 Jul  3 13:01 .
drwx--S--- 3 bandit29 root 4096 Jul  3 12:50 ..
drwxr-sr-x 2 bandit29 root 4096 Jul  3 13:01 code
drwxr-sr-x 8 bandit29 root 4096 Jul  3 13:01 .git
-rw-r--r-- 1 bandit29 root  134 Jul  3 13:01 README.md
bandit29@bandit:/tmp/tmp.Qjbad6ocpi/repo$ cat README.md 
# Bandit Notes
Some notes for bandit30 of bandit.

## credentials

- username: bandit30
- password: 5b90576bedb2cc04c86a9e924ce42faf
```

## Datos adicionales
None
## Referencias
Linux Comand Line