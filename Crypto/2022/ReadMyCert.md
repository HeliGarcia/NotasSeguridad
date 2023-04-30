# ReadMyCert
## Descripción
How about we take you on an adventure on exploring certificate signing requests Take a look at this CSR file [here](https://artifacts.picoctf.net/c/421/readmycert.csr).

## Pistas
- Download the certificate signing request and try to read it.

## Solución
Usar un decodificador de CSR.
```bash
openssl req -text -noout -verify -in readmycert.csr
Certificate request self-signature verify OK
Certificate Request:
    Data:
        Version: 1 (0x0)
        Subject: CN = picoCTF{read_mycert_3aa80090}, name = ctfPlayer
        Subject Public Key Info:
            Public Key Algorithm: rsaEncryption
                Public-Key: (2048 bit)
```

## Bandera
picoCTF{read_mycert_3aa80090}

## Notas adicionales
CSR

## Referencias
[CSR decode](https://www.sslshopper.com/csr-decoder.html)
