# Level 30

## Objetivo
There is a git repository at ssh://bandit30-git@localhost/home/bandit30-git/repo. The password for the user bandit30-git is the same as for the user bandit30.

Clone the repository and find the password for the next level.

## Datos de acceso
**bandit.labs.overthewire.org**
**bandit29**

## Solución

```bash
bandit30@bandit:/tmp/tmp.iFnbTcdMf4/repo$ git tag
secret

bandit30@bandit:/tmp/tmp.iFnbTcdMf4/repo$ git show secret
47e603bb428404d265f59c42920d81e5
```

## Datos adicionales

## Referencias
Linux Comand Line