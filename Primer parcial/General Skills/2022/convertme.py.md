# convertme.py
## Descripción
Run the Python script and convert the given number from decimal to binary to get the flag. [Download Python script](https://artifacts.picoctf.net/c/24/convertme.py)

## Pistas
- Look up a decimal to binary number conversion app on the web or use your computer's calculator!
- The `str_xor` function does not need to be reverse engineered for this challenge.
- If you have Python on your computer, you can download the script normally and run it. Otherwise, use the `wget` command in the webshell.
- To use `wget` in the webshell, first right click on the download link and select 'Copy Link' or 'Copy Link Address'
- Type everything after the dollar sign in the webshell: `$ wget` , then paste the link after the space after `wget` and press enter. This will download the script for you in the webshell so you can run it!
- Finally, to run the script, type everything after the dollar sign and then press enter: `$ python3 convertme.py`

## Solución
```shell
┌──(kali㉿kali)-[~/picoCTF/GeneralSkills/2022/convertme]
└─$ python convertme.py
If 45 is in decimal base, what is it in binary base?
Answer: 101101
That is correct! Here's your flag: picoCTF{4ll_y0ur_b4535_722f6b39}

```

## Bandera
picoCTF{4ll_y0ur_b4535_722f6b39}

## Notas adicionales
python
binary numbers
decimal numbers

## Referencias
CyberChef
