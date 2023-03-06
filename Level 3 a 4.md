# Level 4

## Objetivo
The password for the next level is stored in a hidden file in the **inhere** directory.

## Datos de acceso
**bandit.labs.overthewire.org**
**bandit3**

## Solución

```bash
bandit3@bandit:~/inhere$ ls -la
total 12
drwxr-xr-x 2 root    root    4096 Jan 11 19:19 .
drwxr-xr-x 3 root    root    4096 Jan 11 19:19 ..
-rw-r----- 1 bandit4 bandit3   33 Jan 11 19:19 .hidden
bandit3@bandit:~/inhere$ cat .hidden
2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe
bandit3@bandit:~/inhere$
```

## Datos adicionales
pwd indica carpeta actual
ls listar archivos
clear borrar pantalla
-la sirve para ver archivos y carpetas ocultos
ls indica los archivos en el directorio
cat muestra el contenido de un archivo

## Referencias
None