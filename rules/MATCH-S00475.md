# [Rules](README.md): Renamed MSBUILD.EXE by Arguments

## Description
From FireEye Red Team Tool Countermeasures: This alert looks for renamed msbuild.exe process executions based on common command line arguments used for msbuild.exe. Attackers frequently use msbuild.exe (or renamed versions of this binary) to execute arbitrary CSharp payloads written to disk most commonly as .csproj files (though any file with an extension ending in "proj" will work) either referenced on the command line or located in the same directory as the msbuild.exe binary. The XML payload on disk should be acquired and examined to determine the functionality of the payload.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, user_username, device_ip|
|Signal Name|Renamed MSBUILD.EXE by Arguments|
|Summary Expression|Detected MSBUILD.exe command line arguments on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1127.001, _mitreAttackTechnique:T1127|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|file_path|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


