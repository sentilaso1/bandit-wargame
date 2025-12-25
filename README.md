# bandit-wargame
level 0: 
+ ssh bandit0@bandit.labs.overthewire.org -p 2220 pass: bandit0

level 1: 
+ cat readme
+ ssh bandit1@bandit.labs.overthewire.org -p 2220 pass: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If

level 2: 
+ cat ./-
+ ssh bandit2@bandit.labs.overthewire.org -p 2220 pass: 263JGJPfgU6LtdEvgfWU1XP5yac29mFx
  
level 3: 
+ cat ./'--spaces in this filename--'
+ ssh bandit3@bandit.labs.overthewire.org -p 2220 pass: MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
  
level 4: 
+ cat inhere/...Hiding-From-You
+ ssh bandit4@bandit.labs.overthewire.org -p 2220 pass: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
  
level 5: 
+ cat inhere/-file07
+ ssh bandit5@bandit.labs.overthewire.org -p 2220 pass: 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
  
level 6: 
+ find inhere/ -type f -size 1033c ! -executable
+ cat inhere/maybehere07/.file2
+ ssh bandit6@bandit.labs.overthewire.org -p 2220 pass: HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
  
level 7: 
+ find / -type f -size 33c -user bandit7 -group bandit6 2>/dev/null
+ cat /var/lib/dpkg/info/bandit7.password
+ ssh bandit7@bandit.labs.overthewire.org -p 2220 pass: morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
  
level 8: 
