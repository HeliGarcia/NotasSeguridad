# Vigenere

## Descripción
Can you decrypt this message? Decrypt this [message](https://artifacts.picoctf.net/c/160/cipher.txt) using this key "CYLAB".

## Pistas
- https://en.wikipedia.org/wiki/Vigen%C3%A8re_cipher

## Solución
```bash
┌──(kali㉿kali)-[~/picoCTF/tercerparcial/transposition]
└─$ cat cipher.txt 
rgnoDVD{O0NU_WQ3_G1G3O3T3_A1AH3S_2951c89f}
```
Usando el desencriptado Vigenère se obtiene la bandera.

## Bandera
picoCTF{D0NT_US3_V1G3N3R3_C1PH3R_2951a89h}

## Notas adicionales
Vigenère Cipher

## Referencias
None