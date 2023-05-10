# Need For Speed

## Descripción
The name of the game is [speed](https://www.youtube.com/watch?v=8piqd2BWeGI). Are you quick enough to solve this problem and keep it above 50 mph? [need-for-speed](https://jupiter.challenges.picoctf.org/static/27dd5548b14661f65ce3ac6a8a8f575b/need-for-speed).

## Pistas
- What is the final key?

## Solución
```bash
End of assembler dump.
(gdb) call (int) get_key()
Creating key...
Finished
$1 = 9
(gdb) call (int) print_flag
$2 = 1430259884
(gdb) call (int) print_flag()
Printing flag:
PICOCTF{Good job keeping bus #1f2ac4ec speeding along!}
$3 = 56

```

## Bandera
PICOCTF{Good job keeping bus#1f2ac4ecspeeding along!}

## Notas adicionales
x86 Assembly 
gdb
Debugger

## Referencias
[Debugging with GDB](https://sourceware.org/gdb/current/onlinedocs/gdb.html/)