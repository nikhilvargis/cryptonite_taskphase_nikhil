# File Globbing

## Matching with *
In this module, we learn about globs. Anytime we encounter a * in the argument, it is treated as multiple character wildcard and the shell will replace it with files of similar patterns. It matches any part of the filename, except / or a leading '.'.In this challenge, to cd to the challenge directory, we use cd/c*e as atmost 4 characters are allowed in the challenge. We then obtain the flag.
### flag:
pwn.college{09b2MbAIFCg5fYBrx9FOS9gucd8.dFjM4QDL4QTN0czW}

## Matching with ?
Here, we use the glob '?' and it acts a single character wildcard. To cd into the challenge directory, as specified in the challenge, we use ? in place of c and l obtain the flag
### flag:
pwn.college{wvx1HWYkvk3o4kdgXncCnqNtxCd.dJjM4QDL4QTN0czW}

## Matching with []
This glob '[]' is essentially a limited form of the '?' glob as it can replaces files with only the specified characters in the []. In this challenge, we cd into the /challenge/files directory, run the /challenge/run with the file_[bash] argument and obtain the flag.
### flag:
pwn.college{A7iA3wGXNhEkKS3dFpY7A2FAMzQ.dNjM4QDL4QTN0czW}

## Matching paths with []
We learn that globbing happens on a path basis. We can expand entire paths with globbed arguments. Here we run /challenge/run command in the home directory using the argument /challenge/files/files_[bash] and obtain the flag.
### flag:
pwn.college{AN1Z20LBo9i3ifvf0eq9D8INZsa.dRjM4QDL4QTN0czW}

## Mixing globs
### flag:

## Exclusionary Globbing 
### flag:

