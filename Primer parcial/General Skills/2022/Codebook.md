# Codebook
## Descripción
Run the Python script `code.py` in the same directory as `codebook.txt`.

-   [Download code.py](https://artifacts.picoctf.net/c/1/code.py)
-   [Download codebook.txt](https://artifacts.picoctf.net/c/1/codebook.txt)

## Pistas
- On the webshell, use `ls` to see if both files are in the directory you are in
- The `str_xor` function does not need to be reverse engineered for this challenge.
- 
## Solución
```bash
┌──(kali㉿kali)-[~/picoCTF/GeneralSkills/2022/codebook]
└─$ ls
codebook.txt  code.py

┌──(kali㉿kali)-[~/picoCTF/GeneralSkills/2022/codebook]
└─$ python code.py     
picoCTF{c0d3b00k_455157_d9aa2df2}

```

## Bandera
picoCTF{c0d3b00k_455157_d9aa2df2}

## Notas adicionales
python
cd
mkdir

## Referencias
None
