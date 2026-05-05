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

## Level16 -> level17
The credentials for the next level can be retrieved by submitting the password of the current level to a port on localhost in the range 31000 to 32000. First find out which of these ports have a server listening on them. Then find out which of those speak SSL/TLS and which don’t
Scan local port
```bash
┌──(kali㉿kali)-[~]
└─$ ssh bandit16@bandit.labs.overthewire.org -p 2220
PORT      STATE SERVICE
31046/tcp open  unknown
31518/tcp open  unknown
31691/tcp open  unknown
31790/tcp open  unknown
31960/tcp open  unknown
```

TLS on port 31518 and 31790 trying the 31790 return RSA
```bash
bandit16@bandit:~$ echo "kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx" | openssl s_client -connect localhost:31790 -quiet
Can't use SSL_get_servername
depth=0 CN = SnakeOil
verify error:num=18:self-signed certificate
verify return:1
depth=0 CN = SnakeOil
verify return:1
Correct!
-----BEGIN RSA PRIVATE KEY-----
MIIEogIBAAKCAQEAvmOkuifmMg6HL2YPIOjon6iWfbp7c3jx34YkYWqUH57SUdyJ
imZzeyGC0gtZPGujUSxiJSWI/oTqexh+cAMTSMlOJf7+BrJObArnxd9Y7YT2bRPQ
Ja6Lzb558YW3FZl87ORiO+rW4LCDCNd2lUvLE/GL2GWyuKN0K5iCd5TbtJzEkQTu
DSt2mcNn4rhAL+JFr56o4T6z8WWAW18BR6yGrMq7Q/kALHYW3OekePQAzL0VUYbW
JGTi65CxbCnzc/w4+mqQyvmzpWtMAzJTzAzQxNbkR2MBGySxDLrjg0LWN6sK7wNX
x0YVztz/zbIkPjfkU1jHS+9EbVNj+D1XFOJuaQIDAQABAoIBABagpxpM1aoLWfvD
KHcj10nqcoBc4oE11aFYQwik7xfW+24pRNuDE6SFthOar69jp5RlLwD1NhPx3iBl
J9nOM8OJ0VToum43UOS8YxF8WwhXriYGnc1sskbwpXOUDc9uX4+UESzH22P29ovd
d8WErY0gPxun8pbJLmxkAtWNhpMvfe0050vk9TL5wqbu9AlbssgTcCXkMQnPw9nC
YNN6DDP2lbcBrvgT9YCNL6C+ZKufD52yOQ9qOkwFTEQpjtF4uNtJom+asvlpmS8A
vLY9r60wYSvmZhNqBUrj7lyCtXMIu1kkd4w7F77k+DjHoAXyxcUp1DGL51sOmama
+TOWWgECgYEA8JtPxP0GRJ+IQkX262jM3dEIkza8ky5moIwUqYdsx0NxHgRRhORT
8c8hAuRBb2G82so8vUHk/fur85OEfc9TncnCY2crpoqsghifKLxrLgtT+qDpfZnx
SatLdt8GfQ85yA7hnWWJ2MxF3NaeSDm75Lsm+tBbAiyc9P2jGRNtMSkCgYEAypHd
HCctNi/FwjulhttFx/rHYKhLidZDFYeiE/v45bN4yFm8x7R/b0iE7KaszX+Exdvt
SghaTdcG0Knyw1bpJVyusavPzpaJMjdJ6tcFhVAbAjm7enCIvGCSx+X3l5SiWg0A
R57hJglezIiVjv3aGwHwvlZvtszK6zV6oXFAu0ECgYAbjo46T4hyP5tJi93V5HDi
Ttiek7xRVxUl+iU7rWkGAXFpMLFteQEsRr7PJ/lemmEY5eTDAFMLy9FL2m9oQWCg
R8VdwSk8r9FGLS+9aKcV5PI/WEKlwgXinB3OhYimtiG2Cg5JCqIZFHxD6MjEGOiu
L8ktHMPvodBwNsSBULpG0QKBgBAplTfC1HOnWiMGOU3KPwYWt0O6CdTkmJOmL8Ni
blh9elyZ9FsGxsgtRBXRsqXuz7wtsQAgLHxbdLq/ZJQ7YfzOKU4ZxEnabvXnvWkU
YOdjHdSOoKvDQNWu6ucyLRAWFuISeXw9a/9p7ftpxm0TSgyvmfLF2MIAEwyzRqaM
77pBAoGAMmjmIJdjp+Ez8duyn3ieo36yrttF5NSsJLAbxFpdlc1gvtGCWW+9Cq0b
dxviW8+TFVEBl1O4f7HVm6EpTscdDxU+bCXWkfjuRb7Dy9GOtt9JPsX8MBTakzh3
vBgsyi/sN3RqRBcGU40fOoZyfAMT8s1m/uYv52O6IgeuZ/ujbjY=
-----END RSA PRIVATE KEY-----
```
## Level17 -> level18
Save the RSA on bandit16 mission as `dodol` and `chmod 600 dodol` after that use it as private key on ssh

