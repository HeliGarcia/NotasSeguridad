# Level 6

## Objetivo
The password for the next level is stored in a file somewhere under the **inhere** directory and has all of the following properties:

-   human-readable
-   1033 bytes in size
-   not executable

## Datos de acceso
**bandit.labs.overthewire.org**
**bandit5**

## Solución

```bash
bandit5@bandit:~$ cd inhere
bandit5@bandit:~/inhere$ find -readable -size 1033c -type f
./maybehere07/.file2
bandit5@bandit:~/inhere$ cd maybehere
-bash: cd: maybehere: No such file or directory
bandit5@bandit:~/inhere$ cd maybehere07
bandit5@bandit:~/inhere/maybehere07$ cat .file2
P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU
```

## Datos adicionales
| find | | busca de forma específica con otros parámetros |
| -type f | | parámetro que busca archivos (file) |
| -size | | parámetro que busca según el tamaño del archivo | 
| -readable |  | indica archivos legibles o ascii | 
## Referencias
Linux Comand Line