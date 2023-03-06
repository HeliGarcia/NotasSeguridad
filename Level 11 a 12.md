# Level 12

## Objetivo
The password for the next level is stored in the file **data.txt**, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)
## Datos de acceso
**bandit.labs.overthewire.org**
**bandit11**

## Solución

```bash
bandit12@bandit:~$ cat data.txt | xxd -r
��
 �cdata2.bin<��BZh91AY&SY��q����Y�ůc���s����|�����������������;,YA�dz�@�hi�h4dz�=F��CA�4��z��<��z�hy@�=@����@
�@z��h44�d�hb�Ŭ��j��v��y�TfSW#w�Iڃ`��ȔC��   �pUf���zSVG($�����ZK(&*��nkxM�����j�S��$�:|�ہҺ/��[�ӕ�>2���ұ)P�&���>ڗ����~��@��A�xo���3<�
����OB�ݤ�����O��"C[f�ўH��Q,-֤�V��(� a�l�^��˔�"�a0hVe��I/����q%p[��B&
X��e
    ��VHﹰ#
           �������;�`��(2�FL��*wr���R} �L�Mk����4��d��T�mg��GB���--��ĥzE^-�DξT*���ܑN$#-}�9��}<bandit12@bandit:~$
bandit12@bandit:~$ cat data.txt | xxd -r | file -
/dev/stdin: gzip compressed data, was "data2.bin", last modified: Wed Jan 11 19:18:38 2023, max compression, from Unix
bandit12@bandit:~$
bandit12@bandit:~$ cat data.txt | xxd -r | zcat | file -
/dev/stdin: bzip2 compressed data, block size = 900k
bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | file -
/dev/stdin: gzip compressed data, was "data4.bin", last modified: Wed Jan 11 19:18:38 2023, max compression, from Unix
bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | zcat | file -
/dev/stdin: POSIX tar archive (GNU)
bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | zcat | tar xO | file -
/dev/stdin: POSIX tar archive (GNU)
bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | zcat | tar xO | tar xO | file -
/dev/stdin: bzip2 compressed data, block size = 900k
bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | zcat | tar xO | tar xO | bzcat | file -                                                                             /dev/stdin: POSIX tar archive (GNU)
bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | zcat | tar xO | tar xO | bzcat | tar xO | file -
/dev/stdin: gzip compressed data, was "data9.bin", last modified: Wed Jan 11 19:18:38 2023, max compression, from Unix
bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | zcat | tar xO | tar xO | bzcat | tar xO | zcat | file -
/dev/stdin: ASCII text
bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | zcat | tar xO | tar xO | bzcat | tar xO | zcat
The password is wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw
```
## Datos adicionales
| zcat | | Descomprime archivos gzip |
| bzcat | | Descomprime archivos bzip2 |
| tar xO | | Descomprime archivos tar |
| xxd -r | | Quita el vaciado hexadecimal |
| xxd | Realiza un vaciado hexadecimal |
## Referencias
Linux Comand Line
[Hex dump on Wikipedia](https://en.wikipedia.org/wiki/Hex_dump)