credential bandit18:x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO
```bash
┌──(kali㉿kali)-[/tmp]
└─$ ssh -i dodol bandit17@bandit.labs.overthewire.org -p 2220
bandit17@bandit:~$ ls -la 
total 36
drwxr-xr-x   3 root     root     4096 Apr  3 15:17 .
drwxr-xr-x 150 root     root     4096 Apr  3 15:20 ..
-rw-r-----   1 bandit17 bandit17   33 Apr  3 15:17 .bandit16.password
-rw-r--r--   1 root     root      220 Mar 31  2024 .bash_logout
-rw-r--r--   1 root     root     3851 Apr  3 15:10 .bashrc
-rw-r-----   1 bandit18 bandit17 3300 Apr  3 15:17 passwords.new
-rw-r-----   1 bandit18 bandit17 3300 Apr  3 15:17 passwords.old
-rw-r--r--   1 root     root      807 Mar 31  2024 .profile
drwxr-xr-x   2 root     root     4096 Apr  3 15:17 .ssh

bandit17@bandit:~$ diff passwords.old passwords.new 
42c42
< 390zFj2NETFVZkqYw8UEFdN6h40oGVtT
---
> x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO
```
## Level18 -> level19

credential bandit19:cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8
```bash
┌──(kali㉿kali)-[/tmp]
└─$ ssh  bandit18@bandit.labs.overthewire.org -p 2220 ls
                         _                     _ _ _   
                        | |__   __ _ _ __   __| (_) |_ 
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_ 
                        |_.__/ \__,_|_| |_|\__,_|_|\__|
                                                       

                      This is an OverTheWire game server. 
            More information on http://www.overthewire.org/wargames

backend: gibson-0
bandit18@bandit.labs.overthewire.org's password: 
readme
┌──(kali㉿kali)-[/tmp]
└─$ ssh  bandit18@bandit.labs.overthewire.org -p 2220 "cat readme"
                         _                     _ _ _   
                        | |__   __ _ _ __   __| (_) |_ 
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_ 
                        |_.__/ \__,_|_| |_|\__,_|_|\__|
                                                       

                      This is an OverTheWire game server. 
            More information on http://www.overthewire.org/wargames

backend: gibson-0
bandit18@bandit.labs.overthewire.org's password: 
cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8
```

## Level19 -> level20

Credential for bandit20:0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
```bash
┌──(kali㉿kali)-[/tmp]
└─$ ssh  bandit19@bandit.labs.overthewire.org -p 2220
bandit19@bandit:~$ ls -la 
total 36
drwxr-xr-x   2 root     root      4096 Apr  3 15:17 .
drwxr-xr-x 150 root     root      4096 Apr  3 15:20 ..
-rwsr-x---   1 bandit20 bandit19 14888 Apr  3 15:17 bandit20-do
-rw-r--r--   1 root     root       220 Mar 31  2024 .bash_logout
-rw-r--r--   1 root     root      3851 Apr  3 15:10 .bashrc
-rw-r--r--   1 root     root       807 Mar 31  2024 .profile
bandit19@bandit:~$ ./bandit20-do 
Run a command as another user.
  Example: ./bandit20-do whoami
bandit19@bandit:~$ ./bandit20-do cat /etc/bandit_pass/bandit20
0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
```

## Level20 -> level21

Credential for bandit21:EeoULMCra2q0dSkYj561DX7s1CpBuOBt
```bash
┌──(kali㉿kali)-[/tmp]
└─$ ssh  bandit20@bandit.labs.overthewire.org -p 2220
bandit20@bandit:~$ ls -la 
total 36
drwxr-xr-x   2 root     root      4096 Apr  3 15:17 .
drwxr-xr-x 150 root     root      4096 Apr  3 15:20 ..
-rw-r--r--   1 root     root       220 Mar 31  2024 .bash_logout
-rw-r--r--   1 root     root      3851 Apr  3 15:10 .bashrc
-rw-r--r--   1 root     root       807 Mar 31  2024 .profile
-rwsr-x---   1 bandit21 bandit20 15612 Apr  3 15:17 suconnect
```

Open 2 Terminal first listen on specific port and put the output on the file 
Terminal1:
```bash
bandit20@bandit:~$ touch /tmp/dodol
bandit20@bandit:~$ nc -lnvp 1234 > /tmp/dodol
Listening on 0.0.0.0 1234
Connection received on 127.0.0.1 48710
0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
bandit20@bandit:~$ cat /tmp/dodol
EeoULMCra2q0dSkYj561DX7s1CpBuOBt
```
Terminal2:
```bash
bandit20@bandit:~$ ./suconnect 1234
0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
Read: 0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
Password matches, sending next password
```

