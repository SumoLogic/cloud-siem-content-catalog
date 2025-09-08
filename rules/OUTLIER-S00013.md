# [Rules](README.md): Outlier in Data Outbound Per Day by Admin or Sensitive Device

## Description
A larger than typical amount of data has been observed being sent outbound from a Sensitive Device or an Admin user. It is recommended to investigate the device associated with this IP, the Internet destinations and traffic associated with this anomalous behavior. A normalized record search for the source IP and external network traffic, within the period of time of the detection will help identify suspicious activity. This rule is dependent on the Match Lists "domain_controllers" and "admin_usernames" being populated with the sensitive device IPs and admin usernames. Additionally, Entity Tagging offers a similar and extensible alternative to Match Lists. To add more sensitive Match Lists, or Entity Tagging, please use Rule Tuning Expressions. For further customization, consider adjusting the severity of this rule and/or using entity severity as needed to increase the severity of this rule.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Exfiltration|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Daily Outlier in Outbound Data Sent from Sensitive Device or Admin User - Source IP: {{srcDevice_ip}}|
|Summary Expression|A larger than typical amount of data was sent outbound from {{srcDevice_ip}}|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Standard Deviation Threshold|3|
|Floor Value|1000000000|
|Score/Severity|Static: 0|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1030, _mitreAttackTechnique:T1071, _mitreAttackTactic:TA0010, _mitreAttackTactic:TA0011|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cisco Systems - Firepower](../products/da9e05a5-3fd3-46a7-a107-ae03c01e3f5a.md)
- [Dell - Firewall](../products/b1639f7f-4c11-4d29-ab69-368cf0e05e25.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bytesOut|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|listMatches|
|Normalized Schema|objectClassification|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|user_username|


