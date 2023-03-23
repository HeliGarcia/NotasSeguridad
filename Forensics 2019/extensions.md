# extensions

## Descripción
This is a really weird text file [TXT](https://jupiter.challenges.picoctf.org/static/e7e5d188621ee705ceeb0452525412ef/flag.txt)? Can you find the flag?

## Pistas
- How do operating systems know what kind of file it is? (It's not just the ending!
- Make sure to submit the flag as picoCTF{XXXXX}
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
picoCTF{now_you_know_about_extensions}

## Notas adicionales
file
mv
extensiones
hex

## Referencias
None