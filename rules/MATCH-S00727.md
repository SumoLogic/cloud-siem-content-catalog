# [Rules](README.md): CPL File Executed from Temp Directory

## Description
CPL files are DLL libraries that export a CPlApplet and are normally executed via the Windows Control Panel GUI interface. Having these files executed via the 'control' command from a temp directory is a strong indicator that an attacker has renamed a malicious DLL file as a CPL file and is attempting execution.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|CPL File Executed from Temp Directory|
|Summary Expression|User {{user_username}} exected a CPL file from a temp directory on host {{device_hostname}}|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1218.002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|user_username|


