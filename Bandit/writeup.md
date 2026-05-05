# OverTheWire - Bandit

## Level 0
credential : bandit0:bandit0
```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```
And find the password for bandit1
```bash
bandit0@bandit:~$ cat readme
Congratulations on your first steps into the bandit game!!
Please make sure you have read the rules at https://overthewire.org/rules/
If you are following a course, workshop, walkthrough or other educational activity,
please inform the instructor about the rules as well and encourage them to
contribute to the OverTheWire community so we can keep these games free!

The password you are looking for is: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
```
## Level0 -> Level1 
credential : bandit1:ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
```bash
┌──(kali㉿kali)-[~]
└─$ ssh bandit1@bandit.labs.overthewire.org -p 2220
```
And find the password for bandit2
```bash
bandit1@bandit:~$ cat ./-
263JGJPfgU6LtdEvgfWU1XP5yac29mFx
```
## Level1 -> Level2
credential: bandit2:263JGJPfgU6LtdEvgfWU1XP5yac29mFx
```bash
┌──(kali㉿kali)-[~]
└─$ ssh bandit2@bandit.labs.overthewire.org -p 2220

bandit2@bandit:~$ cat ./'--spaces in this filename--'
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
```
## Level2 -> Level3 
credential: bandit3:MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
```bash
┌──(kali㉿kali)-[~]
└─$ ssh bandit3@bandit.labs.overthewire.org -p 2220
bandit3@bandit:~$ cat inhere/...Hiding-From-You 
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
```

## Level3 -> Level 4
credential: bandit4:2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
```bash
┌──(kali㉿kali)-[~]
└─$ ssh bandit4@bandit.labs.overthewire.org -p 2220
bandit4@bandit:~/inhere$ file ./*
./-file00: data
./-file01: data
./-file02: data
./-file03: DOS executable (COM), start instruction 0x8c887e10 c3ee96c9
./-file04: data
./-file05: data
./-file06: data
./-file07: ASCII text
./-file08: data
./-file09: data
bandit4@bandit:~/inhere$ cat ./-file07
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
```
## Level4 -> Level5 
credential: bandit5:4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
```bash
┌──(kali㉿kali)-[~]
└─$ ssh bandit5@bandit.labs.overthewire.org -p 2220
bandit5@bandit:~/inhere$ find . -type f -size 1033c
./maybehere07/.file2
bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
```
## Level5 -> Level6
credential: bandit6:HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
```bash
┌──(kali㉿kali)-[~]
└─$ ssh bandit5@bandit.labs.overthewire.org -p 2220
bandit5@bandit:~/inhere$ find . -type f -size 1033c
./maybehere07/.file2
bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
```
## Level6 -> Level7
credential: bandit7:morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
```bash
┌──(kali㉿kali)-[~]
└─$ ssh bandit6@bandit.labs.overthewire.org -p 2220
bandit6@bandit:~$ find / -type f -size 33c -user 'bandit7' -group 'bandit6' 2>/dev/null
/var/lib/dpkg/info/bandit7.password
bandit6@bandit:~$ ls -la /var/lib/dpkg/info/bandit7.password
-rw-r----- 1 bandit7 bandit6 33 Apr  3 15:18 /var/lib/dpkg/info/bandit7.password
bandit6@bandit:~$ id
uid=11006(bandit6) gid=11006(bandit6) groups=11006(bandit6)
bandit6@bandit:~$ cat /var/lib/dpkg/info/bandit7.password
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
```
## Level7 -> level8
credential: bandit8:dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
```bash
┌──(kali㉿kali)-[~]
└─$ ssh bandit7@bandit.labs.overthewire.org -p 2220
bandit7@bandit:~$ cat data.txt | grep millionth
millionth	dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
```
## Level8 -> Level9
credential: bandit9:4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
```bash
┌──(kali㉿kali)-[~]
└─$ ssh bandit8@bandit.labs.overthewire.org -p 2220
bandit8@bandit:~$ cat data.txt | sort -n | uniq -c | grep -v "10"
      1 4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
```

## Level9 -> level10
cradential: bandit10:FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
```bash
┌──(kali㉿kali)-[~]
└─$ ssh bandit9@bandit.labs.overthewire.org -p 2220
bandit9@bandit:~$ strings data.txt | grep "=="
========== the
========== password
========== is
========== FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
```
## Level10 -> level11
cradential: bandit11:dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
```bash
┌──(kali㉿kali)-[~]
└─$ ssh bandit10@bandit.labs.overthewire.org -p 2220
bandit10@bandit:~$ cat data.txt 
VGhlIHBhc3N3b3JkIGlzIGR0UjE3M2ZaS2IwUlJzREZTR3NnMlJXbnBOVmozcVJyCg==
bandit10@bandit:~$ cat data.txt | base64 -d
The password is dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
```

