# Pixelated

## Descripción
I have these 2 images, can you make a flag out of them? [scrambled1.png](https://mercury.picoctf.net/static/c9593d1d2ac9d850da95bffe0ac3b6c6/scrambled1.png) [scrambled2.png](https://mercury.picoctf.net/static/c9593d1d2ac9d850da95bffe0ac3b6c6/scrambled2.png)

## Pistas
- [https://en.wikipedia.org/wiki/Visual_cryptography](https://en.wikipedia.org/wiki/Visual_cryptography)
- Think of different ways you can "stack" images

## Solución
```
convert scrambled1.png scrambled2.png -compose Add -composite flag.png
open flag.png
```

## Bandera
picoCTF{CRYPTOISFUN}

## Notas adicionales
vigenère decode
Cyberchef
caesar

## Referencias
None