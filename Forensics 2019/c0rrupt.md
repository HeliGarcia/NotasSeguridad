# c0rrupt

## Descripción
We found this [file](https://jupiter.challenges.picoctf.org/static/ab30fcb7d47364b4190a7d3d40edb551/mystery). Recover the flag.

## Pistas
- Try fixing the file header

## Solución
```bash
┌──(kali㉿kali)-[~/picoCTF/forensics/extensions]
└─$ file flag.txt  
flag.txt: PNG image data, 1697 x 608, 8-bit/color RGB, non-interlaced         
┌──(kali㉿kali)-[~/picoCTF/forensics/extensions]
└─$ hexeditor flag.txt
┌──(kali㉿kali)-[~/picoCTF/forensics/extensions]
└─$ mv flag.txt flag.png
┌──(kali㉿kali)-[~/picoCTF/forensics/extensions]
└─$ open flag.png
```

## Bandera
picoCTF{c0rrupt10n_1847995}

## Notas adicionales
file
mv
extensiones
hex

## Referencias
None