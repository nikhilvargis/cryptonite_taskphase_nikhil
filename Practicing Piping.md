# Practicing Piping

## Redirecting output
We learn that we can redirect output of any command to a file. Hence in this challenge, we assign the output of echo PWN to the file COLLEGE and obtain the flag.
### flag:
```pwn.college{0OkNiYGSWuQaWDkMrxmRhXiGTLB.dRjN1QDL4QTN0czW}```

## Redirecting more output
same process as the previous one and read the output
### flag:
```pwn.college{YER-TWjM8AjA3nekldH2MoF96Ix.dVjN1QDL4QTN0czW}```

## Appending Output
We assign the out of /challenge/run to /home/hacker/the-flag. We then append /challenge/run to the same file and read the file to obtain the flag.
### flag:
```pwn.college{ABUOYH5FI-dbujhWI4Rj1b3FHiS.ddDM5QDL4QTN0czW}```
## Redirecting errors
We learn that we use > to redirect output, 2> to redirect errors and 0> to redirect input. Here we redirect the output of /challenge/run to myflag and the errors of my flag to instructions. We read myflag to obtain flag.
### flag:
```pwn.college{o9X5RuI2dMMKcoMOd4v2POV_48P.ddjN1QDL4QTN0czW}```
## Redirecting input
We assign output of echo COLLEGE into PWN and then assign PWN to /challenge/run and obtain flag
### flag:
```pwn.college{YM2puFXH_aqEwPdg-BnYE88rREB.dBzN1QDL4QTN0czW}```
## Grepping stored results:
we assign /challenge/run to /tmp/data.txt and use grep pwn.college /tmp/data.txt to find the flag
### flag:
```pwn.college{koeFc-2yw32YP9EUgn324yduye7.dhTM4QDL4QTN0czW}```
## Grepping Live Output
This is actually really cool! Instead of storing /challenge/run in some other file we can use the | operator to grep and cut out the middleman to obtain the flag.
### flag:
```pwn.college{I2yoq1Q5tU9_bZUiKAILzkA-sTs.dlTM4QDL4QTN0czW}```
## Grepping errors
There's no | operator for errors and it redirects only standard output to a program. Luckily there is an operator >& which redirects a FD to another FD. In this challenge, we redirect std error to std output 2>& 1 and grep using | operator to obtain the flag.
### flag:
```pwn.college{si2Z_HCl6CmzVeH-saz4VdEMIJ_.dVDM5QDL4QTN0czW}```
## duplicating-piped-data-with-tee:
We use ' tee test' in between /challenge/pwn and /challenge/college to check the secret commands and obtain the flag.
### flag:
```pwn.college{QTfCxxpHa6Nv3vI4N_YlCuJSolz.dFjM5QDL4QTN0czW}```
## Writing mulitple programs
### flag:
``` ```
## Redirecting output
### flag:
``` ```
