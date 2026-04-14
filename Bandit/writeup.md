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