## Level11 -> level12
cradential: bandit12:7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4
```bash
┌──(kali㉿kali)-[~]
└─$ ssh bandit11@bandit.labs.overthewire.org -p 2220
bandit11@bandit:~$ cat data.txt | tr  -t 'a-z' 'n-za-m' | tr  -t 'A-Z' 'N-ZA-M'
The password is 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4
```
## Level12 -> level13
The command is using `xxd` to recover the hexdump file and multiple de-compress the file using `gunzip,bzip2,tar`

cradential: bandit13:FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn
```bash
┌──(kali㉿kali)-[~]
└─$ ssh bandit12@bandit.labs.overthewire.org -p 2220
bandit12@bandit:/tmp/dodol$ cat data8
The password is FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn
```
## Level13 -> level14
```bash
┌──(kali㉿kali)-[~]
└─$ ssh bandit13@bandit.labs.overthewire.org -p 2220
backend: gibson-0
bandit13@bandit.labs.overthewire.org's password:
bandit13@bandit:~$ cat HINT
If you have trouble with this level, note the following:
1) As for all other levels, this level has a website with information:
   https://overthewire.org/wargames/bandit/bandit14.html
2) No, the level is not broken. To verify, see:
   https://status.overthewire.org/
3) The current version of OverTheWire prevents logging in from one
   level to another via localhost. Log out, and see 1)
4) If you get errors, read the error message on your screen.
   We mean it!
```
Download the sshkey.private using scp 
```bash
┌──(kali㉿kali)-[/tmp]
└─$ scp -P 2220 bandit13@bandit.labs.overthewire.org:~/sshkey.private .
                         _                     _ _ _   
                        | |__   __ _ _ __   __| (_) |_ 
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_ 
                        |_.__/ \__,_|_| |_|\__,_|_|\__|
                                                       

                      This is an OverTheWire game server. 
            More information on http://www.overthewire.org/wargames

backend: gibson-0
bandit13@bandit.labs.overthewire.org's password: 
sshkey.private
```


## Level14 -> level15

credential for level15: bandit15:8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo
Change permission to sshkey.private
```bash
┌──(kali㉿kali)-[/tmp]
└─$ chmod 600 sshkey.private
```
Remote using sshkey.private
```bash
┌──(kali㉿kali)-[/tmp]
└─$ ssh -i sshkey.private bandit14@bandit.labs.overthewire.org -p 2220
bandit14@bandit:~$ cat /etc/bandit_pass/bandit14
MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS
```
Connect to port 30000
```bash
bandit14@bandit:~$ nc  localhost 30000
MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS
Correct!
8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo
```

## Level15 -> level16

