# [Rules](README.md): First Seen NTLM Authentication to Host (User)

## Description
A user has performed NTLM authentication to a host on the network for the first time since the baseline period has been established. Rule is disabled by default and requires tuning. Tuning guidance: depending on configurations in the environment, NTLM authentication may be necessary and expected. Examine the username, source IP and destination host in order to ensure that this activity is expected. Look at other signals around the entity in question to determine if any other type of suspicious activity may have occurred. It may also be prudent to isolate the rule to sensitive users and groups

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Credential Access|
|Apply Risk to Entities|user_username, device_hostname|
|Signal Name|First Seen User Performing NTLM Authentication to Host|
|Summary Expression|First Seen User: {{user_username}} Performing NTLM Authentication to Host: {{dstDevice_hostname}}|
|Retention Window|7776000000|
|Baseline Window|5184000000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 2|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1558, _mitreAttackTechnique:T1649|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Direct from Record|fields["EventData.AuthenticationPackageName"]|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


