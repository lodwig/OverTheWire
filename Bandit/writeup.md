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
