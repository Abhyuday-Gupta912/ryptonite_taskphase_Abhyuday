# PONDERING PATH

## THE PATH VARIABLE
### FLAG: pwn.college{wf_AY-RbapINtceXIPG-JspQf3W.dZzNwUDLycTN0czW}
### APPROACH USED: 
````
hacker@path~the-path-variable:~$ PATH=""
hacker@path~the-path-variable:~$ /challenge/run
Trying to remove /flag...
/challenge/run: line 4: rm: No such file or directory
The flag is still there! I might as well give it to you!
pwn.college{wf_AY-RbapINtceXIPG-JspQf3W.dZzNwUDLycTN0czW}
````

## Setting PATH
### FLAG:pwn.college{I0pM6F8ryES_vQWuUl0aG-JejcU.dVzNyUDLycTN0czW}
### APPROACH USED:
````
hacker@path~setting-path:~$ PATH=/challenge/more_commands
hacker@path~setting-path:~$ /challenge/run
Invoking 'win'....
Congratulations! You properly set the flag and 'win' has launched!
pwn.college{I0pM6F8ryES_vQWuUl0aG-JejcU.dVzNyUDLycTN0czW}
````

## ADDING COMMANDS
### FLAG: pwn.college{kC70CEhLXasaElPxwNWrkEHG0ij.dZzNyUDLycTN0czW}
### APPROACH USED:
````
hacker@path~adding-commands:~$ touch win
hacker@path~adding-commands:~$ nano win
hacker@path~adding-commands:~$ cat win
cat /flag
hacker@path~adding-commands:~$ echo $PATH
/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
hacker@path~adding-commands:~$
hacker@path~adding-commands:~$ PATH=~:$PATH
hacker@path~adding-commands:~$ chmod ugo+rwx win
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
pwn.college{kC70CEhLXasaElPxwNWrkEHG0ij.dZzNyUDLycTN0czW}
````

## HIJACKING COMMANDS
### FLAG: pwn.college{QhqYNyNF3ViRnijR-hW3JzDtu6v.ddzNyUDLycTN0czW}
### APPROACH USED:
````
hacker@path~hijacking-commands:~$ touch rm
hacker@path~hijacking-commands:~$ nano rm
hacker@path~hijacking-commands:~$ PATH=~:$PATH
hacker@path~hijacking-commands:~$ chmod uog+x rm
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
Found 'rm' command at /home/hacker/rm. Executing!
pwn.college{QhqYNyNF3ViRnijR-hW3JzDtu6v.ddzNyUDLycTN0czW}
````
