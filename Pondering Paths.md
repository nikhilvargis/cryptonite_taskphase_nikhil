#  Pondering Paths

## The Root
We invoke the pwn program by using the command  '/pwn' to obtain the flag.
### flag:
```pwn.college{IltAD57FtyiyOzzudqaNLktQP6v.dhzN5QDLwEjN0czW}```
##

## Program And Absolute Paths
 / denotes the main directory in which the challenge directory is located.We need to access the challenge program 'run' in the challenge directory and hence we use the command /challenge/run to obtain the flag.
### flag:
```pwn.college{ot0AXLQnC9yQTDdwDP5unUp47Ie.dVDN1QDL4QTN0czW}```
##

## Position Thy Self
After assuming that the flag was located in the challenge directory I used the 'cd' command to navigate to the given directory and then terminal indicated that it was located in the /proc/381/fd. After navigating to this directory I invoked the command and obtained the flag.
### flag:
```pwn.college{EigPsRxonG4jK9B1QBbE5GtPnFS.dZDN1QDL4QTN0czW}```
##

## Position Elsewhere
similar process to the previous one
### flag:
```pwn.college{QiN8Ieb9-zjRF39rYQgV0I5QGKF.ddDN1QDL4QTN0czW}```
##

## Position Yet Elsewhere
similar process to the previous one.
### flag:
```pwn.college{Ak14ETeeXPIttD19w3uKTcXdUaQ.dhDN1QDL4QTN0czW}```
##

## Implicit Relative Paths, From /
It is  given that the cwd was /,so we  run 'challenge/run' for the flag because it was the relative path from '/'.
### flag:
```wn.college{0ODl_j28X2HAgAKWf9SHcyrhSDa.dlDN1QDL4QTN0czW}```
##

## Explicit Relative Paths, From /
I had  to switch to / directory as mentioned in the challenge using the 'cd' command then invoked the relative path ./challenge/run for the flag because they wanted it to start with "."
### flag:
```pwn.college{Yz-Iis_aEfjD47NSMKOtG7UJp6b.dBTN1QDL4QTN0czW}```
##

## Implicit Relative Path
Using the 'cd' command, we switch to the challenge directory and since run is a naked path, we use a relative path ./run as they want it to start with '.'.
### flag:
```pwn.college{sWfaPCcWfoVOkigMqDsThaG_Pfe.dFTN1QDL4QTN0czW}```
##

## Home Sweet Home
We run the command /challenge/run with an argument '~/a'. The ~  means that it is referring to the home directory meaning ~/x is now an absolute path for the file '/x'
### flag:
```pwn.college{09v4rwnuVlMaS5lpp-1qAJhrXT-.dNzM4QDL4QTN0czW}```
##
