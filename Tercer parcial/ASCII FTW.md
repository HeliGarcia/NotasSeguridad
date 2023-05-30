# ASCII FTW

## Descripción
This program has constructed the flag using hex ascii values. Identify the flag text by disassembling the program. You can download the file from [here](https://artifacts.picoctf.net/c/508/asciiftw).

## Pistas
- The combined range of hex-ascii for English alphabets and numerical digits is from 30 to 7A.
- Online hex-ascii converters can be helpful.

## Solución
```bash
┌──(kali㉿kali)-[~/picoCTF/tercerparcial/asciiftw]
└─$ cat asciiftw 
@@@@�▒▒▒XX��   pp�-�=�=`h�-�=�=�888 XXXDDS�td888 P�td      DDQ�tdR�td�-�=�=PP/lib64/ld-linux-x86-64.so.2GNU�GNU��-���
  wI?^����UGNU��e�mZ 
                     2v � #"libc.so.6__stack_chk_failprintf__cxa_finalize__libc_start_mainGLIBC_2.2.5GLIBC_2.4_ITM_�H�=��2/��H�=Y/H�R/H9�tH�/H��t�������H�=)/H�5"/H)�H��H��?H��H�H��tH��.H����fD�����=�.u+UH�=�.H��t��H���PTL�H�
                                                                                                 H�=�.� ����d�����.]������w�����UH��H��0dH�%(H�E�1��E�p�E�i�E�c�E�o�E�C�E�T�E�F�E�{�E�A�E�S�E�C�E�I�E�I�E�_�E�I�E�S�E�_�E�E�E�A�E�S�E���V����H�E�dH3%(t�1�����f.�D��AWL�=c+AVI��AUI��ATA��UH�-T+SL)�H������H��t1��L��L��D��A��H��H9�u�H�[]A\A]A^A_�ff.������H�H��The flag starts with %x
D���x0����@����`���`I���� ��������8zRx
                                     ����/D$4����0F▒J
�                                                    �?▒:*3$"\����t���� �q����E�C
D�(���eF�I▒�E �E(�D0�H8�G@n8A0A(B B▒B�P���` 
��▒����o���
�
 ▒�?0(� ������o8���o���o(���o�=0@GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0▒8X|��(      8
h
 (
 P`��   h �=�=�=▒�?@▒@�
                       ��! 7▒@F�=m`y�=������l!����=��=��=�  �▒�?�
                                                                 � � @3@�:Vj�@� @� �@e�▒▒@��/�▒@�i��@�"crtstuff.cderegister_tm_clones__do_global_dtors_auxcompleted.8061__do_global_dtors_aux_fini_array_entryframe_dummy__frame_dummy_init_array_entryasciiftw.c__FRAME_END____init_array_end_DYNAMIC__init_array_start__GNU_EH_FRAME_HDR_GLOBAL_OFFSET_TABLE___libc_csu_fini_ITM_deregisterTMCloneTable_edata__stack_chk_fail@@GLIBC_2.4printf@@GLIBC_2.2.5__libc_start_main@@GLIBC_2.2.5__data_start__gmon_start____dso_handle_IO_stdin_used__libc_csu_init__bss_startmain__TMC_END___ITM_registerTMCloneTable__cxa_finalize@@GLIBC_2.2.5.symtab.strtab.shstrtab.interp.note.gnu.property.note.gnu.build-id.note.ABI-tag.gnu.hash.dynsym.dynstr.gnu.version.gnu.version_r.rela.dyn.rela.plt.init.plt.got.plt.sec.text.fini.rodata.eh_frame_hdr.eh_frame.init_array.fini_array.dynamic.data.bss.comment▒▒#886XX$I|| W���o��a
                                                                                         ��▒i���q���o((~���o88�hh▒��  �    D�h ������=�-��?�@0
                         @00+@00▒       p6$�8▒   
```

## Bandera
picoCTF{}

## Notas adicionales
ASCII
Hex

## Referencias
None