# miniRSA

## Descripción
Let's decrypt this: [ciphertext](https://jupiter.challenges.picoctf.org/static/ee7e2388b45f521b285334abb5a63771/ciphertext)? Something seems a bit small.

## Pistas
- RSA [tutorial](https://en.wikipedia.org/wiki/RSA_(cryptosystem))
- How could having too small an e affect the security of this 2048 bit key?
- Make sure you don't lose precision, the numbers are pretty big (besides the e value)

## Solución
```python
>>> from Crypto.Util.number import long_to_bytes
>>> from gmpy2 import *
>>> gmpy2.get_context().precision=2048
>>> e = 3
>>> c = 2205316413931134031074603746928247799030155221252519872649649212867614751848436763801274360463406171277838056821437115883619169702963504606017565783537203207707757768473109845162808575425972525116337319108047893250549462147185741761825125
>>> r, t = iroot(c,e)
>>> t
True
>>> r
mpz(13016382529449106065894479374027604750406953699090365388202874238148389207291005)
>>> long_to_bytes(r)
b'picoCTF{n33d_a_lArg3r_e_606ce004}'

```

## Bandera
picoCTF{n33d_a_lArg3r_e_606ce004}

## Notas adicionales
gymp2
pycryptodome

## Referencias
None