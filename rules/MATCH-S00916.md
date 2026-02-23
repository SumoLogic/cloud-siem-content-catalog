# [Rules](README.md): macOS - pwpolicy getaccountpolicies usage detected

## Description
Within macOS and BSD, the pwpolicy command line tool can be used for Password Policy Discovery. This detects usage of pwpolicy and getaccountpolicies for the possible enumeration of password policies in a local directory. Tuning recommendations: this rule will detect MDM and Vulnerability Scanners using pwpolicy, it is recommended to create a tuning expression to filter the baseImages of validated automated processes, such as JamF, from this detection. Understanding the context of this command usage is important in determining the intent of execution, identifying the process executing the command (i.e. baseImage) will help determine if this is an automated process (MDM or Vulnerability Scanner) or if this is a user performing discovery.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|macOS - pwpolicy getaccountpolicies usage detected on {{device_hostname}}|
|Summary Expression|{{user_username}} ran pwpolicy getacccountpolicies on {{device_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1201, MITRE_Expansion_C2|
## Vendors and Products
- [Jamf - Jamf](../products/5c2cc0de-ca31-4ef0-bcfa-133fc8b387ad.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|user_username|


