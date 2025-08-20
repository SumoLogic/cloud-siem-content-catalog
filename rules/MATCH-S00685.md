# [Rules](README.md): Authentication Without MFA

## Description
A login was successful where the account did NOT use multi-factor authentication (MFA) to gain access. It is strongly recommended that all accounts used for access require MFA to protect the account in the event credentials are stolen. If MFA is required, it is recommended this rule be enabled for that vendor/product.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|srcDevice_hostname, srcDevice_ip, device_ip, device_hostname, user_username|
|Signal Name|{{metadata_vendor}} {{metadata_product}} - Authentication Without MFA|
|Summary Expression|{{user_username}} logged on without MFA|
|Score/Severity|Static: 0|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTactic:TA0001, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1586, _mitreAttackTechnique:T1078.004, _mitreAttackTechnique:T1586.002|
## Vendors and Products
- [Alibaba - ActionTrail](../products/79055042-52c8-4998-b201-bd2cd2dbca1f.md)
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)
- [JumpCloud - IdP](../products/1ed80351-d779-4f1f-9ddb-b3881f19d487.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|isNull|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|mfa|
|Normalized Schema|normalizedAction|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|success|
|Normalized Schema|user_username|


