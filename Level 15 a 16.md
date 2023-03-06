# Level 15

## Objetivo
The password for the next level can be retrieved by submitting the password of the current level to **port 30001 on localhost** using SSL encryption.

**Helpful note: Getting “HEARTBEATING” and “Read R BLOCK”? Use -ign_eof and read the “CONNECTED COMMANDS” section in the manpage. Next to ‘R’ and ‘Q’, the ‘B’ command also works in this version of that command…**

## Datos de acceso
**bandit.labs.overthewire.org**
**bandit15**

## Solución

```shell
bandit15@bandit:~$ openssl s_client -connect localhost:30001
CONNECTED(00000003)
Can't use SSL_get_servername
depth=0 CN = localhost
verify error:num=18:self-signed certificate
verify return:1
depth=0 CN = localhost
verify error:num=10:certificate has expired
notAfter=Feb 21 06:20:29 2023 GMT
verify return:1
depth=0 CN = localhost
notAfter=Feb 21 06:20:29 2023 GMT
verify return:1
---
Certificate chain
 0 s:CN = localhost
   i:CN = localhost
   a:PKEY: rsaEncryption, 2048 (bit); sigalg: RSA-SHA1
   v:NotBefore: Feb 21 06:19:29 2023 GMT; NotAfter: Feb 21 06:20:29 2023 GMT
---
Server certificate
-----BEGIN CERTIFICATE-----
MIIDCzCCAfOgAwIBAgIEA7qUdzANBgkqhkiG9w0BAQUFADAUMRIwEAYDVQQDDAls
b2NhbGhvc3QwHhcNMjMwMjIxMDYxOTI5WhcNMjMwMjIxMDYyMDI5WjAUMRIwEAYD
VQQDDAlsb2NhbGhvc3QwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQDL
vM0gZzAHdXTeD5t4ruUJo/kRs4UAodA9XcqDhNtW464W0c55RqKLp921syy3Lvjr
8Q9WkqvCFX+efShMd8XnzbT/dyRrD+cZQnSiPJ3bwDdpwqfkl9h3mb609Kb5HI6R
JgogEyuRLJI+HKtr/wXHwo1vBZ0+yaPMX6sdkd6Hu5Ra0L5Q5+E5+3F/8QgvCeVE
hDRIOrh2a7jxykb8G6+xVC6jIZY0YfrZz6LrESyQau256pqyaQPqQoUWTlitxIql
Ym2Baw7vYDxmFZrvj0FkumC6NokX6K2G9bZ0DaKR/DspPdAC4oT81SawJvsBibdN
51VI6dxBn412ZS8bS155AgMBAAGjZTBjMBQGA1UdEQQNMAuCCWxvY2FsaG9zdDBL
BglghkgBhvhCAQ0EPhY8QXV0b21hdGljYWxseSBnZW5lcmF0ZWQgYnkgTmNhdC4g
U2VlIGh0dHBzOi8vbm1hcC5vcmcvbmNhdC8uMA0GCSqGSIb3DQEBBQUAA4IBAQA9
skxWNwZbedjaVTa5yMPUZQ4Nf5/LAAMtS5Q7mzGH5tdQsTGR0Z4n4eA4hzrmzHBF
MVRL5mR9n+sM5pIrKDa6f4zIc5ObxDyN19ie+3SFASCPz9tihK8Js2V8qsR6LHV1
pfD8DSG0hZPtUuK3Mfi+nWqQUFiiTGj30mb9vlS1sSWv5PGznou1gQ3ZfrDs7B4K
ZKZrllPIVV1CrlDw2Bv8Dc432LQuZAmKAjBd6FG0OAboU/WJMTwAfVjlKMtvC8tg
DZ3djSTprq6PrXlI0utw/MsMIh69b61BRXUuDvRxhU11SNmSI8aegjVL8KuK+Euh
sSLPTocV29SY1YXOwEQi
-----END CERTIFICATE-----
subject=CN = localhost
issuer=CN = localhost
---
No client certificate CA names sent
Peer signing digest: SHA256
Peer signature type: RSA-PSS
Server Temp Key: X25519, 253 bits
---
SSL handshake has read 1339 bytes and written 373 bytes
Verification error: certificate has expired
---
New, TLSv1.3, Cipher is TLS_AES_256_GCM_SHA384
Server public key is 2048 bit
Secure Renegotiation IS NOT supported
Compression: NONE
Expansion: NONE
No ALPN negotiated
Early data was not sent
Verify return code: 10 (certificate has expired)
---
---
Post-Handshake New Session Ticket arrived:
SSL-Session:
    Protocol  : TLSv1.3
    Cipher    : TLS_AES_256_GCM_SHA384
    Session-ID: F0D6039567A6524F225DF580D1493AC54A89B48AF7FA871A1137BFF5867D85A9
    Session-ID-ctx:
    Resumption PSK: 45D9947DB49BFBB520A67788D9740F12B20F45614C10525AEF33AC00CF15AF47260361D99B94CCB005A06C005EFB1C14
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    TLS session ticket lifetime hint: 7200 (seconds)
    TLS session ticket:
    0000 - ee ae 09 e4 56 06 6c 9e-c9 80 86 77 50 83 15 59   ....V.l....wP..Y
    0010 - fe 22 30 86 2d 9d a7 e4-2f e7 54 1a 17 1d 95 86   ."0.-.../.T.....
    0020 - 8f 13 58 2a 1f 27 e0 fe-16 e0 0d 16 4b 3e dd b6   ..X*.'......K>..
    0030 - db 8f ed 3c 30 11 19 cd-8b 94 c0 f9 6f 26 47 b4   ...<0.......o&G.
    0040 - 5c de ce d2 e3 87 af 01-c5 7d 9a 2f a0 7b 5f 30   \........}./.{_0
    0050 - 74 dc bd 04 5d 0e d0 f4-d0 9d 11 90 a9 5b 29 c1   t...]........[).
    0060 - 95 4f 33 b0 44 db 77 44-c9 1b 37 fe ff 09 b0 92   .O3.D.wD..7.....
    0070 - dc 4e 31 bd e5 ce dc e6-0a e0 88 86 f2 2a 3f 9b   .N1..........*?.
    0080 - 87 13 43 ac dc 16 68 f5-66 0b 8c 31 b3 6c 96 a2   ..C...h.f..1.l..
    0090 - d1 91 a5 c7 1d 2f 67 30-9f 9d 09 dc 3f 2d 29 ae   ...../g0....?-).
    00a0 - 76 18 ba fc 62 b6 17 8b-58 db 85 8b cd 8f 50 9a   v...b...X.....P.
    00b0 - b2 af 44 b2 5d 2a c8 91-9a 44 cf 1c ce e1 0b 7f   ..D.]*...D......
    00c0 - 3d ae df b1 08 6f b7 13-6a 90 93 54 34 f4 23 84   =....o..j..T4.#.

    Start Time: 1677007520
    Timeout   : 7200 (sec)
    Verify return code: 10 (certificate has expired)
    Extended master secret: no
    Max Early Data: 0
---
read R BLOCK
---
Post-Handshake New Session Ticket arrived:
SSL-Session:
    Protocol  : TLSv1.3
    Cipher    : TLS_AES_256_GCM_SHA384
    Session-ID: CC829E7D61B275C79F71918D3712456D6EB88C136A19DE27C5E457CFDC4A6A0D
    Session-ID-ctx:
    Resumption PSK: AD4D5C030ED210165FD62E1C00AFA789463D564727EF57A1DD82825A770D6EC66123A5DC7CD76E67F2DEB168E1BFA8C5
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    TLS session ticket lifetime hint: 7200 (seconds)
    TLS session ticket:
    0000 - ee ae 09 e4 56 06 6c 9e-c9 80 86 77 50 83 15 59   ....V.l....wP..Y
    0010 - c4 df 44 af 38 e0 0f 63-d8 21 a2 4f 2c ae 65 76   ..D.8..c.!.O,.ev
    0020 - d3 4f 81 80 58 91 fc 4e-59 b0 e1 3b 59 cd a2 74   .O..X..NY..;Y..t
    0030 - 3a af 4f f4 7f f5 ad 91-54 d1 7e 71 ed 31 ff 32   :.O.....T.~q.1.2
    0040 - 05 5c c5 68 92 a9 c6 f1-83 bf 47 3c 80 27 09 94   .\.h......G<.'..
    0050 - d9 c8 17 c3 cf b6 9e ec-71 07 a5 aa bf 2e 98 07   ........q.......
    0060 - 25 3f b3 64 62 59 21 b4-6d e9 93 e8 11 04 25 a6   %?.dbY!.m.....%.
    0070 - 1b 6f c5 87 7d 88 0b d6-84 8a 23 f6 eb 94 61 47   .o..}.....#...aG
    0080 - ec d1 8e 1a a6 ac 90 4a-c3 1a d2 c3 b7 f2 08 3f   .......J.......?
    0090 - 72 a2 20 da a2 f8 38 d1-9d 96 f7 94 4d 2b d9 54   r. ...8.....M+.T
    00a0 - 4a 42 b8 26 f8 3a 87 da-22 ad 8b 83 91 39 43 73   JB.&.:.."....9Cs
    00b0 - 5f 05 fa 7b b1 54 c1 85-e9 a3 a0 ab 91 78 7f b5   _..{.T.......x..
    00c0 - d1 23 1b 6a 10 f6 a1 aa-53 b0 77 91 74 c8 63 02   .#.j....S.w.t.c.

    Start Time: 1677007520
    Timeout   : 7200 (sec)
    Verify return code: 10 (certificate has expired)
    Extended master secret: no
    Max Early Data: 0
---
read R BLOCK
jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt
Correct!
JQttfApK4SeyHwDlI9SXGR50qclOAil1

closed
```

## Datos adicionales

## Referencias
