# Command to collect Volatile information from Windows

## command we will use is to store the date and time of the system.

> echo %date% %time% > liveIR-050517.txt

## take a snapshot of the currently running tasks:

> tasklist >> liveIR-050517.txt
> tasklist /m >> liveIR-050517.txt
> tasklist /svc >> liveIR-050517.txt


## take a snapshot of the currently available network connections:

> netstat -nao >> liveIR-050517.txt

## ASvailable MAC addresses that are in the system's ARP Cache:

> arp -a >> liveIR-050517.txt

## Network configuration:

> ipconfig /all >> liveIR-050517.txt


## DNS configurations:

> ipconfig /displaydns >> liveIR-050517.txt


## Routing configurations:

> route print >> liveIR-050517.txt

## System variables have been set:

> set >> liveIR-050517.txt

## System user information:

> net user %username% >> liveIR-050517.txt
> net use >> liveIR-050517.txt


## Network shares:

> net share >> liveIR-050517.txt

## Workstation information:

> net config workstation >> liveIR-050517.txt

## System information:

> systeminfo >> liveIR-050517.txt
