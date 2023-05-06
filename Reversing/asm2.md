# asm2

## Descripción
What does asm2(0x4,0x2d) return? Submit the flag as a hexadecimal value (starting with '0x'). NOTE: Your submission for this question will NOT be in the normal flag format. [Source](https://jupiter.challenges.picoctf.org/static/ceac75672637589213b952abe32c84b3/test.S)

## Pistas
- assembly [conditions](https://www.tutorialspoint.com/assembly_programming/assembly_conditions.htm)

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