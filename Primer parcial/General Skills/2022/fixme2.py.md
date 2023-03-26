# fixme2.py
## Descripción
Fix the syntax error in the Python script to print the flag. [Download Python script](https://artifacts.picoctf.net/c/5/fixme2.py)
## Pistas
- Are equality and assignment the same symbol?
- To view the file in the webshell, do: `$ nano fixme2.py`
- To exit `nano`, press Ctrl and x and follow the on-screen prompts.
- The `str_xor` function does not need to be reverse engineered for this challenge.

## Solución
```shell
┌──(kali㉿kali)-[~/picoCTF/GeneralSkills/2022/fixme1]
└─$ nano fixme2.py

'Una vez en el nano, sólo debemos agregar un "=" más en el último if, ya que si no, no se realiza una comparación.'

┌──(kali㉿kali)-[~/picoCTF/GeneralSkills/2022/fixme1]
└─$ python fixme2.py
That is correct! Here's your flag: picoCTF{3qu4l1ty_n0t_4551gnm3nt_4863e11b}


```

## Bandera
picoCTF{3qu4l1ty_n0t_4551gnm3nt_4863e11b}


## Notas adicionales
python
Equals symbol in python for assignment and equality.

## Referencias
None
