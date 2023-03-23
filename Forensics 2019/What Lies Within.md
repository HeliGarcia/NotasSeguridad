# What Lies Within

## Descripción
There's something in the [building](https://jupiter.challenges.picoctf.org/static/011955b303f293d60c8116e6a4c5c84f/buildings.png). Can you retrieve the flag?

## Pistas
- There is data encoded somewhere... there might be an online decoder.
## Solución
```shell
┌──(kali㉿kali)-[~/picoCTF/forensics/whatlieswithin]
└─$ zsteg -a buildings.png | grep pico
b1,rgb,lsb,xy       .. text: "picoCTF{h1d1ng_1n_th3_b1t5}"

```

## Bandera
picoCTF{h1d1ng_1n_th3_b1t5}

## Notas adicionales
zsteg
grep

## Referencias
[zsteg](https://github.com/zed-0xff/zsteg)