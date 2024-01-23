# [Rules](README.md): Global YARA Rule

## Description
A YARA rule matched on a collected file

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|srcDevice_ip, dstDevice_ip|
|Signal Name|YARA rule match: {{fields.yaraRuleName}}|
|Summary Expression|YARA rule: {{fields.yaraRuleName}} hit on a collected file with associated source IP: {{srcDevice_ip}} and destination IP: {{dstDevice_ip}} with description: {{fields.yaraRuleDescription}}|
|Score/Severity|None|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_ip|
|Direct from Record|fields.yaraRuleName|
|Direct from Record|fields.yaraRuleSeverity|
|Direct from Record|fields.yaraStatus|
|Normalized Schema|srcDevice_ip|


