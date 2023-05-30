# SRA

## Descripción
Smash the stack Can you overflow the buffer and modify the other local variable? The program is available [here](https://artifacts.picoctf.net/c/519/local-target). You can view source [here](https://artifacts.picoctf.net/c/519/local-target.c). And connect with it using:

## Pistas
- Do anything you can to change `num`.
- When you change `num`, view the value as hexadecimal.

## Solución
```bash
┌──(kali㉿kali)-[~/picoCTF/tercerparcial/SRA]
└─$ nc saturn.picoctf.net 62697
anger = 40287015126812067339951863570223732501481554826586041903065755366699081920262
envy = 28824063003161168380767515687979247550935709001618371181656782283577971004593
vainglory?
> 

```

## Bandera
picoCTF{1nclu51v17y_1of2_f7w_2of2_6edef411}

## Notas adicionales
RSA
SRA

## Referencias
None