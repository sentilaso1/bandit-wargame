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
+ cat data.txt | grep "millionth"
+ ssh bandit8@bandit.labs.overthewire.org -p 2220 pass: dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc

level 9:
+ sort data.txt | uniq -u
+ ssh bandit9@bandit.labs.overthewire.org -p 2220 pass: 4CKMh1JI91bUIZZPXDqGanal4xvAg0JM

level 10: 
+ strings data.txt | grep -E '=+'
+ ssh bandit10@bandit.labs.overthewire.org -p 2220 pass: FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey

level 11:
+ cat data.txt | base64 -d
+ ssh bandit11@bandit.labs.overthewire.org -p 2220 pass: dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr

level 12:
+ cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
+ ssh bandit12@bandit.labs.overthewire.org -p 2220 pass: 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4

level 13:
+ workdir=$(mktemp -d) | cd "$workdir"
+ cp ~/data.txt . | mv data.txt data.hex | xxd -r data.hex data.bin
+ loop command: file data ->
- gzip: mv data.bin data.gz | gunzip data.gz
- bzip2: mv data.bin data.bz2 | bunzip2 data.bz2
- tar: tar -xf data.bin
+ ssh bandit13@bandit.labs.overthewire.org -p 2220 pass: FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn

level 14:
+ clone sshkey.private
+ chmod 600 sshkey.private
+ ssh bandit14@bandit.labs.overthewire.org -p 2220 -i sshkey.private
+ ssh bandit14@bandit.labs.overthewire.org -p 2220 pass: MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS

level 15: 
+ nc localhost 30000 < /etc/bandit_pass/bandit14
+ ssh bandit15@bandit.labs.overthewire.org -p 2220 pass: 8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo

level 16:
+ printf "%s\n" "$(cat /etc/bandit_pass/bandit15)" | openssl s_client -connect localhost:30001 -quiet
+ ssh bandit16@bandit.labs.overthewire.org -p 2220 pass: kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx
