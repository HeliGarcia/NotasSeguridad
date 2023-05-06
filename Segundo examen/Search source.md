# Search source

## Descripción
The developer of this website mistakenly left an important artifact in the website source, can you find it? The website is [here](http://saturn.picoctf.net:53295/)

## Pistas
- How could you mirror the website on your local machine so you could use more powerful tools for searching?

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