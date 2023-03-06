# Level 10

## Objetivo
The password for the next level is stored in the file **data.txt** in one of the few human-readable strings, preceded by several ‘=’ characters.
## Datos de acceso
**bandit.labs.overthewire.org**
**bandit9**

## Solución

```bash
bandit10@bandit:~$ ls
data.txt
bandit10@bandit:~$ cat data.txt
VGhlIHBhc3N3b3JkIGlzIDZ6UGV6aUxkUjJSS05kTllGTmI2blZDS3pwaGxYSEJNCg==
bandit10@bandit:~$ base64 -d data.txt
The password is 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM
bandit10@bandit:~$ cat data.txt | base64 -d
The password is 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM
bandit10@bandit:~$
```

## Datos adicionales
| base64 | | convierte a base64 el mensaje |
| base64 -d | | revierte la conversión |

## Referencias
Linux Comand Line
[Base64 on Wikipedia](https://en.wikipedia.org/wiki/Base64)