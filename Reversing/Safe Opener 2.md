# asm3

## Descripción
What can you do with this file? I forgot the key to my safe but this [file](https://artifacts.picoctf.net/c/292/SafeOpener.class) is supposed to help me with retrieving the lost key. Can you help me unlock my safe?

## Pistas
- Download and try to decompile the file.

## Solución
```bash
public class SafeOpener
{
    public static void main(final String[] args) throws IOException {
        final BufferedReader keyboard = new BufferedReader(new InputStreamReader(System.in));
        final Base64.Encoder encoder = Base64.getEncoder();
        String encodedkey = "";
        String key = "";
        for (int i = 0; i < 3; ++i) {
            System.out.print("Enter password for the safe: ");
            key = keyboard.readLine();
            encodedkey = encoder.encodeToString(key.getBytes());
            System.out.println(encodedkey);
            final boolean isOpen = openSafe(encodedkey);
            if (isOpen) {
                break;
            }
            System.out.println("You have  " + (2 - i) + " attempt(s) left");
        }
    }
    
    public static boolean openSafe(final String password) {
        final String encodedkey = "picoCTF{SAf3_0p3n3rr_y0u_solv3d_it_0e57c117}";
        if (password.equals(encodedkey)) {
            System.out.println("Sesame open");
            return true;
        }
        System.out.println("Password is incorrect\n");
        return false;
    }
}

     
```

## Bandera
picoCTF{SAf3_0p3n3rr_y0u_solv3d_it_0e57c117}

## Notas adicionales

Java
Reversing

## Referencias
None