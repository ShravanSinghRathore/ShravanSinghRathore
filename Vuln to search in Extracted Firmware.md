
## This command utilizes the Dirb tool for directory brute-forcing on a target web server. Here's what it does:
Dirb: Brute-forces directories and files on a target web server using a specified wordlist.

Command: **dirb http://<target_ip> /path/to/wordlist.txt**

## Here's the command for using Nikto:

Nikto: Scans a target web server for vulnerabilities and misconfigurations.

Command: **nikto -h http://<target_ip>**



# For Binary testing Command, follow the below
Entropy:
**ent Firmware.bin**

**grep -r -i -E 'username|password'**

Search for Common Vulnerability Patterns:        **grep -r -i -E 'password|secret|api_key'**


Scan for Format String Vulnerabilities:         **grep -r -i -E '%[a-zA-Z0-9_]{1,10}'** 

Search for Dangerous Function Calls( Command Injection Vulnerablity ):          **grep -r -i -E 'system\(|exec\(|shell_exec\(|passthru\(|popen\('** 


**grep -r -i -E 'gets\(|strcpy\(|sprintf\(|printf\(|scanf\('**

**grep -r -i -E 'mysql_query\(|mysqli_query\(|pg_query\(|execute\(|query\('**


**grep -r -i -E 'http_|ftp_'**

**grep -r -i -E 'malloc\(|free\(|memcpy\(|memset\('**


**grep -r -i -E 'api_key|secret_key'**


Check for File Permission Issues::         **find -type f ! -perm 600 -exec ls -l {} \;**

Identify Sensitive Information in Logs:          **grep -r -i -E 'apikey|token|password' /var/log** 

Look for Code Injection Points:             **grep -r -i -E 'system\(|exec\(|eval\('**


Check for Cross-Site Scripting (XSS) Patterns:          **grep -r -i -E 'echo\(|print\(|printf\(|document\.write\('**


Search for Dangerous System Calls:                **grep -r -i -E 'system\(|popen\(|exec\(|shell_exec\('**

Examine Cryptographic Implementations:            **grep -r -i -E 'md5\(|sha1\(|base64_encode\('**


Check for Unprotected Database Connections:        **grep -r -i -E 'mysql_connect\(|mysqli_connect\(|pg_connect\('**


**strings Firmware.bin | grep -iE "version|firmware|release"**


Check Running Processes:
**ps aux**

Check Listening Ports:
**netstat -tulpn**

Check Open Files:
**lsof**

Check Network Connections:
**netstat -an**

Check Log Files:
**View system logs:**

**cat /var/log/syslog**

View authentication logs:

**cat /var/log/auth.log**

Check User Accounts:


**cat /etc/passwd**

Check SUID/SGID Binaries:


**find / -type f \( -perm -4000 -o -perm -2000 \) -exec ls -l {} \;**

Check Startup Services:

**systemctl list-units --type=service
**
Check Modified Files:

**find / -mtime -1**

Check for Rootkits:


**rkhunter --check**

Check for Malware and Viruses:

**clamscan -r /**

Check Network Traffic:


**tcpdump -i eth0**



# Analyze all files in the current directory for sensitive information
**strings * | grep -iE 'password|auth|key|config|credentials'**

# Analyze all files in the current directory for configuration-related strings
**strings * | grep -iE 'config|settings|conf'**

# Analyze all files in the current directory for network-related information
**strings * | grep -iE 'ip|port|network'**

# Analyze all files in the current directory for error messages or vulnerabilities
**strings * | grep -iE 'error|exception|vulnerable|exploit'**

# List detailed information about all files in the current directory
**ls -l**

# Cat contents of all files named "configuration_file" in the current directory
**cat configuration_file**


![MicrosoftTeams-image](https://github.com/ShravanSinghRathore/ShravanSinghRathore/assets/161594463/97169dbd-e5c1-4a0d-880f-e614cdcd81a8)
![MicrosoftTeams-image (12)](https://github.com/ShravanSinghRathore/ShravanSinghRathore/assets/161594463/61d0ed31-93eb-4d72-be90-9ce3984e8f91)
![MicrosoftTeams-image (10)](https://github.com/ShravanSinghRathore/ShravanSinghRathore/assets/161594463/a5d4280a-c343-4b3c-9b6a-d74e589bb82e)
![MicrosoftTeams-image (9)](https://github.com/ShravanSinghRathore/ShravanSinghRathore/assets/161594463/016706b4-37fb-47f6-b3a2-2e564f222359)
![MicrosoftTeams-image (8)](https://github.com/ShravanSinghRathore/ShravanSinghRathore/assets/161594463/9baf14c6-e39d-4deb-8ef2-02ad581b44cb)
![MicrosoftTeams-image (7)](https://github.com/ShravanSinghRathore/ShravanSinghRathore/assets/161594463/e587e9df-884d-4c18-a982-5a3db630dd5a)
![MicrosoftTeams-image (6)](https://github.com/ShravanSinghRathore/ShravanSinghRathore/assets/161594463/62452c07-0eec-43da-bc36-68797b9b583c)
![MicrosoftTeams-image (5)](https://github.com/ShravanSinghRathore/ShravanSinghRathore/assets/161594463/8816d979-4a99-47f0-becf-2d36789d5f4e)
![MicrosoftTeams-image (4)](https://github.com/ShravanSinghRathore/ShravanSinghRathore/assets/161594463/45b8ac65-35e1-4809-a581-901d31314053)
![MicrosoftTeams-image (3)](https://github.com/ShravanSinghRathore/ShravanSinghRathore/assets/161594463/ad088607-80d6-4591-add2-d3cf3ed70191)
![MicrosoftTeams-image (2)](https://github.com/ShravanSinghRathore/ShravanSinghRathore/assets/161594463/e52401a0-7921-47b6-b425-8f9caf4ee60a)
![MicrosoftTeams-image (1)](https://github.com/ShravanSinghRathore/ShravanSinghRathore/assets/161594463/672c440f-0195-4a94-a451-81381c14a647)