## Level21 -> level22
Look in /etc/cron.d/ for the configuration and see what command is being executed.
```bash
┌──(kali㉿kali)-[/tmp]
└─$ ssh  bandit21@bandit.labs.overthewire.org -p 2220
bandit21@bandit:~$ ls -la /etc/cron.d/
total 60
drwxr-xr-x   2 root root  4096 Apr  3 15:21 .
drwxr-xr-x 128 root root 12288 Apr  5 12:34 ..
-r--r-----   1 root root    47 Apr  3 15:18 behemoth4_cleanup
-rw-r--r--   1 root root   123 Apr  3 15:10 clean_tmp
-rw-r--r--   1 root root   120 Apr  3 15:17 cronjob_bandit22
-rw-r--r--   1 root root   122 Apr  3 15:17 cronjob_bandit23
-rw-r--r--   1 root root   120 Apr  3 15:17 cronjob_bandit24
-rw-r--r--   1 root root   201 Apr  8  2024 e2scrub_all
-r--r-----   1 root root    48 Apr  3 15:19 leviathan5_cleanup
-rw-------   1 root root   138 Apr  3 15:19 manpage3_resetpw_job
-rwx------   1 root root    52 Apr  3 15:21 otw-tmp-dir
-rw-r--r--   1 root root   102 Mar 31  2024 .placeholder
-rw-r--r--   1 root root   396 Jan  9  2024 sysstat
bandit21@bandit:~$ cat /etc/cron.d/cronjob_bandit22
@reboot bandit22 /usr/bin/cronjob_bandit22.sh &> /dev/null
* * * * * bandit22 /usr/bin/cronjob_bandit22.sh &> /dev/null
bandit21@bandit:~$ cat /usr/bin/cronjob_bandit22.sh
#!/bin/bash
chmod 644 /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
cat /etc/bandit_pass/bandit22 > /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
bandit21@bandit:~$ cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
tRae0UfB9v0UzbCdn9cY0gQnds9GF58Q
```

## Level22 -> level23
```bash
bandit22@bandit:~$ cat /etc/cron.d/cronjob_bandit23
@reboot bandit23 /usr/bin/cronjob_bandit23.sh  &> /dev/null
* * * * * bandit23 /usr/bin/cronjob_bandit23.sh  &> /dev/null
bandit22@bandit:~$ cat /usr/bin/cronjob_bandit23.sh
#!/bin/bash
myname=$(whoami)
mytarget=$(echo I am user $myname | md5sum | cut -d ' ' -f 1)
echo "Copying passwordfile /etc/bandit_pass/$myname to /tmp/$mytarget"
cat /etc/bandit_pass/$myname > /tmp/$mytarget
```
Solve:
```bash
bandit22@bandit:~$ mytarget=$(echo I am user bandit23 | md5sum | cut -d ' ' -f 1)
bandit22@bandit:~$ echo $mytarget
8ca319486bfbbc3663ea0fbe81326349
bandit22@bandit:~$ cat /tmp/$mytarget
0Zf11ioIjMVN551jX3CmStKLYqjk54Ga
```
## Level23 -> level24
```bash
┌──(kali㉿kali)-[/tmp]
└─$ ssh  bandit23@bandit.labs.overthewire.org -p 2220
bandit23@bandit:~$ cat /etc/cron.d/cronjob_bandit24
@reboot bandit24 /usr/bin/cronjob_bandit24.sh &> /dev/null
* * * * * bandit24 /usr/bin/cronjob_bandit24.sh &> /dev/null
bandit23@bandit:~$ cat /usr/bin/cronjob_bandit24.sh
#!/bin/bash

shopt -s nullglob

myname=$(whoami)

cd /var/spool/"$myname"/foo || exit 
echo "Executing and deleting all scripts in /var/spool/$myname/foo:"
for i in * .*;
do
    if [ "$i" != "." ] && [ "$i" != ".." ];
    then
        echo "Handling $i"
        owner="$(stat --format "%U" "./$i")"
        if [ "${owner}" = "bandit23" ] && [ -f "$i" ]; then
            timeout -s 9 60 "./$i"
        fi
        rm -rf "./$i"
    fi
done
```
Solve : create an executable script using bash that cat `/etc/bandit_pass/bandit24 > /tmp/goreng/passwd` and file text 
```bash
bandit23@bandit:/tmp/goreng$ ls -la 
total 796
drwxrwxr-x    2 bandit23 bandit23   4096 May  5 08:32 .
drwxrwx-wt 1359 root     root     802816 May  5 08:33 ..
-rwxrwxr-x    1 bandit23 bandit23     64 May  5 08:32 doreng.sh
-rwxrwxrwx    1 bandit23 bandit23      0 May  5 08:32 passwd

bandit23@bandit:/tmp/goreng$ cat passwd
gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8
```

