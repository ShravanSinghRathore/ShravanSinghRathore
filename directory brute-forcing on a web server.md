### Dirsearch: Recursively scans a target URL for directories and files using common names.

Command: **python3 dirsearch.py -u http://<target_ip>**


## Gobuster: Brute-forces directories on a target URL using a specified wordlist.
Command: **gobuster dir -u http://<target_ip> -w /path/to/wordlist.txt**


## Wfuzz: Fuzzes directory names on a target URL using a specified wordlist.
Command: **wfuzz -c -z file,/path/to/wordlist.txt --hc 404 http://<target_ip>/FUZZ**


## Feroxbuster: Performs fast, recursive content discovery on a web server.
Command: **feroxbuster -u http://<target_ip> -w /path/to/wordlist.txt**


## Dirbuster: Brute-forces directories and files on a web server using a specified wordlist.
Command: **java -jar DirBuster-<version>.jar -u http://<target_ip> -w /path/to/wordlist.txt**



### Each command is tailored for directory brute-forcing on a web server, helping security professionals identify potential vulnerabilities and attack vectors.
