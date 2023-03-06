# Level 27

## Objetivo
Good job getting a shell! Now hurry and grab the password for bandit27!
## Datos de acceso
**bandit.labs.overthewire.org**
**bandit26**

## Solución

```bash
:shell
bandit26@bandit:~$ ls -la
total 44
drwxr-xr-x  3 root     root      4096 Feb 21 22:03 .
drwxr-xr-x 70 root     root      4096 Feb 21 22:04 ..
-rwsr-x---  1 bandit27 bandit26 14876 Feb 21 22:03 bandit27-do
-rw-r--r--  1 root     root       220 Jan  6  2022 .bash_logout
-rw-r--r--  1 root     root      3771 Jan  6  2022 .bashrc
-rw-r--r--  1 root     root       807 Jan  6  2022 .profile
drwxr-xr-x  2 root     root      4096 Feb 21 22:03 .ssh
-rw-r-----  1 bandit26 bandit26   258 Feb 21 22:03 text.txt
bandit26@bandit:~$ ./bandit27-do
Run a command as another user.
  Example: ./bandit27-do id
bandit26@bandit:~$ ./bandit27-do cat /etc/bandit_pass/bandit27
YnQpBuifNMas1hcUFk70ZmqkhUU2EuaS
```

## Datos adicionales

## Referencias
Linux Comand Line