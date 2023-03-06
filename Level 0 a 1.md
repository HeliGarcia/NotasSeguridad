# Level 1

## Objetivo
The password for the next level is stored in a file called **readme** located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

## Datos de acceso
**bandit.labs.overthewire.org**
**bandit0**
**bandit0**
readme

## Solución

```bash
bandit0@bandit:~$ ls
readme
bandit0@bandit:~$ cat readme
NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL
bandit0@bandit:~$
```

## Datos adicionales
pwd indica carpeta actual
ls listar archivos
clear borrar pantalla
ls indica los archivos en el directorio
cat muestra el contenido de un archivo

## Referencias
[Secure Shell (SSH) on Wikipedia](https://en.wikipedia.org/wiki/Secure_Shell)
[How to use SSH on wikiHow](https://www.wikihow.com/Use-SSH)