## Level24 -> level25
```bash
┌──(kali㉿kali)-[/tmp]
└─$ ssh bandit24@bandit.labs.overthewire.org -p 2220
bandit24@bandit:/tmp/goreng$ for i in $(seq -f "%04g" 0 9999); do echo 'gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8 '$i >> /tmp/goreng/pin.txt; done
cat pin.txt | nc localhost 30002 >> hasil.txt
bandit24@bandit:/tmp/goreng$ cat hasil.txt  | grep -v 'Wrong'
I am the pincode checker for user bandit25. Please enter the password for user bandit24 and the secret pincode on a single line, separated by a space.
Correct!
The password of user bandit25 is iCi86ttT4KSNe1armKiwbQNmB3YJP3q4
```
## Level25 -> level26
```bash
┌──(kali㉿kali)-[/tmp]
└─$ ssh  bandit25@bandit.labs.overthewire.org -p 2220
bandit25@bandit:~$ ls -la 
total 40
drwxr-xr-x   2 root     root     4096 Apr  3 15:17 .
drwxr-xr-x 150 root     root     4096 Apr  3 15:20 ..
-rw-r-----   1 bandit25 bandit25   33 Apr  3 15:17 .bandit24.password
-r--------   1 bandit25 bandit25 1679 Apr  3 15:17 bandit26.sshkey
-rw-r-----   1 bandit25 bandit25  151 Apr  3 15:17 .banner
-rw-r--r--   1 root     root      220 Mar 31  2024 .bash_logout
-rw-r--r--   1 root     root     3851 Apr  3 15:10 .bashrc
-rw-r-----   1 bandit25 bandit25   66 Apr  3 15:17 .flag
-rw-r-----   1 bandit25 bandit25    4 Apr  3 15:17 .pin
-rw-r--r--   1 root     root      807 Mar 31  2024 .profile
bandit25@bandit:~$ cat bandit26.sshkey
-----BEGIN RSA PRIVATE KEY-----
MIIEpQIBAAKCAQEApis2AuoooEqeYWamtwX2k5z9uU1Afl2F8VyXQqbv/LTrIwdW
pTfaeRHXzr0Y0a5Oe3GB/+W2+PReif+bPZlzTY1XFwpk+DiHk1kmL0moEW8HJuT9
/5XbnpjSzn0eEAfFax2OcopjrzVqdBJQerkj0puv3UXY07AskgkyD5XepwGAlJOG
xZsMq1oZqQ0W29aBtfykuGie2bxroRjuAPrYM4o3MMmtlNE5fC4G9Ihq0eq73MDi
1ze6d2jIGce873qxn308BA2qhRPJNEbnPev5gI+5tU+UxebW8KLbk0EhoXB953Ix
3lgOIrT9Y6skRjsMSFmC6WN/O7ovu8QzGqxdywIDAQABAoIBAAaXoETtVT9GtpHW
qLaKHgYtLEO1tOFOhInWyolyZgL4inuRRva3CIvVEWK6TcnDyIlNL4MfcerehwGi
il4fQFvLR7E6UFcopvhJiSJHIcvPQ9FfNFR3dYcNOQ/IFvE73bEqMwSISPwiel6w
e1DjF3C7jHaS1s9PJfWFN982aublL/yLbJP+ou3ifdljS7QzjWZA8NRiMwmBGPIh
Yq8weR3jIVQl3ndEYxO7Cr/wXXebZwlP6CPZb67rBy0jg+366mxQbDZIwZYEaUME
zY5izFclr/kKj4s7NTRkC76Yx+rTNP5+BX+JT+rgz5aoQq8ghMw43NYwxjXym/MX
c8X8g0ECgYEA1crBUAR1gSkM+5mGjjoFLJKrFP+IhUHFh25qGI4Dcxxh1f3M53le
wF1rkp5SJnHRFm9IW3gM1JoF0PQxI5aXHRGHphwPeKnsQ/xQBRWCeYpqTme9amJV
tD3aDHkpIhYxkNxqol5gDCAt6tdFSxqPaNfdfsfaAOXiKGrQESUjIBcCgYEAxvmI
2ROJsBXaiM4Iyg9hUpjZIn8TW2UlH76pojFG6/KBd1NcnW3fu0ZUU790wAu7QbbU
i7pieeqCqSYcZsmkhnOvbdx54A6NNCR2btc+si6pDOe1jdsGdXISDRHFb9QxjZCj
6xzWMNvb5n1yUb9w9nfN1PZzATfUsOV+Fy8CbG0CgYEAifkTLwfhqZyLk2huTSWm
pzB0ltWfDpj22MNqVzR3h3d+sHLeJVjPzIe9396rF8KGdNsWsGlWpnJMZKDjgZsz
JQBmMc6UMYRARVP1dIKANN4eY0FSHfEebHcqXLho0mXOUTXe37DWfZza5V9Oify3
JquBd8uUptW1Ue41H4t/ErsCgYEArc5FYtF1QXIlfcDz3oUGz16itUZpgzlb71nd
1cbTm8EupCwWR5I1j+IEQU+JTUQyI1nwWcnKwZI+5kBbKNJUu/mLsRyY/UXYxEZh
ibrNklm94373kV1US/0DlZUDcQba7jz9Yp/C3dT/RlwoIw5mP3UxQCizFspNKOSe
euPeaxUCgYEAntklXwBbokgdDup/u/3ms5Lb/bm22zDOCg2HrlWQCqKEkWkAO6R5
/Wwyqhp/wTl8VXjxWo+W+DmewGdPHGQQ5fFdqgpuQpGUq24YZS8m66v5ANBwd76t
IZdtF5HXs2S5CADTwniUS5mX1HO9l5gUkk+h0cH5JnPtsMCnAUM+BRY=
-----END RSA PRIVATE KEY-----
```

