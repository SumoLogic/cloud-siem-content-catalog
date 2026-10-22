# [Rules](README.md): Suspicious Shells Spawned by Web Servers

## Description
Detection: This rule detects a web server process (IIS, Apache, Nginx, Tomcat, or PHP-CGI, on Windows or Linux) spawning a shell or scripting interpreter (cmd, PowerShell, bash, sh, python, perl, etc.) as a child process.

Scenario: Web servers have no legitimate operational need to launch command shells. When this occurs, it typically indicates an attacker has exploited a vulnerability in the web application to achieve remote code execution, often to establish persistence via a web shell or pivot further into the environment.

Recommended Actions: Review commandLine for the exact command executed, check device_hostname and user_username to identify the affected host and account context, and inspect the web application and file system for newly dropped web shell files or unauthorized script modifications.

Tuning Recommendations: If legitimate automation or administrative scripts regularly invoke shells from these web server processes, exclude the specific commandLine patterns or source hosts via a match list rather than removing the parent/child process conditions.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Suspicious Shells Spawned by Web Servers|
|Summary Expression|Parent process: {{parentBaseImage}} spawned process: {{baseImage}} on host: {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1505, _mitreAttackTechnique:T1505.003|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


