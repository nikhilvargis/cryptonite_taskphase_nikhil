# Shells and Variables

## Printing Variables
The flag is stored in the variable FLAG. We use the command echo to read the flag from the variable FLAG. $ is used to access variables.
### flag:
```pwn.college{4vnSxsjaQMWbikD30mrBDSVyZ3v.ddTN1QDL4QTN0czW}```

## Setting Variables
we can also assign values to variables however there should be no spaces around the = sign otherwise it will be read as a command. We assign the value COLLEGE to the variable PWN>
### flag:
```pwn.college{o_ttsJFGVjm2_ZKnBSE74d4PM7s.dlTN1QDL4QTN0czW}```

## Multi-worded Variables
As soon the terminal reads a space character during a variable assignment, it ends it and reads the rest as a command. To prevent this, we put the value in "" and can obtain the flag.
### flag:
```pwn.college{weKsdW0B-rbMqpj6Wrr6jjT1eU9.dBjN1QDL4QTN0czW}```

## Exporting Variables
Learned that variables you set in a shell are local to the shell process. We need to export these variables as other commands wont inherit them. We follow the instructions in the challenge and obtain the flag
### flag:
```pwn.college{wJmPxJvA6zpF607JKOG2mMF66ym.dJjN1QDL4QTN0czW}```

## Printing Exporting Variables
We use the env command to print out every exported variable and find the FLAG variable.
###flag:
```pwn.college{oeFU9rDwtJ_Nyxvg_bTBWAGRDEK.dhTN1QDL4QTN0czW}```
 
## Storing Command Output
We can store command output in a variable. We do Command Substitution with the PWN variable and obtain the flag.
### flag:
```pwn.college{0mc_SPANUFp2ck_SWEmixHtw6gJ.dVzN0UDL4QTN0czW}```

## Reading Input
read command reads the input and using this we obtain the flag.
### flag:
```pwn.college{swUdfDbes1HkeXP-ACaMbP8FVin.dhzN1QDL4QTN0czW}```

## Reading Files
We read the /challenge/read_me into the PWN variable and obtain the flag.
### flag:
```pwn.college{w0jKSuNcDrQkOXCGTSh_PlRlZrx.dBjM4QDL4QTN0czW}```
