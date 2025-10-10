# [Rules](README.md): Threat Intel - Inbound Traffic from Threat Feed IP (Low Confidence)

## Description
This rule detects allowed inbound traffic from an IP address with a low confidence rating from a threat intelligence feed.
Note that this rule is disabled by default due to a high likelihood of excessive signal volume and risk assignment to entities triggering this rule as-is. Tuning to reduce signal volume and potential false positives is highly recommended before activating this rule.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Threat Intelligence|
|Apply Risk to Entities|srcDevice_ip, dstDevice_ip, device_ip, srcDevice_ip, srcDevice_hostname, srcDevice_hostname, dstDevice_hostname, device_hostname, user_username|
|Signal Name|Threat Intel - Inbound Traffic From Low Confidence Threat IP|
|Summary Expression|Successful inbound network traffic from a low confidence Threat IP address {{srcDevice_ip}}}|
|Score/Severity|Static: 1|
|Enabled by Default|False|
|Prototype|False|
|Tags||
## Vendors and Products
- [Amazon AWS - AWS S3 Server Access Logs](../products/41f70c6e-18a9-462c-a04d-4edc7baead7a.md)
- [Amazon AWS - VpcFlowLogs](../products/021d1ded-1c82-4663-bf5d-d6ed5170efa3.md)
- [Amazon AWS - Web Application Firewall (WAF)](../products/072b85a2-1765-45c2-911d-b0509880326e.md)
- [CheckPoint - Firewall and VPN](../products/c3c1a4fc-10cc-4155-8a30-a3bb14fc9f31.md)
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Google - BigQuery](../products/a67d97fe-6e68-4cfb-9500-cfc5492da565.md)
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - IIS](../products/fca8785d-4823-4442-86b2-8acbaa176da4.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|OR|
|Normalized Schema|confidence|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|success|
|Normalized Schema|type|
|Normalized Schema|user_username|


