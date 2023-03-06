# Level 20

## Objetivo
To gain access to the next level, you should use the setuid binary in the homedirectory. Execute it without arguments to find out how to use it. The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary.

## Datos de acceso
**bandit.labs.overthewire.org**
**bandit19**
## Solución

```bash
bandit20@bandit:~$ nc -lnvp 2020 <<< VxCazJaVykI6W36BkBU0mJTCM8rR95XT & [1] 3444802 bandit20@bandit:~$ Listening on 0.0.0.0 2020 bandit20@bandit:~$ ./suconnect 2020 Connection received on 127.0.0.1 48964 Read: VxCazJaVykI6W36BkBU0mJTCM8rR95XT Password matches, sending next password NvEJF7oVjkddltPSrdKEFOllh9V1IBcq [1]+ Done nc -lnvp 2020 <<< VxCazJaVykI6W36BkBU0mJTCM8rR95XT bandit20@bandit:~$ exit
```

## Datos adicionales

ls listar archivos
clear borrar pantalla

## Referencias
[setuid on Wikipedia](https://en.wikipedia.org/wiki/Setuid)