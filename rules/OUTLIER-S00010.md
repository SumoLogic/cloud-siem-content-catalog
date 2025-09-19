# [Rules](README.md): Spike in URL Length from IP Address

## Description
Observes for an outlier in URL length sourcing from an IP Address based on a daily standard deviation using a designated historic baseline of what has been previously observed for said IP Address. This type of anomaly can linked with web based execution of Command and Control. The minimum URL length expected by default is set to 128 characters.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Command and Control|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Spike in URL Length from IP Address: {{srcDevice_ip}}|
|Summary Expression|Excessive URL length identified for IP Address: {{srcDevice_ip}} based on daily historic activity|
|Retention Window|7776000000|
|Baseline Window|1296000000|
|Standard Deviation Threshold|3|
|Floor Value|128|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1102|
## Vendors and Products
- [Akamai - SIEM](../products/9a28f2af-5526-414d-973b-c3fc7984b8a1.md)
- [Amazon AWS - Application Load Balancer](../products/5bb9e0b3-8d57-4b10-8952-0b6ffe91b599.md)
- [Amazon AWS - CloudFront](../products/44f07c08-c2ad-4a95-a058-1d0737ff90db.md)
- [Amazon AWS - EKS](../products/234ec2b5-4142-4837-bc78-95da8a2db81a.md)
- [Amazon AWS - Web Application Firewall (WAF)](../products/072b85a2-1765-45c2-911d-b0509880326e.md)
- [Apache - Apache HTTP Server](../products/6787d77a-1ee0-43d4-8ca0-96af8ee755bc.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cisco Systems - Ironport](../products/c07b5749-deda-4c7e-8e78-4a5dec1fcf4d.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Cisco Systems - Umbrella](../products/5ba50e74-3c05-4ea8-aeaf-5efde588c60f.md)
- [Forcepoint - Web Security](../products/e90edc67-68d4-4d67-82f6-4524f94b59bb.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)
- [Imperva - Imperva Incapsula](../products/2a236ab1-77d2-4867-a571-a1cfd64528e6.md)
- [McAfee - Web Gateway](../products/003d35b3-3ba8-4e93-8776-e5810b4e243e.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - IIS](../products/fca8785d-4823-4442-86b2-8acbaa176da4.md)
- [Squid - Squid Proxy](../products/af61d8a8-3eba-42fb-9f17-87443924f3f4.md)
- [Symantec - Web Security Service](../products/bf865cb5-0b26-4010-8b3c-5ae2d1f716d8.md)
- [Zscaler - Firewall](../products/9e0641a7-22ce-4ac8-8113-ee48b368ac3d.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|http_url|
|Normalized Schema|http_userAgent|
|Normalized Schema|isEmpty|
|Normalized Schema|listMatches|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_ip|


