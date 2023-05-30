# transposition-trial

## Descripción
Our data got corrupted on the way here. Luckily, nothing got replaced, but every block of 3 got scrambled around! The first word seems to be three letters long, maybe you can use that to recover the rest of the message. Download the corrupted message [here](https://artifacts.picoctf.net/c/191/message.txt).

## Pistas
- Split the message up into blocks of 3 and see how the first block is scrambled

## Solución
```bash
┌──(kali㉿kali)-[~/picoCTF/tercerparcial/transposition]
└─$ cat message.txt 
heTfl g as iicpCTo{7F4NRP051N5_16_35P3X51N3_V6E5926A}4    
```
Usando Transposition Cipher solver se obtiene una tabla que indica el orden de los elementos para la bandera.

## Bandera
picoCTF{7R4N5P051N6_15_3XP3N51V3_56E6924A}

## Notas adicionales
Transposition Cripher
Tholman

## Referencias
None