## Level26 -> level27
```bash
bandit25@bandit:~$ cat /etc/passwd | grep bandit26
bandit26:x:11026:11026:bandit level 26:/home/bandit26:/usr/bin/showtext
bandit25@bandit:~$ file /usr/bin/showtext
/usr/bin/showtext: POSIX shell script, ASCII text executable
bandit25@bandit:~$ cat /usr/bin/showtext
#!/bin/sh

export TERM=linux

exec more ~/text.txt
exit 0
```
Setup the terminal set history to the 2 and minimize the width of the terminal so more is showed
after that press `v` to change to vim mode, on vim type `:!/bin/bash` 
```bash
bandit26@bandit:~$ ls -la 
total 44
drwxr-xr-x   3 root     root      4096 Apr  3 15:17 .
drwxr-xr-x 150 root     root      4096 Apr  3 15:20 ..
-rwsr-x---   1 bandit27 bandit26 14888 Apr  3 15:17 bandit27-do
-rw-r--r--   1 root     root       220 Mar 31  2024 .bash_logout
-rw-r--r--   1 root     root      3851 Apr  3 15:10 .bashrc
-rw-r--r--   1 root     root       807 Mar 31  2024 .profile
drwxr-xr-x   2 root     root      4096 Apr  3 15:17 .ssh
-rw-r-----   1 bandit26 bandit26   258 Apr  3 15:17 text.txt
bandit26@bandit:~$ ./bandit27-do
Run a command as another user.
  Example: ./bandit27-do id
bandit26@bandit:~$ ./bandit27-do cat /etc/bandit_pass/bandit27
upsNCc7vzaRDx6oZC6GiR6ERwe1MowGB
```
## Level27 -> level28

git ssh://bandit27-git@bandit.labs.overthewire.org/home/bandit27-git/repo
```bash
┌──(kali㉿kali)-[/tmp]
└─$ git clone ssh://bandit27-git@bandit.labs.overthewire.org:2220/home/bandit27-git/repo
Cloning into 'repo'...
                         _                     _ _ _   
                        | |__   __ _ _ __   __| (_) |_ 
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_ 
                        |_.__/ \__,_|_| |_|\__,_|_|\__|
                                                       

                      This is an OverTheWire game server. 
            More information on http://www.overthewire.org/wargames

backend: gibson-0
bandit27-git@bandit.labs.overthewire.org's password: 
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.

┌──(kali㉿kali)-[/tmp]
└─$ ls -la repo 
total 4
drwxrwxr-x  3 kali kali  80 May  5 16:34 .
drwxrwxrwt 18 root root 480 May  5 16:33 ..
drwxrwxr-x  7 kali kali 240 May  5 16:34 .git
-rw-rw-r--  1 kali kali  68 May  5 16:34 README

┌──(kali㉿kali)-[/tmp]
└─$ cd repo 
┌──(kali㉿kali)-[/tmp/repo]
└─$ cat README 
The password to the next level is: Yz9IpL0sBcCeuG7m9uQFt8ZNpS4HZRcN
```
## Level28 -> level29
```bash
┌──(kali㉿kali)-[/tmp]
└─$ git clone ssh://bandit28-git@bandit.labs.overthewire.org:2220/home/bandit28-git/repo
Cloning into 'repo'...
                         _                     _ _ _   
                        | |__   __ _ _ __   __| (_) |_ 
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_ 
                        |_.__/ \__,_|_| |_|\__,_|_|\__|
                                                       

                      This is an OverTheWire game server. 
            More information on http://www.overthewire.org/wargames

backend: gibson-0
bandit28-git@bandit.labs.overthewire.org's password: 
remote: Enumerating objects: 9, done.
remote: Counting objects: 100% (9/9), done.
remote: Compressing objects: 100% (6/6), done.
Receiving objects: 100% (9/9), 799 bytes | 88.00 KiB/s, done.
Resolving deltas: 100% (2/2), done.
remote: Total 9 (delta 2), reused 0 (delta 0), pack-reused 0
                                                                                                                                                                            
┌──(kali㉿kali)-[/tmp]
└─$ cd repo 
                                                                                                                                                                            
┌──(kali㉿kali)-[/tmp/repo]
└─$ ls -la 
total 4
drwxrwxr-x  3 kali kali  80 May  5 16:37 .
drwxrwxrwt 18 root root 480 May  5 16:37 ..
drwxrwxr-x  7 kali kali 240 May  5 16:37 .git
-rw-rw-r--  1 kali kali 111 May  5 16:37 README.md
                                                                                                                                                                            
┌──(kali㉿kali)-[/tmp/repo]
└─$ cat README.md 
# Bandit Notes
Some notes for level29 of bandit.

## credentials

- username: bandit29
- password: xxxxxxxxxx

                                                                                                                                                                            
┌──(kali㉿kali)-[/tmp/repo]
└─$ git log 
commit adc7f885a129baee883058b8a870739489f80194 (HEAD -> master, origin/master, origin/HEAD)
Author: Morla Porla <morla@overthewire.org>
Date:   Fri Apr 3 15:17:54 2026 +0000

    fix info leak

commit a3437bddd447f2d496731658e86b98cbea9d3c98
Author: Morla Porla <morla@overthewire.org>
Date:   Fri Apr 3 15:17:54 2026 +0000

    add missing data

commit cb630ec182b75bc289595511f8bcf4d47cfec50d
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Apr 3 15:17:54 2026 +0000

    initial commit of README.md
                                                                                                                                                                            
┌──(kali㉿kali)-[/tmp/repo]
└─$ git show adc7f885a129baee883058b8a870739489f80194
commit adc7f885a129baee883058b8a870739489f80194 (HEAD -> master, origin/master, origin/HEAD)
Author: Morla Porla <morla@overthewire.org>
Date:   Fri Apr 3 15:17:54 2026 +0000

    fix info leak

diff --git a/README.md b/README.md
index d4e3b74..5c6457b 100644
--- a/README.md
+++ b/README.md
@@ -4,5 +4,5 @@ Some notes for level29 of bandit.
 ## credentials
 
 - username: bandit29
-- password: 4pT1t5DENaYuqnqvadYs1oE4QLCdjmJ7
+- password: xxxxxxxxxx
```

