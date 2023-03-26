# PW Crack 1
## Descripción
Can you crack the password to get the flag? Download the password checker [here](https://artifacts.picoctf.net/c/11/level1.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/11/level1.flag.txt.enc) in the same directory too.

## Pistas
- To view the file in the webshell, do: `$ nano level1.py`
- To exit `nano`, press Ctrl and x and follow the on-screen prompts.
- The `str_xor` function does not need to be reverse engineered for this challenge.

## Solución
```shell
┌──(kali㉿kali)-[~/picoCTF/GeneralSkills/2022/PW1]
└─$ ls
level1.flag.txt.enc  level1.py

┌──(kali㉿kali)-[~/picoCTF/GeneralSkills/2022/PW1]
└─$ nano level1.py

┌──(kali㉿kali)-[~/picoCTF/GeneralSkills/2022/PW1]
└─$ python level1.py
Please enter correct password for flag: 1e1a
Welcome back... your flag, user:'
picoCTF{545h_r1ng1ng_fa343060}

```

## Bandera
picoCTF{545h_r1ng1ng_fa343060}

## Notas adicionales
nano
python

## Referencias
None