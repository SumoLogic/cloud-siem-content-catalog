# [Rules](README.md): IIS - Executable File Added to Directory

## Description
Context:
Executable files added to Microsoft Internet Information Server (IIS) directories can indicate the installation of a web shell by an attacker. For example, the ToolShell exploit (CVE-2025-53770, CVE-2025-53771) included the installation of spinstall10.aspx in an executable directory.

Detection:
This detection will trigger when files executable by IIS are added to directories that frequently have execute permissions.

Recommended Actions:
Determine whether the addition of the executable file was an expected action, and if not, consider disconnecting the IIS server from the network for forensic analysis. Review logs indicating  unusual network activity originating from the IIS server to other internal assets.

Tuning Recommendations: 
Add executable directories specific to your IIS installation(s) to the rule expression by duplicating the rule and modifying it. Add exclusions as necessary to processes expected to add IIS script files to IIS directories.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname|
|Signal Name|IIS - Executable File Added to Directory on host {{device_hostname}}|
|Summary Expression|The executable file {{changeTarget}}   was added by process {{baseImage}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1505.003, _mitreAttackTechnique:T1505|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|normalizedAction|
|Normalized Schema|normalizedResource|


