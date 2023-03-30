# m00nwalk

## Descripción
Decode this [message](https://jupiter.challenges.picoctf.org/static/14393e18d98fedbaedbc28896d7ef31a/message.wav) from the moon.

## Pistas
- How did pictures from the moon landing get sent back to Earth?
- What is the CMU mascot?, that might help select a RX option
-
## Solución
```bash
┌──(kali㉿kali)-[~/picoCTF/forensics/moonwalk]
└─$ sstv
usage: sstv [-h] [-d AUDIO_FILE] [-o OUTPUT_FILE] [-s SKIP] [-V] [--list-modes] [--list-audio-formats]
            [--list-image-formats]

options:
  -h, --help            show this help message and exit
  -d AUDIO_FILE, --decode AUDIO_FILE
                        decode SSTV audio file
  -o OUTPUT_FILE, --output OUTPUT_FILE
                        save output image to custom location
  -s SKIP, --skip SKIP  time in seconds to start decoding signal at
  -V, --version         show program's version number and exit
  --list-modes          list supported SSTV modes
  --list-audio-formats  list supported audio file formats
  --list-image-formats  list supported image file formats

examples:
  Decode local SSTV audio file named 'audio.ogg' to 'result.png':
    $ sstv -d audio.ogg

  Decode SSTV audio file in /tmp to './image.jpg':
    $ sstv -d /tmp/signal.wav -o ./image.jpg

  Start decoding SSTV signal at 50.5 seconds into the audio
    $ sstv -d audio.ogg -s 50.50
                                                                                                             
┌──(kali㉿kali)-[~/picoCTF/forensics/moonwalk]
┌──(kali㉿kali)-[~/picoCTF/forensics/moonwalk]
└─$ sstv -d message.wav -o flag.png
[sstv] Searching for calibration header... Found!    
[sstv] Detected SSTV mode Scottie 1
[sstv] Decoding image...   [###########################################################################] 100%
[sstv] Drawing image data...
[sstv] ...Done!
                                                                                                             
┌──(kali㉿kali)-[~/picoCTF/forensics/moonwalk]
└─$ ls
flag.png  message.wav

```

## Bandera
picoCTF{beep_boop_im_in_space}

## Notas adicionales
sstv

## Referencias
[sstv](https://github.com/colaclanth/sstv)