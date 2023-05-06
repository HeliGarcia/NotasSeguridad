# asm1

## Descripción
What does asm1(0x2e0) return? Submit the flag as a hexadecimal value (starting with '0x'). NOTE: Your submission for this question will NOT be in the normal flag format. [Source](https://jupiter.challenges.picoctf.org/static/f1c2358ff7d1e9386e41552c549cf2f6/test.S)

## Pistas
- assembly [conditions](https://www.tutorialspoint.com/assembly_programming/assembly_conditions.htm)

## Solución
```python
>>> 0x2e0 > 0x3fb
>>> 0x2e0 != 0x559
>>> hex(0x2e0 - 0xa)
'0x2d6'
```

## Bandera
0x2d6

## Notas adicionales
x86 Assembly language
Reversing

## Referencias
None