## Level29 -> level30
```bash
┌──(kali㉿kali)-[/tmp]
└─$ git clone ssh://bandit29-git@bandit.labs.overthewire.org:2220/home/bandit29-git/repo
Cloning into 'repo'...
                         _                     _ _ _   
                        | |__   __ _ _ __   __| (_) |_ 
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_ 
                        |_.__/ \__,_|_| |_|\__,_|_|\__|
                                                       

                      This is an OverTheWire game server. 
            More information on http://www.overthewire.org/wargames

backend: gibson-0
bandit29-git@bandit.labs.overthewire.org's password: 
remote: Enumerating objects: 16, done.
remote: Counting objects: 100% (16/16), done.
remote: Compressing objects: 100% (11/11), done.
remote: Total 16 (delta 2), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (16/16), done.
Resolving deltas: 100% (2/2), done.
                                                                                                                                                                            
┌──(kali㉿kali)-[/tmp]
└─$ cd repo 
                                                                                                                                                                            
┌──(kali㉿kali)-[/tmp/repo]
└─$ ls -la
total 4
drwxrwxr-x  3 kali kali  80 May  5 16:41 .
drwxrwxrwt 18 root root 480 May  5 16:41 ..
drwxrwxr-x  7 kali kali 240 May  5 16:41 .git
-rw-rw-r--  1 kali kali 131 May  5 16:41 README.md
                                                                                                                                                                            
┌──(kali㉿kali)-[/tmp/repo]
└─$ cat README.md 
# Bandit Notes
Some notes for bandit30 of bandit.

## credentials

- username: bandit30
- password: <no passwords in production!>

┌──(kali㉿kali)-[/tmp/repo]
└─$ git branch 
* master
                                                                                                                                                                            
┌──(kali㉿kali)-[/tmp/repo]
└─$ git branch -a
* master
  remotes/origin/HEAD -> origin/master
  remotes/origin/dev
  remotes/origin/master
  remotes/origin/sploits-dev

┌──(kali㉿kali)-[/tmp/repo]
└─$ git checkout dev
branch 'dev' set up to track 'origin/dev'.
Switched to a new branch 'dev'
                     
┌──(kali㉿kali)-[/tmp/repo]
└─$ cat README.md 
# Bandit Notes
Some notes for bandit30 of bandit.

## credentials

- username: bandit30
- password: qp30ex3VLz5MDG1n91YowTv4Q8l7CDZL
```

