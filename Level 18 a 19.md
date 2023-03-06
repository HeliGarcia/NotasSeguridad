# Level 19

## Objetivo
The password for the next level is stored in a file **readme** in the homedirectory. Unfortunately, someone has modified **.bashrc** to log you out when you log in with SSH.

## Datos de acceso
**bandit.labs.overthewire.org**
**bandit18**

## Solución

```bash
ssh bandit18@bandit.labs.overthewire.org -p 2220 /bin/bash _ _ _ _ | |__ __ _ _ __ __| (_) |_ | '_ \ / _` | '_ \ / _` | | __| | |_) | (_| | | | | (_| | | |_ |_.__/ \__,_|_| |_|\__,_|_|\__| This is an OverTheWire game server. More information on http://www.overthewire.org/wargames bandit18@bandit.labs.overthewire.org's password: cat readme awhqfNnAbc1naukrpqDYcF95h7HoMTrC
```

## Datos adicionales
ssh, ls, cat

## Referencias
[Secure Shell (SSH) on Wikipedia](https://en.wikipedia.org/wiki/Secure_Shell)
[How to use SSH on wikiHow](https://www.wikihow.com/Use-SSH)