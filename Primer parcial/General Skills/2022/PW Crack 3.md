# PW Crack 3
## Descripción
Can you crack the password to get the flag? Download the password checker [here](https://artifacts.picoctf.net/c/17/level3.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/17/level3.flag.txt.enc) and the [hash](https://artifacts.picoctf.net/c/17/level3.hash.bin) in the same directory too. There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.

## Pistas
- To view the level3.hash.bin file in the webshell, do: `$ bvi level3.hash.bin`
- To exit `bvi` type `:q` and press enter.
- The `str_xor` function does not need to be reverse engineered for this challenge.

## Solución
```shell
Posibles contraseñas:
pos_pw_list = ["f09e", "4dcf", "87ab", "dba8", "752e", "3961", "f159"]
Yo sólo inserté de una en una hasta dar con la correcta.

┌──(kali㉿kali)-[~/picoCTF/GeneralSkills/2022/PW3]
└─$ python level3.py
Please enter correct password for flag: 87ab
Welcome back... your flag, user:'
picoCTF{m45h_fl1ng1ng_cd6ed2eb}

```

## Bandera
picoCTF{m45h_fl1ng1ng_cd6ed2eb}

## Notas adicionales
nano
bvi
python

## Referencias
None