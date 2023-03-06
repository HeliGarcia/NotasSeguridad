# Level 14

## Objetivo
The password for the next level is stored in **/etc/bandit_pass/bandit14 and can only be read by user bandit14**. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. **Note:** **localhost** is a hostname that refers to the machine you are working on

## Datos de acceso
**bandit.labs.overthewire.org**
**bandit13**

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
-   [IP Addresses](http://computer.howstuffworks.com/web-server5.htm)
-   [IP Address on Wikipedia](https://en.wikipedia.org/wiki/IP_address)
-   [Localhost on Wikipedia](https://en.wikipedia.org/wiki/Localhost)
-   [Ports](http://computer.howstuffworks.com/web-server8.htm)
-   [Port (computer networking) on Wikipedia](https://en.wikipedia.org/wiki/Port_(computer_networking))