# PW Crack 2
## Descripción
Can you crack the password to get the flag? Download the password checker [here](https://artifacts.picoctf.net/c/13/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/13/level2.flag.txt.enc) in the same directory too.

## Pistas
- Does that encoding look familiar?
- The `str_xor` function does not need to be reverse engineered for this challenge.

## Solución
```shell
┌──(kali㉿kali)-[~/picoCTF/GeneralSkills/2022/PW2]
└─$ nano level2.py

┌──(kali㉿kali)-[~/picoCTF/GeneralSkills/2022/PW2]
└─$ python3         
Python 3.10.8 (main, Nov  4 2022, 09:21:25) [GCC 12.2.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> chr(0x64) + chr(0x65) + chr(0x37) + chr(0x36)
'de76'
>>> 

┌──(kali㉿kali)-[~/picoCTF/GeneralSkills/2022/PW2]
└─$ python level2.py
Please enter correct password for flag: de76
Welcome back... your flag, user:'
picoCTF{tr45h_51ng1ng_489dea9a}

```

## Bandera
picoCTF{tr45h_51ng1ng_489dea9a}

## Notas adicionales
nano
python

## Referencias
None