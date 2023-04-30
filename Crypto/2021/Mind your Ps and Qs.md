# Mind your Ps and Qs

## Descripción
In RSA, a small `e` value can be problematic, but what about `N`? Can you decrypt this? [values](https://mercury.picoctf.net/static/3cfeb09681369c26e3f19d886bc1e5d9/values)

## Pistas
- Bits are expensive, I used only a little bit over 100 to save money

## Solución
```python
>>> from Crypto.Util.number import inverse, long_to_bytes
>>> p = 1617549722683965197900599011412144490161
>>> q = 475693130177488446807040098678772442581573
>>> n = 65537
>>> p * q == n
False
>>> n = 769457290801263793712740792519696786147248001937382943813345728685422050738403253
>>> p * q == n
True
>>> tn = (p-1)*(q-1)
>>> e = 65537
>>> c = 8533139361076999596208540806559574687666062896040360148742851107661304651861689
>>> d = inverse(e,tn)
>>> m = pow(c,d,n)
>>> m
13016382529449106065927291425342535437996222135352905256639629442503647501498237
>>> long_to_bytes(m)
b'picoCTF{sma11_N_n0_g0od_45369387}'

```

## Bandera
picoCTF{sma11_N_n0_g0od_45369387}

## Notas adicionales
factordb
RSA

## Referencias
[factordb](http://www.factordb.com/index.php?query=769457290801263793712740792519696786147248001937382943813345728685422050738403253)