Credential bandit16:kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx
```bash
┌──(kali㉿kali)-[~]
└─$ ssh bandit15@bandit.labs.overthewire.org -p 2220
```
Connect to port 30001 using SSL/TLS
```bash
bandit15@bandit:~$ openssl s_client localhost:30001
CONNECTED(00000003)
Can't use SSL_get_servername
depth=0 CN = SnakeOil
verify error:num=18:self-signed certificate
verify return:1
depth=0 CN = SnakeOil
verify return:1
---
Certificate chain
 0 s:CN = SnakeOil
   i:CN = SnakeOil
   a:PKEY: rsaEncryption, 4096 (bit); sigalg: RSA-SHA256
   v:NotBefore: Jun 10 03:59:50 2024 GMT; NotAfter: Jun  8 03:59:50 2034 GMT
---
Server certificate
-----BEGIN CERTIFICATE-----
MIIFBzCCAu+gAwIBAgIUBLz7DBxA0IfojaL/WaJzE6Sbz7cwDQYJKoZIhvcNAQEL
BQAwEzERMA8GA1UEAwwIU25ha2VPaWwwHhcNMjQwNjEwMDM1OTUwWhcNMzQwNjA4
MDM1OTUwWjATMREwDwYDVQQDDAhTbmFrZU9pbDCCAiIwDQYJKoZIhvcNAQEBBQAD
ggIPADCCAgoCggIBANI+P5QXm9Bj21FIPsQqbqZRb5XmSZZJYaam7EIJ16Fxedf+
jXAv4d/FVqiEM4BuSNsNMeBMx2Gq0lAfN33h+RMTjRoMb8yBsZsC063MLfXCk4p+
09gtGP7BS6Iy5XdmfY/fPHvA3JDEScdlDDmd6Lsbdwhv93Q8M6POVO9sv4HuS4t/
jEjr+NhE+Bjr/wDbyg7GL71BP1WPZpQnRE4OzoSrt5+bZVLvODWUFwinB0fLaGRk
GmI0r5EUOUd7HpYyoIQbiNlePGfPpHRKnmdXTTEZEoxeWWAaM1VhPGqfrB/Pnca+
vAJX7iBOb3kHinmfVOScsG/YAUR94wSELeY+UlEWJaELVUntrJ5HeRDiTChiVQ++
wnnjNbepaW6shopybUF3XXfhIb4NvwLWpvoKFXVtcVjlOujF0snVvpE+MRT0wacy
tHtjZs7Ao7GYxDz6H8AdBLKJW67uQon37a4MI260ADFMS+2vEAbNSFP+f6ii5mrB
18cY64ZaF6oU8bjGK7BArDx56bRc3WFyuBIGWAFHEuB948BcshXY7baf5jjzPmgz
mq1zdRthQB31MOM2ii6vuTkheAvKfFf+llH4M9SnES4NSF2hj9NnHga9V08wfhYc
x0W6qu+S8HUdVF+V23yTvUNgz4Q+UoGs4sHSDEsIBFqNvInnpUmtNgcR2L5PAgMB
AAGjUzBRMB0GA1UdDgQWBBTPo8kfze4P9EgxNuyk7+xDGFtAYzAfBgNVHSMEGDAW
gBTPo8kfze4P9EgxNuyk7+xDGFtAYzAPBgNVHRMBAf8EBTADAQH/MA0GCSqGSIb3
DQEBCwUAA4ICAQAKHomtmcGqyiLnhziLe97Mq2+Sul5QgYVwfx/KYOXxv2T8ZmcR
Ae9XFhZT4jsAOUDK1OXx9aZgDGJHJLNEVTe9zWv1ONFfNxEBxQgP7hhmDBWdtj6d
taqEW/Jp06X+08BtnYK9NZsvDg2YRcvOHConeMjwvEL7tQK0m+GVyQfLYg6jnrhx
egH+abucTKxabFcWSE+Vk0uJYMqcbXvB4WNKz9vj4V5Hn7/DN4xIjFko+nREw6Oa
/AUFjNnO/FPjap+d68H1LdzMH3PSs+yjGid+6Zx9FCnt9qZydW13Miqg3nDnODXw
+Z682mQFjVlGPCA5ZOQbyMKY4tNazG2n8qy2famQT3+jF8Lb6a4NGbnpeWnLMkIu
jWLWIkA9MlbdNXuajiPNVyYIK9gdoBzbfaKwoOfSsLxEqlf8rio1GGcEV5Hlz5S2
txwI0xdW9MWeGWoiLbZSbRJH4TIBFFtoBG0LoEJi0C+UPwS8CDngJB4TyrZqEld3
rH87W+Et1t/Nepoc/Eoaux9PFp5VPXP+qwQGmhir/hv7OsgBhrkYuhkjxZ8+1uk7
tUWC/XM0mpLoxsq6vVl3AJaJe1ivdA9xLytsuG4iv02Juc593HXYR8yOpow0Eq2T
U5EyeuFg5RXYwAPi7ykw1PW7zAPL4MlonEVz+QXOSx6eyhimp1VZC11SCg==
-----END CERTIFICATE-----
subject=CN = SnakeOil
issuer=CN = SnakeOil
---
No client certificate CA names sent
Peer signing digest: SHA256
Peer signature type: RSA-PSS
Server Temp Key: X25519, 253 bits
---
SSL handshake has read 2103 bytes and written 373 bytes
Verification error: self-signed certificate
---
New, TLSv1.3, Cipher is TLS_AES_256_GCM_SHA384
Server public key is 4096 bit
Secure Renegotiation IS NOT supported
Compression: NONE
Expansion: NONE
No ALPN negotiated
Early data was not sent
Verify return code: 18 (self-signed certificate)
---
---
Post-Handshake New Session Ticket arrived:
SSL-Session:
    Protocol  : TLSv1.3
    Cipher    : TLS_AES_256_GCM_SHA384
    Session-ID: 85C7A03B27455691E19AB7C4C0B5D63A7138E2127C24314DE656BD690C4716AF
    Session-ID-ctx: 
    Resumption PSK: E0D029676C6DF87D33AE916E2FBF650AE2504AB4656CAD97FC51D5D687E13A6DFAB12400698FE08F615F005931413638
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    TLS session ticket lifetime hint: 300 (seconds)
    TLS session ticket:
    0000 - 8f 5c e1 57 40 ed ab 16-41 2a 79 fb 80 49 37 a8   .\.W@...A*y..I7.
    0010 - c3 af 0d 5f ae ce 1f d3-9e d3 7f af 50 d9 f2 00   ..._........P...
    0020 - 19 e5 08 63 8e c3 4e 4a-c1 67 91 7e ec 4a cd 93   ...c..NJ.g.~.J..
    0030 - 38 a2 11 7a 3f 7f 2a 3a-be b1 d3 b1 cb 24 10 62   8..z?.*:.....$.b
    0040 - 1c 42 1f 6b 28 70 a4 24-b6 54 14 d7 bb be 2d 60   .B.k(p.$.T....-`
    0050 - bd 26 bc 2c b6 19 6b e6-dd d6 0f 6b 69 19 aa f8   .&.,..k....ki...
    0060 - ee 3d 1d 10 70 3b a1 58-77 ab bf 26 7a 9b c8 de   .=..p;.Xw..&z...
    0070 - 16 54 85 2c 9d b7 9c 60-e6 f6 a8 9b 38 71 51 42   .T.,...`....8qQB
    0080 - 9e e3 ec f6 4d a3 21 d4-bf f3 cd c8 85 13 5d 88   ....M.!.......].
    0090 - fa 67 3d 03 1b f1 3a c9-6b 3c 11 69 ae d8 25 21   .g=...:.k<.i..%!
    00a0 - f5 71 a0 66 09 6b 5e 17-b3 a4 63 35 0a 2c b0 e8   .q.f.k^...c5.,..
    00b0 - 83 a9 18 31 67 30 36 ab-52 d9 c4 e1 1a 45 04 e2   ...1g06.R....E..
    00c0 - e5 ef 59 27 39 9f ec 23-b5 f7 02 74 5b ee bf b6   ..Y'9..#...t[...
    00d0 - e8 f7 31 c8 08 fb 2b f1-e7 55 65 8c ee e0 35 a0   ..1...+..Ue...5.

    Start Time: 1777966055
    Timeout   : 7200 (sec)
    Verify return code: 18 (self-signed certificate)
    Extended master secret: no
    Max Early Data: 0
---
read R BLOCK
---
Post-Handshake New Session Ticket arrived:
SSL-Session:
    Protocol  : TLSv1.3
    Cipher    : TLS_AES_256_GCM_SHA384
    Session-ID: 51F7800975A3E8B57E968EE99A95D1A96E1025A6624026D37F4D8648CDFE4E63
    Session-ID-ctx: 
    Resumption PSK: 3AAAC19E880FDA69688D5A4CDB7C9C29EA15868B78223DBD2237ADEBA52038525470C10DB253C7591D02C7A2268B2325
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    TLS session ticket lifetime hint: 300 (seconds)
    TLS session ticket:
    0000 - 8f 5c e1 57 40 ed ab 16-41 2a 79 fb 80 49 37 a8   .\.W@...A*y..I7.
    0010 - 02 2d 07 68 22 a9 f3 c4-71 12 36 39 73 99 aa 2a   .-.h"...q.69s..*
    0020 - 69 df 94 9e 45 d0 57 16-6d 02 66 2f fe 1f 5e e9   i...E.W.m.f/..^.
    0030 - 4a 18 ee 77 59 50 cf 62-f8 92 1f 5a a9 ea 35 33   J..wYP.b...Z..53
    0040 - 67 2b 3b e6 4a d9 d9 c2-22 10 af 8b 9b 9f 73 c2   g+;.J...".....s.
    0050 - 8d 01 9c db d1 c4 41 4c-98 85 c1 7b 24 4f b6 ea   ......AL...{$O..
    0060 - a9 fd 97 fc 2f ad b1 6e-69 50 bd 30 ba bc 8b 98   ..../..niP.0....
    0070 - 60 9c 2f d1 a6 b2 e2 7c-af e3 a0 3d 81 77 96 16   `./....|...=.w..
    0080 - e7 21 d6 1a 6c 75 8c 73-30 e1 e7 f0 a9 8b 97 92   .!..lu.s0.......
    0090 - 3e b6 f0 88 a3 72 c8 eb-bc 8d 4d de a8 1e 50 c9   >....r....M...P.
    00a0 - 02 38 eb e5 75 8d 4b 59-7e ab 2f bd 08 c2 11 10   .8..u.KY~./.....
    00b0 - e7 39 da cd 5b 09 78 ce-56 c8 11 97 ef 12 59 f9   .9..[.x.V.....Y.
    00c0 - 26 33 62 d3 45 25 b2 4e-ca ea 09 31 d5 96 d9 f8   &3b.E%.N...1....
    00d0 - 2e 1a 8b 6b dd 3f fe b4-eb da ef fa 48 b0 c5 34   ...k.?......H..4

    Start Time: 1777966055
    Timeout   : 7200 (sec)
    Verify return code: 18 (self-signed certificate)
    Extended master secret: no
    Max Early Data: 0
---
read R BLOCK
8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo
Correct!
kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx
```





