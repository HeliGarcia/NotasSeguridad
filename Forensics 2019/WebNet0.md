# WebNet0

## Descripción
We found this [packet capture](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/capture.pcap) and [key](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/picopico.key). Recover the flag.

## Pistas
- Try using a tool like Wireshark.
- How can you decrypt the TLS stream?

## Solución
Usando wireshark agregamos la key en preferencias TSL, posteriormente se busca la siguiente string en los detalles del paquete que contenga la contraseña.

## Bandera
picoCTF{nongshim.shrimp.crackers}

## Notas adicionales
wget
wireshark

## Referencias
None