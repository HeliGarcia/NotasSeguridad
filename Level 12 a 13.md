# Level 13

## Objetivo
The password for the next level is stored in the file **data.txt**, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)
## Datos de acceso
**bandit.labs.overthewire.org**
**bandit12**

## Solución

```bash
ssh -i llave.txt bandit14@bandit.labs.overthewire.org -p 2220

bandit14@bandit:~$ ls /etc/bandit_pass/bandit14
/etc/bandit_pass/bandit14
bandit14@bandit:~$ cat /etc/bandit_pass/bandit14
fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq

```
## Datos adicionales

## Referencias
Linux Comand Line
[SSH/OpenSSH/Keys](https://help.ubuntu.com/community/SSH/OpenSSH/Keys)