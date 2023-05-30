# Picker IV

## Descripción
Can you figure out how this program works to get the flag? Connect to the program with netcat: `$ nc saturn.picoctf.net 63913` The program's source code can be downloaded [here](https://artifacts.picoctf.net/c/529/picker-IV.c). The binary can be downloaded [here](https://artifacts.picoctf.net/c/529/picker-IV).

## Pistas
- With Python, there are no binaries. With compiled languages like C, there is source code, and there are binaries. Binaries are created from source code, they are a conversion from the human-readable source code, to the highly efficient machine language, in this case: x86_64.
- How can you find the address that `win` is at?

## Solución
```bash
printf("%p", &win);
```

## Bandera
picoCTF{48}

## Notas adicionales
None

## Referencias
None