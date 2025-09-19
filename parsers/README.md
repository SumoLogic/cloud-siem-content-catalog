# Parsers

The `type` listed lets you know if you can directly apply the parser to a collector to parse messages ingested by Sumo Logic and forwarded to Cloud SIEM or if it is used as a dependency to assist other parsers with the `[dependencies]` stanza.

|Type|Parser Path|
|----|-----------|
|Parser|/Parsers/System/1Password/1Password|
|Parser|/Parsers/System/1PasswordC2C/1PasswordC2C|
|Parser|/Parsers/System/AWS/AWS ALB|
|Parser|/Parsers/System/AWS/AWS CloudFront|
|Parser|/Parsers/System/AWS/AWS CloudWatch|
|Parser|/Parsers/System/AWS/AWS Config|
|Parser|/Parsers/System/AWS/AWS EKS|
|Parser|/Parsers/System/AWS/AWS ELB|
|Parser|/Parsers/System/AWS/AWS Inspector|
|Parser|/Parsers/System/AWS/AWS Network Firewall|
|Parser|/Parsers/System/AWS/AWS Redshift|
|Parser|/Parsers/System/AWS/AWS Route 53|
|Parser|/Parsers/System/AWS/AWS S3 Server Access Logs|
|Parser|/Parsers/System/AWS/AWS Security Hub|
|Parser|/Parsers/System/AWS/AWS VPC Flow|
|Parser|/Parsers/System/AWS/AWS VPC Transit Gateways Flow Logs|
|Parser|/Parsers/System/AWS/AWS VPN|
|Parser|/Parsers/System/AWS/AWS WAF|
|Parser|/Parsers/System/AWS/CloudTrail|
|Parser|/Parsers/System/AWS/GuardDuty|
|Parser|/Parsers/System/Abnormal Security/Abnormal Security|
|Parser|/Parsers/System/Adaxes/Adaxes Syslog|
|Parser|/Parsers/System/Airtable/Airtable Audit C2C|
|Parser|/Parsers/System/Akamai/Akamai CPC|
|Parser|/Parsers/System/Alert Logic/Alert Logic|
|Parser|/Parsers/System/Apache/Apache HTTP Server|
|Parser|/Parsers/System/Aqua/Aqua JSON|
|Parser|/Parsers/System/Atlassian/Atlassian Audit Events|
|Parser|/Parsers/System/Atlassian/Atlassian Confluence Access Logs|
|Parser|/Parsers/System/Atlassian/Atlassian Jira|
|Parser|/Parsers/System/Auth0/Auth0|
|Parser|/Parsers/System/Automox/Automox|
|Parser|/Parsers/System/Bandura/Bandura Syslog|
|Parser|/Parsers/System/Barracuda/Barracuda CloudGen|
|Parser|/Parsers/System/Barracuda/Barracuda WAF|
|Parser|/Parsers/System/Bitwarden/Bitwarden|
|Parser|/Parsers/System/Blue Coat/Blue Coat ProxySG|
|Parser|/Parsers/System/Blue Coat/Blue Coat ProxySG CEF|
|Parser|/Parsers/System/Blue Coat/Blue Coat ProxySG CSV|
|Parser|/Parsers/System/BlueCat/BlueCat DHCP-DNS Syslog|
|Parser|/Parsers/System/Cato Networks/Cato Networks|
|Parser|/Parsers/System/Check Point/Check Point Avanan JSON|
|Parser|/Parsers/System/Check Point/Check Point Firewall JSON|
|Parser|/Parsers/System/Check Point/Check Point Firewall Syslog|
|Parser|/Parsers/System/Cisco/Cisco ASA|
|Parser|/Parsers/System/Cisco/Cisco Firepower JSON|
|Parser|/Parsers/System/Cisco/Cisco Firepower Syslog|
|Parser|/Parsers/System/Cisco/Cisco IOS|
|Parser|/Parsers/System/Cisco/Cisco ISE|
|Parser|/Parsers/System/Cisco/Cisco Ironport|
|Parser|/Parsers/System/Cisco/Cisco Meraki|
|Parser|/Parsers/System/Cisco/Cisco Meraki C2C|
|Parser|/Parsers/System/Cisco/Cisco Secure Email|
|Parser|/Parsers/System/Cisco/Cisco Umbrella CSV|
|Parser|/Parsers/System/Cisco/Cisco Umbrella JSON|
|Parser|/Parsers/System/Citrix/Citrix Cloud C2C|
|Parser|/Parsers/System/Citrix/Citrix NetScaler Syslog|
|Parser|/Parsers/System/Claroty/Claroty xDome CEF|
|Parser|/Parsers/System/Cloudflare/Cloudflare Logpush|
|Parser|/Parsers/System/Code42/Code42|
|Parser|/Parsers/System/Code42/Code42 Incydr|
|Parser|/Parsers/System/CommScope/CommScope|
|Parser|/Parsers/System/CommScope/CommScope Ruckus SmartZone|
|Parser|/Parsers/System/Contrast Security/Contrast ADR|
|Parser|/Parsers/System/Corelight/Corelight NSM|
|Parser|/Parsers/System/CrowdStrike/CrowdStrike FDR - JSON|
|Parser|/Parsers/System/CrowdStrike/CrowdStrike Falcon Endpoint - CEF|
|Parser|/Parsers/System/CrowdStrike/CrowdStrike Falcon Endpoint - JSON|
|Parser|/Parsers/System/CrowdStrike/CrowdStrike Filevantage|
|Parser|/Parsers/System/CrowdStrike/CrowdStrike Spotlight|
|Parser|/Parsers/System/Cyber-Ark/Cyber-Ark Vault - CEF|
|Parser|/Parsers/System/Cyber-Ark/CyberArk Audit|
|Parser|/Parsers/System/Cyber-Ark/CyberArk EPM JSON|
|Parser|/Parsers/System/Cylance/Cylance Syslog|
|Parser|/Parsers/System/Cylance/Cylance Threat JSON|
|Parser|/Parsers/System/Darktrace/Darktrace JSON|
|Parser|/Parsers/System/Darktrace/Darktrace Syslog|
|Parser|/Parsers/System/Dataminr/Dataminr|
|Parser|/Parsers/System/Dell/Dell SonicWall|
|Parser|/Parsers/System/Digital Guardian/Digital Guardian ARC|
|Parser|/Parsers/System/Docker/Docker JSON|
|Parser|/Parsers/System/DocuSign/DocuSign Monitor|
|Parser|/Parsers/System/Dragos/Dragos|
|Parser|/Parsers/System/Druva/Druva Cyber Resilience|
|Parser|/Parsers/System/Druva/Druva inSync Cloud|
|Parser|/Parsers/System/Duo Security/Duo Multi-Factor Authentication|
|Parser|/Parsers/System/ESET/ESET|
|Parser|/Parsers/System/Egnyte/Egnyte DLP|
|Parser|/Parsers/System/Exabeam/Exabeam Security Management Platform (SMP) Syslog|
|Parser|/Parsers/System/Extrahop/Extrahop CEF|
|Parser|/Parsers/System/Extrahop/Extrahop JSON|
|Parser|/Parsers/System/F5/F5 Syslog|
|Parser|/Parsers/System/Falco/Falco JSON|
|Parser|/Parsers/System/FireEye/FireEye CMS CEF|
|Parser|/Parsers/System/FireEye/FireEye Web MPS JSON|
|Parser|/Parsers/System/Forescout/Forescout CounterACT|
|Parser|/Parsers/System/Fortinet/Fortigate/Fortigate-CEF|
|Parser|/Parsers/System/Fortinet/Fortigate/Fortigate-JSON|
|Parser|/Parsers/System/Fortinet/Fortigate/Fortigate-Syslog|
|Parser|/Parsers/System/Genetec/Genetec Synergis|
|Parser|/Parsers/System/Gigamon/GigamonTI|
|Parser|/Parsers/System/Github/GitHub Enterprise Audit|
|Parser|/Parsers/System/Github/Github|
|Parser|/Parsers/System/Google/G Suite Alert Center|
|Parser|/Parsers/System/Google/G Suite Audit|
|Parser|/Parsers/System/Google/GCP|
|Parser|/Parsers/System/Google/GCP BigQuery Gmail|
|Parser|/Parsers/System/Google/Security Command Center|
|Parser|/Parsers/System/HP/Aruba ClearPass - Syslog|
|Parser|/Parsers/System/HP/Aruba WAP|
|Parser|/Parsers/System/Honeywell/Honeywell Pro-Watch|
|Parser|/Parsers/System/ISC/ISC BIND|
|Parser|/Parsers/System/Imperva/Imperva Incapsula|
|Parser|/Parsers/System/Infoblox/Infoblox|
|Parser|/Parsers/System/JFrog/JFrog Artifactory|
|Parser|/Parsers/System/Jamf/Jamf|
|Parser|/Parsers/System/JumpCloud/JumpCloud Directory Insights|
|Parser|/Parsers/System/JumpCloud/JumpCloud IdP|
|Parser|/Parsers/System/Juniper/Juniper SRX Series Firewall Syslog|
|Parser|/Parsers/System/Juniper/Juniper SSG Series Firewall Syslog|
|Parser|/Parsers/System/Kaltura/Kaltura|
|Parser|/Parsers/System/Kandji/Kandji EDR|
|Parser|/Parsers/System/Kaspersky/Kaspersky Endpoint Security|
|Parser|/Parsers/System/Keeper/Keeper|
|Parser|/Parsers/System/Kemp/Kemp LoadMaster Syslog|
|Parser|/Parsers/System/KnowBe4/KnowBe4 KMSAT C2C|
|Parser|/Parsers/System/Kubernetes/Kubernetes|
|Parser|/Parsers/System/Lacework/Lacework JSON|
|Parser|/Parsers/System/LastPass/LastPass|
|Parser|/Parsers/System/Laurel/Laurel Linux Audit|
|Parser|/Parsers/System/Libraesva/Libraesva Email Security|
|Parser|/Parsers/System/Linux/Linux OS Syslog|
|Parser|/Parsers/System/Linux/Linux Sysmon XML|
|Parser|/Parsers/System/Linux/Shared/Linux Shared Syslog Headers|
|Parser|/Parsers/System/ManageEngine/ADAuditPlus Syslog|
|Parser|/Parsers/System/McAfee/McAfee CEF|
|Parser|/Parsers/System/McAfee/McAfee EPO XML|
|Parser|/Parsers/System/McAfee/McAfee LEEF|
|Parser|/Parsers/System/McAfee/McAfee Mvision ENS|
|Parser|/Parsers/System/McAfee/McAfee Network Security|
|Parser|/Parsers/System/McAfee/McAfee Web Gateway CSV|
|Parser|/Parsers/System/McAfee/Shared/Syslog Headers McAfee|
|Parser|/Parsers/System/Microsoft/Azure Storage Analytics|
|Parser|/Parsers/System/Microsoft/Azure Virtual Network|
|Parser|/Parsers/System/Microsoft/Exchange|
|Parser|/Parsers/System/Microsoft/Graph Security Alert API|
|Parser|/Parsers/System/Microsoft/Microsoft Azure JSON|
|Parser|/Parsers/System/Microsoft/Microsoft Azure Nested JSON|
|Parser|/Parsers/System/Microsoft/Microsoft Defender Advanced Hunting|
|Parser|/Parsers/System/Microsoft/Microsoft IIS|
|Parser|/Parsers/System/Microsoft/Microsoft SQL Server|
|Parser|/Parsers/System/Microsoft/O365 Exchange Message Trace C2C|
|Parser|/Parsers/System/Microsoft/Office 365|
|Parser|/Parsers/System/Microsoft/Shared/Syslog Headers Microsoft|
|Parser|/Parsers/System/Microsoft/Shared/Windows Field Renames|
|Parser|/Parsers/System/Microsoft/Shared/Windows Forwarding Headers|
|Parser|/Parsers/System/Microsoft/Shared/Windows Text Transforms - Security|
|Parser|/Parsers/System/Microsoft/Sysmon-JSON|
|Parser|/Parsers/System/Microsoft/Windows DNS|
|Parser|/Parsers/System/Microsoft/Windows Defender ATP Alert JSON|
|Parser|/Parsers/System/Microsoft/Windows Defender SCCM DB CSV|
|Parser|/Parsers/System/Microsoft/Windows Firewall Syslog|
|Parser|/Parsers/System/Microsoft/Windows PowerShell-JSON|
|Parser|/Parsers/System/Microsoft/Windows PowerShell-Syslog|
|Parser|/Parsers/System/Microsoft/Windows XML from Azure|
|Parser|/Parsers/System/Microsoft/Windows-JSON|
|Parser|/Parsers/System/Microsoft/Windows-JSON-Open Telemetry|
|Parser|/Parsers/System/Microsoft/Windows-NXLog|
|Parser|/Parsers/System/Microsoft/Windows-Syslog|
|Parser|/Parsers/System/Microsoft/Windows-Syslog Multiline|
|Parser|/Parsers/System/Microsoft/Windows-Syslog Snare|
|Parser|/Parsers/System/Microsoft/Windows-Syslog Tenable LCE|
|Parser|/Parsers/System/Microsoft/Windows-Syslog WinCollect|
|Parser|/Parsers/System/Microsoft/Windows-XML|
|Parser|/Parsers/System/Mimecast/Mimecast|
|Parser|/Parsers/System/Mindpoint Group/Mindpoint Group Keeper|
|Parser|/Parsers/System/Miro/Miro Audit C2C|
|Parser|/Parsers/System/Netskope/Netskope Security Cloud JSON|
|Parser|/Parsers/System/Nginx/Nginx Syslog|
|Parser|/Parsers/System/OCSF/OCSF|
|Parser|/Parsers/System/OSSEC/OSSEC JSON|
|Parser|/Parsers/System/Okta/Okta|
|Parser|/Parsers/System/OneLogin/OneLogin SSO JSON|
|Parser|/Parsers/System/OpenVPN/OpenVPN Syslog|
|Parser|/Parsers/System/Oracle/Oracle Cloud Infrastructure|
|Parser|/Parsers/System/Orca Security/Orca Security|
|Parser|/Parsers/System/Osquery/Osquery JSON|
|Parser|/Parsers/System/Palo Alto/PAN Firewall CEF|
|Parser|/Parsers/System/Palo Alto/PAN Firewall CSV|
|Parser|/Parsers/System/Palo Alto/PAN Firewall LEEF|
|Parser|/Parsers/System/Palo Alto/PAN Prisma Cloud JSON|
|Parser|/Parsers/System/Parser Templates/CEF Template|
|Parser|/Parsers/System/Parser Templates/CEF Template Commented|
|Parser|/Parsers/System/Parser Templates/CSV Template|
|Parser|/Parsers/System/Parser Templates/CSV Template Commented|
|Parser|/Parsers/System/Parser Templates/JSON Template|
|Parser|/Parsers/System/Parser Templates/JSON Template Commented|
|Parser|/Parsers/System/Parser Templates/Key Value Pair Template|
|Parser|/Parsers/System/Parser Templates/Key Value Pair Template Commented|
|Parser|/Parsers/System/Parser Templates/LEEF Template|
|Parser|/Parsers/System/Parser Templates/LEEF Template Commented|
|Parser|/Parsers/System/Parser Templates/Unstructured Template|
|Parser|/Parsers/System/Parser Templates/Unstructured Template Commented|
|Parser|/Parsers/System/Parser Templates/Windows XML Template|
|Parser|/Parsers/System/Parser Templates/Windows XML Template Commented|
|Parser|/Parsers/System/Parser Templates/XML Template|
|Parser|/Parsers/System/Parser Templates/XML Template Commented|
|Parser|/Parsers/System/Pfsense/Pfsense Firewall|
|Parser|/Parsers/System/PingIdentity/PingFederate|
|Parser|/Parsers/System/Pulse Secure/Pulse Secure Appliance|
|Parser|/Parsers/System/Qualys/Qualys Vulnerability Data|
|Parser|/Parsers/System/Qumulo/Qumulo Core|
|Parser|/Parsers/System/RSA/RSA SecurID Runtime CSV|
|Parser|/Parsers/System/RSA/RSA SecurID SinglePoint|
|Parser|/Parsers/System/Radiant Logic/Radiant Logic VDS|
|Parser|/Parsers/System/Salesforce/Salesforce|
|Parser|/Parsers/System/SentinelOne/SentinelOne CEF|
|Parser|/Parsers/System/SentinelOne/SentinelOne MGMT API|
|Parser|/Parsers/System/SentinelOne/SentinelOne Syslog|
|Parser|/Parsers/System/Shared/Formatter|
|Parser|/Parsers/System/Shared/Process CEF Fields|
|Parser|/Parsers/System/Shared/Syslog Headers|
|Parser|/Parsers/System/Signal Science/Signal Science WAF|
|Parser|/Parsers/System/Slack/Slack Enterprise Audit|
|Parser|/Parsers/System/Snort/Snort|
|Parser|/Parsers/System/Snowflake/Snowflake|
|Parser|/Parsers/System/Sophos/Sophos Central C2C JSON|
|Parser|/Parsers/System/Sophos/Sophos UTM|
|Parser|/Parsers/System/Squid/Squid Proxy Syslog|
|Parser|/Parsers/System/Sucuri/Sucuri WAF|
|Parser|/Parsers/System/SurePass/SurePass|
|Parser|/Parsers/System/Suricata/Suricata Syslog|
|Parser|/Parsers/System/Symantec/Data Loss Prevention/Symantec DLP|
|Parser|/Parsers/System/Symantec/Symantec Endpoint Protection/Symantec Endpoint Protection-Syslog|
|Parser|/Parsers/System/Symantec/Symantec Endpoint Security|
|Parser|/Parsers/System/Sysdig/Sysdig JSON|
|Parser|/Parsers/System/Sysdig/Sysdig Secure|
|Parser|/Parsers/System/Tanium/Tanium CEF|
|Parser|/Parsers/System/Tanium/Tanium JSON|
|Parser|/Parsers/System/Tanium/Tanium Syslog|
|Parser|/Parsers/System/Teramind/Teramind Teraserver|
|Parser|/Parsers/System/Thinkst Canary/Thinkst Canary|
|Parser|/Parsers/System/Thinkst Canary/Thinkst Canary JSON|
|Parser|/Parsers/System/TippingPoint/TippingPoint TPS Cloud|
|Parser|/Parsers/System/Trellix/Trellix MVision EPO|
|Parser|/Parsers/System/Trend Micro/Trend Micro Deep Security - CEF|
|Parser|/Parsers/System/Trend Micro/Trend Micro Vision One|
|Parser|/Parsers/System/Trust Login/Trust Login|
|Parser|/Parsers/System/Twistlock/Twistlock|
|Parser|/Parsers/System/VMware/Carbon Black Cloud|
|Parser|/Parsers/System/VMware/VMware Avi Load Balancer|
|Parser|/Parsers/System/VMware/VMware ESXi|
|Parser|/Parsers/System/VMware/VMware NSX|
|Parser|/Parsers/System/Varonis/Varonis DatAlert Syslog|
|Parser|/Parsers/System/Vectra/Vectra AI|
|Parser|/Parsers/System/WatchGuard/WatchGuard Fireware|
|Parser|/Parsers/System/Wiz/Wiz|
|Parser|/Parsers/System/Workday/Workday|
|Parser|/Parsers/System/Zeek/Zeek|
|Parser|/Parsers/System/Zendesk/Zendesk|
|Parser|/Parsers/System/Zero Networks/Zero Networks Segment|
|Parser|/Parsers/System/Zoom/Zoom|
|Parser|/Parsers/System/Zscaler/Zscaler Nanolog Streaming Service/Zscaler Nanolog Streaming Service-CEF|
|Parser|/Parsers/System/Zscaler/Zscaler Nanolog Streaming Service/Zscaler Nanolog Streaming Service-JSON|
|Parser|/Parsers/System/Zscaler/Zscaler Nanolog Streaming Service/Zscaler Nanolog Streaming Service-LEEF|
|Parser|/Parsers/System/Zscaler/Zscaler Next Generation Firewall/Firewall-JSON|
|Parser|/Parsers/System/Zscaler/Zscaler Next Generation Firewall/Firewall-Syslog|
|Parser|/Parsers/System/Zscaler/Zscaler Private Access/Zscaler Private Access-JSON|
|Parser|/Parsers/System/Zscaler/Zscaler Workload Segmentation/Zscaler Workload Segmentation JSON|
