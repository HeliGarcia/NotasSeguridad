# fixme1.py
## Descripción
Fix the syntax error in this Python script to print the flag. [Download Python script](https://artifacts.picoctf.net/c/26/fixme1.py)

## Pistas
- Indentation is very meaningful in Python
- To view the file in the webshell, do: `$ nano fixme1.py`
- To exit `nano`, press Ctrl and x and follow the on-screen prompts.
- The `str_xor` function does not need to be reverse engineered for this challenge.

## Solución
```shell
┌┌──(kali㉿kali)-[~/picoCTF/GeneralSkills/2022/fixme1]
└─$ nano fixme1.py             

'Una vez en el nano, sólo debemos eliminar espacios al momento de imprimir para evitar el error de identación.'

┌──(kali㉿kali)-[~/picoCTF/GeneralSkills/2022/fixme1]
└─$ python fixme1.py   
That is correct! Here's your flag: picoCTF{1nd3nt1ty_cr1515_09ee727a}

```

## Bandera
picoCTF{1nd3nt1ty_cr1515_09ee727a}

## Notas adicionales
python
Identation

## Referencias
None
