# Level 7

## Objetivo
The password for the next level is stored **somewhere on the server** and has all of the following properties:

-   owned by user bandit7
-   owned by group bandit6
-   33 bytes in size

## Datos de acceso
**bandit.labs.overthewire.org**
**bandit6**

## Solución

```bash
bandit6@bandit:~$ find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
/var/lib/dpkg/info/bandit7.password
bandit6@bandit:~$ cat /var/lib/dpkg/info/bandit7.password
z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S
bandit6@bandit:~$
```

## Datos adicionales
| find |  | busca de forma específica con otros parámetros |
| -type f |  | parámetro que busca archivos (file) |
| -size |  | parámetro que busca según el tamaño del archivo | 
| -readable |  | indica archivos legibles o ascii | 
| -group |  |
| -user |  |
## Referencias
Linux Comand Line