## Level30 -> level31
```bash
┌──(kali㉿kali)-[/tmp]
└─$ git clone ssh://bandit30-git@bandit.labs.overthewire.org:2220/home/bandit30-git/repo
Cloning into 'repo'...
                         _                     _ _ _   
                        | |__   __ _ _ __   __| (_) |_ 
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_ 
                        |_.__/ \__,_|_| |_|\__,_|_|\__|
                                                       

                      This is an OverTheWire game server. 
            More information on http://www.overthewire.org/wargames

backend: gibson-0
bandit30-git@bandit.labs.overthewire.org's password: 
remote: Enumerating objects: 16, done.
remote: Counting objects: 100% (16/16), done.
remote: Compressing objects: 100% (11/11), done.
remote: Total 16 (delta 2), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (16/16), done.
Resolving deltas: 100% (2/2), done.

┌──(kali㉿kali)-[/tmp/repo]
└─$ git tag
secret
┌──(kali㉿kali)-[/tmp/repo]
└─$ git show secret
fb5S2xb7bRyFmAvQYQGEqsbhVyJqhnDy
```
## Level31 -> level32
```bash
┌──(kali㉿kali)-[/tmp]
└─$ git clone ssh://bandit31-git@bandit.labs.overthewire.org:2220/home/bandit31-git/repo
Cloning into 'repo'...
                         _                     _ _ _   
                        | |__   __ _ _ __   __| (_) |_ 
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_ 
                        |_.__/ \__,_|_| |_|\__,_|_|\__|
                                                       

                      This is an OverTheWire game server. 
            More information on http://www.overthewire.org/wargames

backend: gibson-0
bandit31-git@bandit.labs.overthewire.org's password: 
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (4/4), done.
                            
┌──(kali㉿kali)-[/tmp]
└─$ cd repo 
                            
┌──(kali㉿kali)-[/tmp/repo]
└─$ ls -la
total 8
drwxrwxr-x  3 kali kali 100 May  5 16:59 .
drwxrwxrwt 18 root root 480 May  5 16:58 ..
drwxrwxr-x  7 kali kali 240 May  5 16:59 .git
-rw-rw-r--  1 kali kali   6 May  5 16:59 .gitignore
-rw-rw-r--  1 kali kali 147 May  5 16:59 README.md
                            
┌──(kali㉿kali)-[/tmp/repo]
└─$ cat README.md 
This time your task is to push a file to the remote repository.

Details:
    File name: key.txt
    Content: 'May I come in?'
    Branch: master

┌──(kali㉿kali)-[/tmp/repo]
└─$ cat .gitignore 
*.txt

┌──(kali㉿kali)-[/tmp/repo]
└─$ echo 'May I come in?' > key.txt
                                                                                                                                                                            
┌──(kali㉿kali)-[/tmp/repo]
└─$ git add .                      
                                                                                                                                                                            
┌──(kali㉿kali)-[/tmp/repo]
└─$ git commit -m "Adding key.txt"
[master bb46203] Adding key.txt
 1 file changed, 1 insertion(+)
 create mode 100644 key.txt
                                                                                                                                                                            
┌──(kali㉿kali)-[/tmp/repo]
└─$ git push 
                         _                     _ _ _   
                        | |__   __ _ _ __   __| (_) |_ 
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_ 
                        |_.__/ \__,_|_| |_|\__,_|_|\__|
                                                       

                      This is an OverTheWire game server. 
            More information on http://www.overthewire.org/wargames

backend: gibson-0
bandit31-git@bandit.labs.overthewire.org's password: 
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (6/6), 516 bytes | 516.00 KiB/s, done.
Total 6 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: ### Attempting to validate files... ####
remote: 
remote: .oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.
remote: 
remote: Well done! Here is the password for the next level:
remote: 3O9RfhqyAlVBEZpVb6LYStshZoqoSx5K 
remote: 
remote: .oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.
remote: 
To ssh://bandit.labs.overthewire.org:2220/home/bandit31-git/repo
 ! [remote rejected] master -> master (pre-receive hook declined)
error: failed to push some refs to 'ssh://bandit.labs.overthewire.org:2220/home/bandit31-git/repo'
```
## Level32 -> level33
```bash
┌──(kali㉿kali)-[/tmp]
└─$ ssh bandit32@bandit.labs.overthewire.org -p 2220                            
                         _                     _ _ _   
                        | |__   __ _ _ __   __| (_) |_ 
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_ 
                        |_.__/ \__,_|_| |_|\__,_|_|\__|
                                                       

                      This is an OverTheWire game server. 
            More information on http://www.overthewire.org/wargames

backend: gibson-0
bandit32@bandit.labs.overthewire.org's password: 

      ,----..            ,----,          .---.
     /   /   \         ,/   .`|         /. ./|
    /   .     :      ,`   .'  :     .--'.  ' ;
   .   /   ;.  \   ;    ;     /    /__./ \ : |
  .   ;   /  ` ; .'___,/    ,' .--'.  '   \' .
  ;   |  ; \ ; | |    :     | /___/ \ |    ' '
  |   :  | ; | ' ;    |.';  ; ;   \  \;      :
  .   |  ' ' ' : `----'  |  |  \   ;  `      |
  '   ;  \; /  |     '   :  ;   .   \    .\  ;
   \   \  ',  /      |   |  '    \   \   ' \ |
    ;   :    /       '   :  |     :   '  |--"
     \   \ .'        ;   |.'       \   \ ;
  www. `---` ver     '---' he       '---" ire.org


Welcome to OverTheWire!

If you find any problems, please report them to the #wargames channel on
discord or IRC.

--[ Playing the games ]--

  This machine might hold several wargames.
  If you are playing "somegame", then:

    * USERNAMES are somegame0, somegame1, ...
    * Most LEVELS are stored in /somegame/.
    * PASSWORDS for each level are stored in /etc/somegame_pass/.

  Write-access to homedirectories is disabled. It is advised to create a
  working directory with a hard-to-guess name in /tmp/.  You can use the
  command "mktemp -d" in order to generate a random and hard to guess
  directory in /tmp/.  Read-access to both /tmp/ is disabled and to /proc
  restricted so that users cannot snoop on eachother. Files and directories
  with easily guessable or short names will be periodically deleted! The /tmp
  directory is regularly wiped.
  Please play nice:

    * don't leave orphan processes running
    * don't leave exploit-files laying around
    * don't annoy other players
    * don't post passwords or spoilers
    * again, DONT POST SPOILERS!
      This includes writeups of your solution on your blog or website!

--[ Tips ]--

  This machine has a 64bit processor and many security-features enabled
  by default, although ASLR has been switched off.  The following
  compiler flags might be interesting:

    -m32                    compile for 32bit
    -fno-stack-protector    disable ProPolice
    -Wl,-z,norelro          disable relro

  In addition, the execstack tool can be used to flag the stack as
  executable on ELF binaries.

  Finally, network-access is limited for most levels by a local
  firewall.

--[ Tools ]--

 For your convenience we have installed a few useful tools which you can find
 in the following locations:

    * gef (https://github.com/hugsy/gef) in /opt/gef/
    * pwndbg (https://github.com/pwndbg/pwndbg) in /opt/pwndbg/
    * gdbinit (https://github.com/gdbinit/Gdbinit) in /opt/gdbinit/
    * pwntools (https://github.com/Gallopsled/pwntools)
    * radare2 (http://www.radare.org/)

--[ More information ]--

  For more information regarding individual wargames, visit
  http://www.overthewire.org/wargames/

  For support, questions or comments, contact us on discord or IRC.

  Enjoy your stay!

WELCOME TO THE UPPERCASE SHELL
sh: 1: 7: Permission denied
>> $0
$ ls -la 
total 36
drwxr-xr-x   2 root     root      4096 Apr  3 15:18 .
drwxr-xr-x 150 root     root      4096 Apr  3 15:20 ..
-rw-r--r--   1 root     root       220 Mar 31  2024 .bash_logout
-rw-r--r--   1 root     root      3851 Apr  3 15:10 .bashrc
-rw-r--r--   1 root     root       807 Mar 31  2024 .profile
-rwsr-x---   1 bandit33 bandit32 15144 Apr  3 15:18 uppershell
$ id
uid=11033(bandit33) gid=11032(bandit32) groups=11032(bandit32)
$ cat /etc/bandit_pass/bandit33
tQdtbs5D5i2vJwkO8mEyYEyTL8izoeJ0
```
## Level33 -> level34
```bash
┌──(kali㉿kali)-[/tmp]
└─$ ssh bandit33@bandit.labs.overthewire.org -p 2220
                         _                     _ _ _   
                        | |__   __ _ _ __   __| (_) |_ 
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_ 
                        |_.__/ \__,_|_| |_|\__,_|_|\__|
                                                       

                      This is an OverTheWire game server. 
            More information on http://www.overthewire.org/wargames

backend: gibson-0
bandit33@bandit.labs.overthewire.org's password: 

      ,----..            ,----,          .---.
     /   /   \         ,/   .`|         /. ./|
    /   .     :      ,`   .'  :     .--'.  ' ;
   .   /   ;.  \   ;    ;     /    /__./ \ : |
  .   ;   /  ` ; .'___,/    ,' .--'.  '   \' .
  ;   |  ; \ ; | |    :     | /___/ \ |    ' '
  |   :  | ; | ' ;    |.';  ; ;   \  \;      :
  .   |  ' ' ' : `----'  |  |  \   ;  `      |
  '   ;  \; /  |     '   :  ;   .   \    .\  ;
   \   \  ',  /      |   |  '    \   \   ' \ |
    ;   :    /       '   :  |     :   '  |--"
     \   \ .'        ;   |.'       \   \ ;
  www. `---` ver     '---' he       '---" ire.org


Welcome to OverTheWire!

If you find any problems, please report them to the #wargames channel on
discord or IRC.

--[ Playing the games ]--

  This machine might hold several wargames.
  If you are playing "somegame", then:

    * USERNAMES are somegame0, somegame1, ...
    * Most LEVELS are stored in /somegame/.
    * PASSWORDS for each level are stored in /etc/somegame_pass/.

  Write-access to homedirectories is disabled. It is advised to create a
  working directory with a hard-to-guess name in /tmp/.  You can use the
  command "mktemp -d" in order to generate a random and hard to guess
  directory in /tmp/.  Read-access to both /tmp/ is disabled and to /proc
  restricted so that users cannot snoop on eachother. Files and directories
  with easily guessable or short names will be periodically deleted! The /tmp
  directory is regularly wiped.
  Please play nice:

    * don't leave orphan processes running
    * don't leave exploit-files laying around
    * don't annoy other players
    * don't post passwords or spoilers
    * again, DONT POST SPOILERS!
      This includes writeups of your solution on your blog or website!

--[ Tips ]--

  This machine has a 64bit processor and many security-features enabled
  by default, although ASLR has been switched off.  The following
  compiler flags might be interesting:

    -m32                    compile for 32bit
    -fno-stack-protector    disable ProPolice
    -Wl,-z,norelro          disable relro

  In addition, the execstack tool can be used to flag the stack as
  executable on ELF binaries.

  Finally, network-access is limited for most levels by a local
  firewall.

--[ Tools ]--

 For your convenience we have installed a few useful tools which you can find
 in the following locations:

    * gef (https://github.com/hugsy/gef) in /opt/gef/
    * pwndbg (https://github.com/pwndbg/pwndbg) in /opt/pwndbg/
    * gdbinit (https://github.com/gdbinit/Gdbinit) in /opt/gdbinit/
    * pwntools (https://github.com/Gallopsled/pwntools)
    * radare2 (http://www.radare.org/)

--[ More information ]--

  For more information regarding individual wargames, visit
  http://www.overthewire.org/wargames/

  For support, questions or comments, contact us on discord or IRC.

  Enjoy your stay!

bandit33@bandit:~$ ls -la 
total 24
drwxr-xr-x   2 root     root     4096 Apr  3 15:18 .
drwxr-xr-x 150 root     root     4096 Apr  3 15:20 ..
-rw-r--r--   1 root     root      220 Mar 31  2024 .bash_logout
-rw-r--r--   1 root     root     3851 Apr  3 15:10 .bashrc
-rw-r--r--   1 root     root      807 Mar 31  2024 .profile
-rw-------   1 bandit33 bandit33  430 Apr  3 15:18 README.txt
bandit33@bandit:~$ cat README.txt 
Congratulations on solving the last level of this game!

At this moment, there are no more levels to play in this game. However, we are constantly working
on new levels and will most likely expand this game with more levels soon.
Keep an eye out for an announcement on our usual communication channels!
In the meantime, you could play some of our other wargames.

If you have an idea for an awesome new level, please let us know!
```
