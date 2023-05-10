# b00tl3gRSA2
## Descripción
In RSA d is a lot bigger than e, why don't we use d to encrypt instead of e? Connect with `nc jupiter.challenges.picoctf.org 18243`.

## Pistas
- What is e generally?

## Solución
```python
>>> e = 65537
>>> c = 44341769988312655701807812216657753060566205683931620423483822093521294714241176254609785355675527466288225767450823875001097311512468484280532459556697877452997513482145214467139173665456058513604388551547181620033036526280958376875935149840725942948755612449494750056090617215122551272346491517310166498677
>>> n = 112805153021926830234521511522546830616341031253355580948940237168089628435250699665468762130591489141800070097966427854807711714101033104547942101757186641163056808895133411855785136984119186833560518397254730139219011410551445071914507009275789971554773171334223203908799250758093382782445148083747827258139
>>> m = pow(c,e,n)
>>> m
180638594769037903267909311328535969949661653466129492033745533
>>> long_to_bytes(m)
b'picoCTF{bad_1d3a5_4783252}'

```

## Bandera
picoCTF{bad_1d3a5_4783252}

## Notas adicionales
gymp2
pycryptodome

## Referencias
None