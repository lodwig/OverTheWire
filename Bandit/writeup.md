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













