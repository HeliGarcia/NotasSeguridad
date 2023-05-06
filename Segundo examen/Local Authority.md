# Local Authority 

## Descripción
Can you get the flag? Go to this [website](http://saturn.picoctf.net:64710/) and see what you can discover.

## Pistas
- How is the password checked on this website?

## Solución
```javascript
function checkPassword(username, password)
{
  if( username === 'admin' && password === 'strongPassword098765' )
  {
    return true;
  }
  else
  {
    return false;
  }
}
//Al introducir el admin y password, la bandera sale. 
```

## Bandera
picoCTF{j5_15_7r4n5p4r3n7_b0c2c9cb}

## Notas adicionales
Inspect
JavaScript
HTML

## Referencias
None