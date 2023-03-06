# Level 9

## Objetivo
The password for the next level is stored in the file **data.txt** and is the only line of text that occurs only once
## Datos de acceso
**bandit.labs.overthewire.org**
**bandit8**

## Solución

```bash
bandit9@bandit:~$ strings data.txt | grep "=="
c========== the
h;========== password
========== isT
n.E========== G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s
bandit9@bandit:~$
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