# [Rules](README.md): OCSF Compliance Finding

## Description
Passes through compliance findings from OCSF sources.

Compliance Control: {{fields['compliance.control']}} 
Finding Info: {{fields['finding_info.desc']}} 
Finding Origin: {{fields['metadata.product.name']}}

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|resource, user_username|
|Signal Name|OCSF Compliance Finding: {{threat_signalName}}|
|Summary Expression|Unresolved compliance issue detected on {{resource}} ({{resourceType}}) . {{threat_signalSummary}}|
|Score/Severity|Dynamic: 0 or 1 or 3 or 5 or 6|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Amazon AWS - Security Hub](../products/d0aebc1c-db4d-440f-b69f-70dae24befff.md)


## Dynamic Signal Score/Severity Translation

The default score of `0` is used as a catch all if none of the translations are met.

|Schema Field|Field Value|Score/Severity|
|------------|-----------|--------------|
|normalizedSeverity|0|0|
|normalizedSeverity|1|1|
|normalizedSeverity|3|3|
|normalizedSeverity|5|5|
|normalizedSeverity|6|6|
## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields['activity_name']|
|Direct from Record|fields['activity_uid']|
|Direct from Record|fields['category_name']|
|Direct from Record|fields['category_uid']|
|Direct from Record|fields['class_name']|
|Direct from Record|fields['class_uid']|
|Direct from Record|fields['compliance.control']|
|Direct from Record|fields['finding_info.desc']|
|Direct from Record|fields['metadata.product.name']|
|Direct from Record|fields['status']|
|Direct from Record|fields['status_id']|
|Normalized Schema|normalizedSeverity|
|Normalized Schema|resource|
|Normalized Schema|threat_ruleType|
|Normalized Schema|threat_signalName|
|Normalized Schema|user_username|


