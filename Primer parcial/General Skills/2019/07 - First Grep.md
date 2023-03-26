# First Grep

## Descripción
Can you find the flag in [file](https://jupiter.challenges.picoctf.org/static/315d3325dc668ab7f1af9194f2de7e7a/file)? This would be really tedious to look through manually, something tells me there is a better way.

## Pistas
grep [tutorial](https://ryanstutorials.net/linuxtutorial/grep.php)

## Solución
```python
heligarcia-picoctf@webshell:~$ wget https://jupiter.challenges.picoctf.org/static/315d3325dc668ab7f1af9194f2de7e7a/file
--2023-03-07 18:07:47--  https://jupiter.challenges.picoctf.org/static/315d3325dc668ab7f1af9194f2de7e7a/file
Resolving jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)... 3.131.60.8
Connecting to jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)|3.131.60.8|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 14551 (14K) [application/octet-stream]
Saving to: 'file'

file                  100%[=======================>]  14.21K  --.-KB/s    in 0s      

2023-03-07 18:07:47 (446 MB/s) - 'file' saved [14551/14551]

heligarcia-picoctf@webshell:~$ ls
README.txt  file  strings
heligarcia-picoctf@webshell:~$ grep file
^C
heligarcia-picoctf@webshell:~$ cat file | grep picoCTF
picoCTF{grep_is_good_to_find_things_f77e0797}
```

## Bandera
picoCTF{grep_is_good_to_find_things_f77e0797}

## Notas adicionales

## Referencias
[Converter](https://www.rapidtables.com/convert/number/hex-to-decimal.html)
