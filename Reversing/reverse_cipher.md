# reverse_cipher

## Descripción
We have recovered a [binary](https://jupiter.challenges.picoctf.org/static/7aa5f383ec616fe9d72c2ffe1fabd0d9/rev) and a [text file](https://jupiter.challenges.picoctf.org/static/7aa5f383ec616fe9d72c2ffe1fabd0d9/rev_this). Can you reverse the flag.

## Pistas
- objdump and Gihdra are some tools that could assist with this

## Solución
```python
rev = open('rev_this').read()

for j in range(8,len(rev)-1):
        if j & 1 == 0:
                print(chr(ord(rev[j])-5), end= '')
        else:
                print(chr(ord(rev[j])+2), end= '')
   
```

## Bandera
picoCTF{r3v3rs36ad73964}

## Notas adicionales
Ghidra
Reversing
Python3

## Referencias
None