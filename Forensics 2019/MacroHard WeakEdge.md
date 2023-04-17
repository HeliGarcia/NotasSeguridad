# MacroHard WeakEdge

## Descripción
I've hidden a flag in this file. Can you find it? [Forensics is fun.pptm](https://mercury.picoctf.net/static/52da699e0f203321c7c90ab56ea912d8/Forensics is fun.pptm)

## Pistas
- None

## Solución
```bash
┌──(kali㉿kali)-[~/picoCTF/forensics/macros]
└─$ ls
'[Content_Types].xml'   docProps  'Forensics is fun.pptm'   ppt   _rels

┌──(kali㉿kali)-[~/picoCTF/forensics/macros]
└─$ cd ppt              

┌──(kali㉿kali)-[~/picoCTF/forensics/macros/ppt]
└─$ cd slideMasters 

┌──(kali㉿kali)-[~/…/forensics/macros/ppt/slideMasters]
└─$ ls
hidden  _rels  slideMaster1.xml

┌──(kali㉿kali)-[~/…/forensics/macros/ppt/slideMasters]
└─$ cat hidden       
Z m x h Z z o g c G l j b 0 N U R n t E M W R f d V 9 r b j B 3 X 3 B w d H N f c l 9 6 M X A 1 f Q                                                                                                                                          
┌──(kali㉿kali)-[~/…/forensics/macros/ppt/slideMasters]
└─$ cat hidden | tr -d ' ' | base64 -d
flag: picoCTF{D1d_u_kn0w_ppts_r_z1p5}

```

## Bandera
picoCTF{D1d_u_kn0w_ppts_r_z1p5}

## Notas adicionales
macros
tree
unzip

## Referencias
None