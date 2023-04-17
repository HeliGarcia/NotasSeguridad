# WebNet1

## Descripción
We found this [packet capture](https://jupiter.challenges.picoctf.org/static/fbf98e695555a2a48fe42c9a245de376/capture.pcap) and [key](https://jupiter.challenges.picoctf.org/static/fbf98e695555a2a48fe42c9a245de376/picopico.key). Recover the flag.

## Pistas
- Try using a tool like Wireshark.
- How can you decrypt the TLS stream?

## Solución
Usando wireshark agregamos la key en preferencias TSL, posteriormente se busca la siguiente string en los detalles del paquete que contenga la contraseña.
Nos da una contraseña falsa, entonces exportamos los archivos empaquetados, donde está una imagen. A esa imagen se le hace un strings y grep y se obtiene la bandera.

## Bandera
picoCTF{honey.roasted.peanuts}

## Notas adicionales
wget
wireshark
strings
grep

## Referencias
None