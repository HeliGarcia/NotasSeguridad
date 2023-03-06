# Level 15

## Objetivo
The password for the next level can be retrieved by submitting the password of the current level to **port 30000 on localhost**.

## Datos de acceso
**bandit.labs.overthewire.org**
**bandit14**

## Solución

```bash
bandit14@bandit:~$ nc -v localhost 30000
Connection to localhost (127.0.0.1) 30000 port [tcp/*] succeeded!
fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq
Correct!
jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt
```

## Datos adicionales
pwd indica carpeta actual
ls listar archivos
clear borrar pantalla

## Referencias
