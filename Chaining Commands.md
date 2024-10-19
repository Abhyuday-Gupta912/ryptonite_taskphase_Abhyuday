# CHAINING COMMANDS

## CHAINING WITH SEMICOLONS
### FLAG: pwn.college{s0vFH8qhQtDTGRwa69bYUJUdE75.dVTN4QDLycTN0czW}
### APPROACH USED:
````
/challenge/pwn ; /challenge/college
````

## YOUR FIRST SHELL SCRIP
### FLAG: pwn.college{osNMxWfnT2KAcm4RTvERsZ-rMYB.dFzN4QDLycTN0czW}
### APPROACH USED:
````
hacker@chaining~your-first-shell-script:~$ touch x.sh
hacker@chaining~your-first-shell-script:~$ nano x.sh
hacker@chaining~your-first-shell-script:~$ bash x.sh
Great job, you've written your first shell script! Here is the flag:
pwn.college{osNMxWfnT2KAcm4RTvERsZ-rMYB.dFzN4QDLycTN0czW}
````

## REDIRETINF SCRIPT COMMAND
### FLAG: pwn.college{IGhSuGFxCraHh3fxhXTJAGvebUI.dhTM5QDLycTN0czW}
### APPROACH USED:
````
hacker@chaining~redirecting-script-output:~$ touch script.sh
hacker@chaining~redirecting-script-output:~$ nano script.sh
hacker@chaining~redirecting-script-output:~$ bash script.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{IGhSuGFxCraHh3fxhXTJAGvebUI.dhTM5QDLycTN0czW}
````

## EXECUTABLE SHELL SCRIPTS
### FLAG: pwn.college{ocPV9sbcbTDBNtSaUFPNRbNvgxf.dRzNyUDLycTN0czW}
### APPROACH USED:
````
hacker@chaining~executable-shell-scripts:~$ touch exec.sh
hacker@chaining~executable-shell-scripts:~$ nano exec.sh
hacker@chaining~executable-shell-scripts:~$ chmod ugo+x exec.sh
hacker@chaining~executable-shell-scripts:~$ ./exec.sh
Congratulations on your shell script execution! Your flag:
pwn.college{ocPV9sbcbTDBNtSaUFPNRbNvgxf.dRzNyUDLycTN0czW}
````