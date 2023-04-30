# basic-mod1

## Descripción
We found this weird message being passed around on the servers, we think we have a working decryption scheme. Download the message [here](https://artifacts.picoctf.net/c/128/message.txt). Take each number mod 37 and map it to the following character set: 0-25 is the alphabet (uppercase), 26-35 are the decimal digits, and 36 is an underscore. Wrap your decrypted message in the picoCTF flag format (i.e. `picoCTF{decrypted_message}`)

## Pistas
- Do you know what `mod 37` means?
- `mod 37` means modulo 37. It gives the remainder of a number after being divided by 37.

## Solución
```python
f = open("message.txt").read().split()
flag = ''
print(f)

for n in f:
	n = int(n) % 37
	if n >= 0 and n <= 25:
		c = chr(n+65)
	elif n >=26 and n <= 35:
		c = chr(n+22)
	else: c = '_'
	flag += c

print(flag)
```
['165', '248', '94', '346', '299', '73', '198', '221', '313', '137', '205', '87', '336', '110', '186', '69', '223', '213', '216', '216', '177', '138']
R0UND_N_R0UND_B6B25531

## Bandera
picoCTF{R0UND_N_R0UND_B6B25531}

## Notas adicionales
python

## Referencias
None