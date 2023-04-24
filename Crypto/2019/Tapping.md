# The Numbers

## Descripción
The [numbers](https://jupiter.challenges.picoctf.org/static/f209a32253affb6f547a585649ba4fda/the_numbers.png)... what do they mean?

## Pistas
- The flag is in the format PICOCTF{}

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