# [Rules](README.md): Spike in PowerShell Command Line Length From Host

## Description
Observes for PowerShell command lines with excessive length found on a given system based on a daily outlier of standard deviation using a designated historic baseline of what has been previously observed for said system. The minimum PowerShell command line length expected by default is set to 3 characters.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Execution|
|Apply Risk to Entities|device_hostname|
|Signal Name|Spike in PowerShell Command Line Length From Host: {{device_hostname}}|
|Summary Expression|Excessive PowerShell command line length identified for Host: {{device_hostname}} based on daily historic activity|
|Retention Window|7776000000|
|Baseline Window|1296000000|
|Standard Deviation Threshold|3|
|Floor Value|3|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1059.001|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [VMware - Carbon Black Cloud](../products/f9cea291-9030-4e41-9836-6dd9274d6df4.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|isEmpty|
|Normalized Schema|metadata_deviceEventId|


