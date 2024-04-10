Tool Documentation:
hydra Usage Example

Attempt to login as the root user (-l root) using a password list (-P /usr/share/wordlists/metasploit/unix_passwords.txt) with 6 threads (-t 6) on the given SSH server (ssh://192.168.1.123):

root@kali:~# hydra -l root -P /usr/share/wordlists/metasploit/unix_passwords.txt -t 6 ssh://192.168.1.123
Hydra v7.6 (c)2013 by van Hauser/THC & David Maciejak - for legal purposes only

Hydra (http://www.thc.org/thc-hydra) starting at 2014-05-19 07:53:33
[DATA] 6 tasks, 1 server, 1003 login tries (l:1/p:1003), ~167 tries per task
[DATA] attacking service ssh on port 22


pw-inspector Usage Example

Read in a list of passwords (-i /usr/share/wordlists/nmap.lst) and save to a file (-o /root/passes.txt), selecting passwords of a minimum length of 6 (-m 6) and a maximum length of 10 (-M 10):