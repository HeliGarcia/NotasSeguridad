# vault-door-1

## Descripción
This vault uses some complicated arrays! I hope you can make sense of it, special agent. The source code for this vault is here: [VaultDoor1.java](https://jupiter.challenges.picoctf.org/static/ff2585f7afd21b81f69d2fbe37c081ae/VaultDoor1.java)

## Pistas
- Look up the charAt() method online.

## Solución
```bash
┌──(kali㉿kali)-[~/picoCTF/Reverse/vault-training]
└─$ cat bandera | sort | awk '{print($3)}' | tr -d "'" | tr -d "\n"
d35cr4mbl3_tH3_cH4r4cT3r5_75092e;    
```

## Bandera
picoCTF{d35cr4mbl3_tH3_cH4r4cT3r5_75092e}

## Notas adicionales
awk
tr
sort
Java
Reversing

## Referencias
None