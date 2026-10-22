# [Rules](README.md): Web Services Executing Common Web Shell Commands

## Description
Detection: This rule detects a web server process (IIS, Apache, Nginx, Tomcat, or PHP-CGI, on Windows or Linux) executing command-line reconnaissance or network utilities (whoami, net user, ping, systeminfo, netstat, arp, ipconfig/ifconfig, curl, wget, id, uname, cat /etc/passwd, or netcat) as a child process.

Scenario: These commands are commonly run by attackers who have successfully uploaded and are interacting with a web shell to perform reconnaissance, establish a reverse shell, or pivot further into the environment. Legitimate web server processes have no routine need to execute these commands.

Recommended Actions: Review commandLine for the full command executed, correlate with device_hostname and user_username, and inspect the web application directory for unauthorized script or web shell files.

Tuning Recommendations: If legitimate monitoring agents or health-check scripts invoke these commands from web server processes, exclude the specific commandLine patterns or source hosts via a match list rather than removing the parent/child process conditions.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Web Services Executing Common Web Shell Commands|
|Summary Expression|Observed common web shell commands on host: {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTactic:TA0007, _mitreAttackTechnique:T1082, _mitreAttackTechnique:T1505, _mitreAttackTechnique:T1505.003|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


