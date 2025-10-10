# [Rules](README.md): GitHub Raw URL Resource Request

## Description
Github.com is the most popular code repo site on the internet. Typically users of GitHub will look at the code from the Github.com website or clone it locally to their system. You can however request a raw version of a individual file directly. Attackers like to use GitHub as well to host their malicious code and will often download malicious files and scripts directly from the site which uses the domain raw.githubusercontent.com instead of github.com. This signal looks for HTTP requests to that raw domain to monitor individual file downloads from the site.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Execution|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|GitHub Raw URL Resource Request|
|Summary Expression|Raw Github URL request from: {{srcDevice_ip}} to URL: {{http_url}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1204, _mitreAttackTechnique:T1204.001, _mitreAttackTechnique:T1204.002, _mitreAttackTechnique:T1204.003, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [CheckPoint - Firewall and VPN](../products/c3c1a4fc-10cc-4155-8a30-a3bb14fc9f31.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Sophos - UTM 9](../products/0fb003bc-8383-442f-8f3d-afcfbaefe617.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|http_hostname|
|Normalized Schema|http_url_path|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|


