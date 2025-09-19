# [Rules](README.md): Windows - Delete Windows Backup Catalog

## Description
Detects the deletion of backup catalogs on a Windows host through the command line. This activity is commonly seen in ransomware, where the program encrypts the host and deletes the backups to remove the possibility of restoring the computer and avoid paying the ransom.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Impact|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Windows - Delete Windows Backup Catalog|
|Summary Expression|Observed backup deletion on host: {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0040, _mitreAttackTechnique:T1490|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


