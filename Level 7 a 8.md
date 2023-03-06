# Level 8

## Objetivo
The password for the next level is stored in the file **data.txt** next to the word **millionth**
## Datos de acceso
**bandit.labs.overthewire.org**
**bandit7**

## Solución

```bash
bandit8@bandit:~$ sort data.txt | uniq -u
EN632PlfYiZbn3PhVK3XOGSlNInNE00t
bandit8@bandit:~$
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