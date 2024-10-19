# Processes and Jobs
We learn how to view and interact with processes

## Listing Processes
.The ps command is used to list every running process. We can use ps -ef to list every process in full format and ps -aux to list all processes for all users, process not running in the terminal and for a user readable output. In this  case we use ps -ef to check what the /challenge/run fil has been renamed to and run that file to obtain the flag.
### flag:
```pwn.college{4a2qP4DzCioywK83cx7bQM31zeg.dhzM4QDL4QTN0czW}```

## Killing Processes
We can use the kill command to eliminate a process by passing the PID as an argument. we kill the process /challenge/dont_run to invoke the /challenge/run command to obtain the flag.
### flag:
```pwn.college{oIelXhx12kUdX00KPyHtYSgYoL9.dJDN4QDL4QTN0czW}```

## Interrupting Processes
Instead of using the kill command, we can do Ctrl-C that sends an interrupt to whatever application is waiting on input from the terminal and, typically, this causes the application to cleanly exit. I used the /challenge/run command and pressed Ctrl C to obtain the flag.
### flag:
```pwn.college{YlkQXDZLd_A3hIjndcz7ifm5VG-.dNDN4QDL4QTN0czW}```

## Suspending Processes
we can suspend properties using Ctrl Z. In this challenge, we need 2 copies of .challenge/run to obtain the flag. So I suspend one process and run another to obtain 2 and hence the flag.
### flag:
```pwn.college{Uqg4O2LSz792E56nqpiWKDJmWQU.dVDN4QDL4QTN0czW}```

## Resuming Processes
After suspending properties, we can resume them in the foreground by using the fg command. We suspend /challenge/run then resume it to obtain the flag.
### flag:
```pwn.college{U_27PU5U_tVJSezAedaycJUwwr3.dZDN4QDL4QTN0czW}```

## Backgrounding Processes
We can resume processes in the background by bg command. In this challenge, we need 2 copies of /challenge/run to obtain the flag hence we suspend, resume in background and run /challenge/run to obtain the flag.
### flag:
```pwn.college{YvYgV3Y5ZECsNT-nfmLo78g6-Up.ddDN4QDL4QTN0czW}```

## Foregrounding Processes
We can foreground backgrounded processes with fg just like with a suspended process.
### flag:
```pwn.college{oIelXhx12kUdX00KPyHtYSgYoL9.dJDN4QDL4QTN0czW}```

## Starting Backgrounded Processes
We don't have to suspend processes to background them. We can background processes by appending & to the command and hence we can obtain the flag by appending & to /challenge/run
### flag:
```pwn.college{k_aMmry5IsUAVAAko5iugZLyrFo.dlDN4QDL4QTN0czW}```

## Process Exit Codes
We can access the exit code of a command by using the ? variable. If it returns 0 it was successful and else it failed. We retrieve the exit code of /challenge/get-code and pass the error code as an argument for /challenge/submit-code to obtain the flag.

### flag:
```pwn.college{U3UAX_mxMcPmsmfM5_DB-9kuIh4.dljN4UDL4QTN0czW}```