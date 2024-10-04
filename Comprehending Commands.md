## cat: not the pet, but the command!
The cat command is used for reading out files( single file or multiple files at the same time). In the home directory, we invoke the command 'cat' on the 'flag' file.
### flag:
```
pwn.college{MY8wtnretsnY-fTU94qmTVUFqOo.dFzN1QDL4QTN0czW}
```

## catting absolute paths
To specify the arguments of the 'cat' command as absolute paths, we use /flag as the argument to obtain flag.
### flag:
```
pwn.college{EOyUi11JlnPbT3ZYyDAbwT4W-uz.dlTM5QDL4QTN0czW}
```

## more catting practice

To obtain the flag with using the 'cd' command to change directories and to directly read the file from the given directory. We invoke the 'cat' command on the absolute path /lib/ecl/flag
### flag:
```
pwn.college{k89qz7Q9DEA_GunCAIic3Tr3_uu.dBjM5QDL4QTN0czW}
```

## Grepping for a needle in a haystack
For extremely large files, we use the 'grep' command to search for the contents we need.In this challenge, grep searches /challenge/data.text for the substring pwn.college and obtains the flag
### flag:
```
pwn.college{cbc1IGCu8YQ5FRyJE3HakCI66hs.ddTM4QDL4QTN0czW}


```



## Listing Files
On listing the /challenge directory, we find that /challenge/run is renamed to 14735-renamed-run-7150. Thus we run it using /challenge/14735-renamed-run-7150 and obtain the flag.
### flag:
```
pwn.college{U2b_o1n7alKxx5GJGuu88UZEjNa.dhjM4QDL4QTN0czW}
```

## Touching Files
You can now create a file using the touch command! We create pwn and college and use ls /tmp
to check whether both files pwn and college are there. After that we run the command /challenge/run to obtain the flag.
### flag:
```
pwn.college{Y1aeXgzplZqPv5BptgYOWiUzlzg.dBzM4QDL4QTN0czW}
```
## Removing Files
We can remove files using the rm command. Using the previous touch command, we create a delete_me and use rm to delete the file. We then use /challenge/check to obtain the given flag.
### flag:
```
pwn.college{o34eCHuLyxeoLjWaWuLk7hMSBZ3.dZTOwUDL4QTN0czW}
```

## Hidden Files
 We use the ls -a command to view the files starting with a . as well, as by convention Linux does not list files starting with '.'.On using ls -a in the / directory, we see a file .flag-11254221316221. On invoking the cat command on this file, we get the flag.
### flag:
```
pwn.college{cJwn1ubkRRsXHSJmIKLP1GzeOCf.dBTN4QDL4QTN0czW}
```

## An Epic Filesystem Quest
 