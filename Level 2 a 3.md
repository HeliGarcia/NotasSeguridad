# Level 3

## Objetivo
The password for the next level is stored in a file called **spaces in this filename** located in the home directory.

## Datos de acceso
**bandit.labs.overthewire.org**
**bandit2**

## Solución

```bash
bandit2@bandit:~$ ls
spaces in this filename
bandit2@bandit:~$ cat "spaces in this file"
cat: 'spaces in this file': No such file or directory
bandit2@bandit:~$ cat "spaces in this filename"
aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG
bandit2@bandit:~$
```

## Datos adicionales
pwd indica carpeta actual
ls listar archivos
clear borrar pantalla
ls indica los archivos en el directorio
cat muestra el contenido de un archivo

## Referencias
[Google Search for “spaces in filename”](https://www.google.com/search?q=spaces+in+filename)
