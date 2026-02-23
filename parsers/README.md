# Parsers (aka Custom Parsers)

The `type` listed lets you know if you can directly apply the parser to a collector to parse messages from CIP or if it is used as a dependency to assist other parsers with the `[dependencies]` stanza.

|Type|Parser Path|
|----|-----------|
|Parser|[/Parsers/System/1Password/1Password](Parsers~System~1Password~1Password.md)|
|Parser|[/Parsers/System/1PasswordC2C/1PasswordC2C](Parsers~System~1PasswordC2C~1PasswordC2C.md)|
|Parser|[/Parsers/System/AWS/AWS ALB](Parsers~System~AWS~AWS_ALB.md)|
|Parser|[/Parsers/System/AWS/AWS CloudFront](Parsers~System~AWS~AWS_CloudFront.md)|
|Parser|[/Parsers/System/AWS/AWS CloudWatch](Parsers~System~AWS~AWS_CloudWatch.md)|
|Parser|[/Parsers/System/AWS/AWS Config](Parsers~System~AWS~AWS_Config.md)|
|Parser|[/Parsers/System/AWS/AWS EKS](Parsers~System~AWS~AWS_EKS.md)|
|Parser|[/Parsers/System/AWS/AWS ELB](Parsers~System~AWS~AWS_ELB.md)|
|Parser|[/Parsers/System/AWS/AWS Inspector](Parsers~System~AWS~AWS_Inspector.md)|
|Parser|[/Parsers/System/AWS/AWS Network Firewall](Parsers~System~AWS~AWS_Network_Firewall.md)|
|Parser|[/Parsers/System/AWS/AWS Redshift](Parsers~System~AWS~AWS_Redshift.md)|
|Parser|[/Parsers/System/AWS/AWS Route 53](Parsers~System~AWS~AWS_Route_53.md)|
|Parser|[/Parsers/System/AWS/AWS S3 Server Access Logs](Parsers~System~AWS~AWS_S3_Server_Access_Logs.md)|
|Parser|[/Parsers/System/AWS/AWS Security Hub](Parsers~System~AWS~AWS_Security_Hub.md)|
|Parser|[/Parsers/System/AWS/AWS VPC Flow](Parsers~System~AWS~AWS_VPC_Flow.md)|
|Parser|[/Parsers/System/AWS/AWS VPC Transit Gateways Flow Logs](Parsers~System~AWS~AWS_VPC_Transit_Gateways_Flow_Logs.md)|
|Parser|[/Parsers/System/AWS/AWS VPN](Parsers~System~AWS~AWS_VPN.md)|
|Parser|[/Parsers/System/AWS/AWS WAF](Parsers~System~AWS~AWS_WAF.md)|
|Parser|[/Parsers/System/AWS/CloudTrail](Parsers~System~AWS~CloudTrail.md)|
|Parser|[/Parsers/System/AWS/GuardDuty](Parsers~System~AWS~GuardDuty.md)|
|Parser|[/Parsers/System/Abnormal Security/Abnormal Security](Parsers~System~Abnormal_Security~Abnormal_Security.md)|
|Parser|[/Parsers/System/Adaxes/Adaxes Syslog](Parsers~System~Adaxes~Adaxes_Syslog.md)|
|Parser|[/Parsers/System/Airtable/Airtable Audit C2C](Parsers~System~Airtable~Airtable_Audit_C2C.md)|
|Parser|[/Parsers/System/Akamai/Akamai CPC](Parsers~System~Akamai~Akamai_CPC.md)|
|Parser|[/Parsers/System/Akamai/Noname API Security](Parsers~System~Akamai~Noname_API_Security.md)|
|Parser|[/Parsers/System/Alert Logic/Alert Logic](Parsers~System~Alert_Logic~Alert_Logic.md)|
|Parser|[/Parsers/System/Anthropic/Claude Code](Parsers~System~Anthropic~Claude_Code.md)|
|Parser|[/Parsers/System/Apache/Apache HTTP Server](Parsers~System~Apache~Apache_HTTP_Server.md)|
|Parser|[/Parsers/System/Aqua/Aqua JSON](Parsers~System~Aqua~Aqua_JSON.md)|
|Parser|[/Parsers/System/Asana/Asana Audit](Parsers~System~Asana~Asana_Audit.md)|
|Parser|[/Parsers/System/Atlassian/Atlassian Audit Events](Parsers~System~Atlassian~Atlassian_Audit_Events.md)|
|Parser|[/Parsers/System/Atlassian/Atlassian Confluence Access Logs](Parsers~System~Atlassian~Atlassian_Confluence_Access_Logs.md)|
|Parser|[/Parsers/System/Atlassian/Atlassian Jira](Parsers~System~Atlassian~Atlassian_Jira.md)|
|Parser|[/Parsers/System/Auth0/Auth0](Parsers~System~Auth0~Auth0.md)|
|Parser|[/Parsers/System/Automox/Automox](Parsers~System~Automox~Automox.md)|
|Parser|[/Parsers/System/Bandura/Bandura Syslog](Parsers~System~Bandura~Bandura_Syslog.md)|
|Parser|[/Parsers/System/Barracuda/Barracuda CloudGen](Parsers~System~Barracuda~Barracuda_CloudGen.md)|
|Parser|[/Parsers/System/Barracuda/Barracuda WAF](Parsers~System~Barracuda~Barracuda_WAF.md)|
|Parser|[/Parsers/System/Bitwarden/Bitwarden](Parsers~System~Bitwarden~Bitwarden.md)|
|Parser|[/Parsers/System/Blue Coat/Blue Coat ProxySG](Parsers~System~Blue_Coat~Blue_Coat_ProxySG.md)|
|Parser|[/Parsers/System/Blue Coat/Blue Coat ProxySG CEF](Parsers~System~Blue_Coat~Blue_Coat_ProxySG_CEF.md)|
|Parser|[/Parsers/System/Blue Coat/Blue Coat ProxySG CSV](Parsers~System~Blue_Coat~Blue_Coat_ProxySG_CSV.md)|
|Parser|[/Parsers/System/BlueCat/BlueCat DHCP-DNS Syslog](Parsers~System~BlueCat~BlueCat_DHCP-DNS_Syslog.md)|
|Parser|[/Parsers/System/Cato Networks/Cato Networks](Parsers~System~Cato_Networks~Cato_Networks.md)|
|Parser|[/Parsers/System/Check Point/Check Point Avanan JSON](Parsers~System~Check_Point~Check_Point_Avanan_JSON.md)|
|Parser|[/Parsers/System/Check Point/Check Point Firewall JSON](Parsers~System~Check_Point~Check_Point_Firewall_JSON.md)|
|Parser|[/Parsers/System/Check Point/Check Point Firewall Syslog](Parsers~System~Check_Point~Check_Point_Firewall_Syslog.md)|
|Parser|[/Parsers/System/Cisco/Cisco ASA](Parsers~System~Cisco~Cisco_ASA.md)|
|Parser|[/Parsers/System/Cisco/Cisco Firepower JSON](Parsers~System~Cisco~Cisco_Firepower_JSON.md)|
|Parser|[/Parsers/System/Cisco/Cisco Firepower Syslog](Parsers~System~Cisco~Cisco_Firepower_Syslog.md)|
|Parser|[/Parsers/System/Cisco/Cisco IOS](Parsers~System~Cisco~Cisco_IOS.md)|
|Parser|[/Parsers/System/Cisco/Cisco ISE](Parsers~System~Cisco~Cisco_ISE.md)|
|Parser|[/Parsers/System/Cisco/Cisco Ironport](Parsers~System~Cisco~Cisco_Ironport.md)|
|Parser|[/Parsers/System/Cisco/Cisco Meraki](Parsers~System~Cisco~Cisco_Meraki.md)|
|Parser|[/Parsers/System/Cisco/Cisco Meraki C2C](Parsers~System~Cisco~Cisco_Meraki_C2C.md)|
|Parser|[/Parsers/System/Cisco/Cisco Secure Email](Parsers~System~Cisco~Cisco_Secure_Email.md)|
|Parser|[/Parsers/System/Cisco/Cisco Umbrella CSV](Parsers~System~Cisco~Cisco_Umbrella_CSV.md)|
|Parser|[/Parsers/System/Cisco/Cisco Umbrella JSON](Parsers~System~Cisco~Cisco_Umbrella_JSON.md)|
|Parser|[/Parsers/System/Citrix/Citrix Cloud C2C](Parsers~System~Citrix~Citrix_Cloud_C2C.md)|
|Parser|[/Parsers/System/Citrix/Citrix NetScaler Syslog](Parsers~System~Citrix~Citrix_NetScaler_Syslog.md)|
|Parser|[/Parsers/System/Claroty/Claroty xDome CEF](Parsers~System~Claroty~Claroty_xDome_CEF.md)|
|Parser|[/Parsers/System/Cloudflare/Cloudflare Logpush](Parsers~System~Cloudflare~Cloudflare_Logpush.md)|
|Parser|[/Parsers/System/Code42/Code42](Parsers~System~Code42~Code42.md)|
|Parser|[/Parsers/System/Code42/Code42 Incydr](Parsers~System~Code42~Code42_Incydr.md)|
|Parser|[/Parsers/System/CommScope/CommScope](Parsers~System~CommScope~CommScope.md)|
|Parser|[/Parsers/System/CommScope/CommScope Ruckus SmartZone](Parsers~System~CommScope~CommScope_Ruckus_SmartZone.md)|
|Parser|[/Parsers/System/Contrast Security/Contrast ADR](Parsers~System~Contrast_Security~Contrast_ADR.md)|
|Parser|[/Parsers/System/Corelight/Corelight NSM](Parsers~System~Corelight~Corelight_NSM.md)|
|Parser|[/Parsers/System/CrowdStrike/CrowdStrike FDR - JSON](Parsers~System~CrowdStrike~CrowdStrike_FDR_-_JSON.md)|
|Parser|[/Parsers/System/CrowdStrike/CrowdStrike Falcon Endpoint - CEF](Parsers~System~CrowdStrike~CrowdStrike_Falcon_Endpoint_-_CEF.md)|
|Parser|[/Parsers/System/CrowdStrike/CrowdStrike Falcon Endpoint - JSON](Parsers~System~CrowdStrike~CrowdStrike_Falcon_Endpoint_-_JSON.md)|
|Parser|[/Parsers/System/CrowdStrike/CrowdStrike Filevantage](Parsers~System~CrowdStrike~CrowdStrike_Filevantage.md)|
|Parser|[/Parsers/System/CrowdStrike/CrowdStrike Spotlight](Parsers~System~CrowdStrike~CrowdStrike_Spotlight.md)|
|Parser|[/Parsers/System/Cyber-Ark/Cyber-Ark Vault - CEF](Parsers~System~Cyber-Ark~Cyber-Ark_Vault_-_CEF.md)|
|Parser|[/Parsers/System/Cyber-Ark/CyberArk Audit](Parsers~System~Cyber-Ark~CyberArk_Audit.md)|
|Parser|[/Parsers/System/Cyber-Ark/CyberArk EPM JSON](Parsers~System~Cyber-Ark~CyberArk_EPM_JSON.md)|
|Parser|[/Parsers/System/Cylance/Cylance Syslog](Parsers~System~Cylance~Cylance_Syslog.md)|
|Parser|[/Parsers/System/Cylance/Cylance Threat JSON](Parsers~System~Cylance~Cylance_Threat_JSON.md)|
|Parser|[/Parsers/System/Darktrace/Darktrace JSON](Parsers~System~Darktrace~Darktrace_JSON.md)|
|Parser|[/Parsers/System/Darktrace/Darktrace Syslog](Parsers~System~Darktrace~Darktrace_Syslog.md)|
|Parser|[/Parsers/System/Databricks/Databricks Audit](Parsers~System~Databricks~Databricks_Audit.md)|
|Parser|[/Parsers/System/Dataminr/Dataminr](Parsers~System~Dataminr~Dataminr.md)|
|Parser|[/Parsers/System/Dell/Dell SonicWall](Parsers~System~Dell~Dell_SonicWall.md)|
|Parser|[/Parsers/System/Digital Guardian/Digital Guardian ARC](Parsers~System~Digital_Guardian~Digital_Guardian_ARC.md)|
|Parser|[/Parsers/System/Docker/Docker JSON](Parsers~System~Docker~Docker_JSON.md)|
|Parser|[/Parsers/System/DocuSign/DocuSign Monitor](Parsers~System~DocuSign~DocuSign_Monitor.md)|
|Parser|[/Parsers/System/Dragos/Dragos](Parsers~System~Dragos~Dragos.md)|
|Parser|[/Parsers/System/Druva/Druva Cyber Resilience](Parsers~System~Druva~Druva_Cyber_Resilience.md)|
|Parser|[/Parsers/System/Druva/Druva inSync Cloud](Parsers~System~Druva~Druva_inSync_Cloud.md)|
|Parser|[/Parsers/System/Duo Security/Duo Multi-Factor Authentication](Parsers~System~Duo_Security~Duo_Multi-Factor_Authentication.md)|
|Parser|[/Parsers/System/ESET/ESET](Parsers~System~ESET~ESET.md)|
|Parser|[/Parsers/System/Egnyte/Egnyte DLP](Parsers~System~Egnyte~Egnyte_DLP.md)|
|Parser|[/Parsers/System/Exabeam/Exabeam Security Management Platform (SMP) Syslog](Parsers~System~Exabeam~Exabeam_Security_Management_Platform_(SMP)_Syslog.md)|
|Parser|[/Parsers/System/Extrahop/Extrahop CEF](Parsers~System~Extrahop~Extrahop_CEF.md)|
|Parser|[/Parsers/System/Extrahop/Extrahop JSON](Parsers~System~Extrahop~Extrahop_JSON.md)|
|Parser|[/Parsers/System/F5/F5 Syslog](Parsers~System~F5~F5_Syslog.md)|
|Parser|[/Parsers/System/Falco/Falco JSON](Parsers~System~Falco~Falco_JSON.md)|
|Parser|[/Parsers/System/FireEye/FireEye CMS CEF](Parsers~System~FireEye~FireEye_CMS_CEF.md)|
|Parser|[/Parsers/System/FireEye/FireEye Web MPS JSON](Parsers~System~FireEye~FireEye_Web_MPS_JSON.md)|
|Parser|[/Parsers/System/Forescout/Forescout CounterACT](Parsers~System~Forescout~Forescout_CounterACT.md)|
|Parser|[/Parsers/System/Fortinet/Fortigate/Fortigate-CEF](Parsers~System~Fortinet~Fortigate~Fortigate-CEF.md)|
|Parser|[/Parsers/System/Fortinet/Fortigate/Fortigate-JSON](Parsers~System~Fortinet~Fortigate~Fortigate-JSON.md)|
|Parser|[/Parsers/System/Fortinet/Fortigate/Fortigate-Syslog](Parsers~System~Fortinet~Fortigate~Fortigate-Syslog.md)|
|Parser|[/Parsers/System/Genetec/Genetec Synergis](Parsers~System~Genetec~Genetec_Synergis.md)|
|Parser|[/Parsers/System/Gigamon/GigamonTI](Parsers~System~Gigamon~GigamonTI.md)|
|Parser|[/Parsers/System/Github/GitHub Enterprise Audit](Parsers~System~Github~GitHub_Enterprise_Audit.md)|
|Parser|[/Parsers/System/Github/Github](Parsers~System~Github~Github.md)|
|Parser|[/Parsers/System/Google/G Suite Alert Center](Parsers~System~Google~G_Suite_Alert_Center.md)|
|Parser|[/Parsers/System/Google/G Suite Audit](Parsers~System~Google~G_Suite_Audit.md)|
|Parser|[/Parsers/System/Google/GCP](Parsers~System~Google~GCP.md)|
|Parser|[/Parsers/System/Google/GCP BigQuery Gmail](Parsers~System~Google~GCP_BigQuery_Gmail.md)|
|Parser|[/Parsers/System/Google/Google Workspace Alert Center](Parsers~System~Google~Google_Workspace_Alert_Center.md)|
|Parser|[/Parsers/System/Google/Google Workspace Audit](Parsers~System~Google~Google_Workspace_Audit.md)|
|Parser|[/Parsers/System/Google/Security Command Center](Parsers~System~Google~Security_Command_Center.md)|
|Parser|[/Parsers/System/HP/Aruba ClearPass - Syslog](Parsers~System~HP~Aruba_ClearPass_-_Syslog.md)|
|Parser|[/Parsers/System/HP/Aruba WAP](Parsers~System~HP~Aruba_WAP.md)|
|Parser|[/Parsers/System/Honeywell/Honeywell Pro-Watch](Parsers~System~Honeywell~Honeywell_Pro-Watch.md)|
|Parser|[/Parsers/System/ISC/ISC BIND](Parsers~System~ISC~ISC_BIND.md)|
|Parser|[/Parsers/System/Imperva/Imperva Incapsula](Parsers~System~Imperva~Imperva_Incapsula.md)|
|Parser|[/Parsers/System/Infoblox/Infoblox](Parsers~System~Infoblox~Infoblox.md)|
|Parser|[/Parsers/System/JFrog/JFrog Artifactory](Parsers~System~JFrog~JFrog_Artifactory.md)|
|Parser|[/Parsers/System/Jamf/Jamf](Parsers~System~Jamf~Jamf.md)|
|Parser|[/Parsers/System/JumpCloud/JumpCloud Directory Insights](Parsers~System~JumpCloud~JumpCloud_Directory_Insights.md)|
|Parser|[/Parsers/System/JumpCloud/JumpCloud IdP](Parsers~System~JumpCloud~JumpCloud_IdP.md)|
|Parser|[/Parsers/System/Juniper/Juniper SRX Series Firewall Syslog](Parsers~System~Juniper~Juniper_SRX_Series_Firewall_Syslog.md)|
|Parser|[/Parsers/System/Juniper/Juniper SSG Series Firewall Syslog](Parsers~System~Juniper~Juniper_SSG_Series_Firewall_Syslog.md)|
|Parser|[/Parsers/System/Kaltura/Kaltura](Parsers~System~Kaltura~Kaltura.md)|
|Parser|[/Parsers/System/Kandji/Kandji EDR](Parsers~System~Kandji~Kandji_EDR.md)|
|Parser|[/Parsers/System/Kaspersky/Kaspersky Endpoint Security](Parsers~System~Kaspersky~Kaspersky_Endpoint_Security.md)|
|Dependency|[/Parsers/System/Keeper/Keeper](Parsers~System~Keeper~Keeper.md)|
|Parser|[/Parsers/System/Kemp/Kemp LoadMaster Syslog](Parsers~System~Kemp~Kemp_LoadMaster_Syslog.md)|
|Parser|[/Parsers/System/KnowBe4/KnowBe4 KMSAT C2C](Parsers~System~KnowBe4~KnowBe4_KMSAT_C2C.md)|
|Parser|[/Parsers/System/Kubernetes/Kubernetes](Parsers~System~Kubernetes~Kubernetes.md)|
|Parser|[/Parsers/System/Lacework/Lacework JSON](Parsers~System~Lacework~Lacework_JSON.md)|
|Parser|[/Parsers/System/LastPass/LastPass](Parsers~System~LastPass~LastPass.md)|
|Parser|[/Parsers/System/Laurel/Laurel Linux Audit](Parsers~System~Laurel~Laurel_Linux_Audit.md)|
|Parser|[/Parsers/System/Libraesva/Libraesva Email Security](Parsers~System~Libraesva~Libraesva_Email_Security.md)|
|Parser|[/Parsers/System/Linux/Linux OS Syslog](Parsers~System~Linux~Linux_OS_Syslog.md)|
|Parser|[/Parsers/System/Linux/Linux Sysmon XML](Parsers~System~Linux~Linux_Sysmon_XML.md)|
|Dependency|[/Parsers/System/Linux/Shared/Linux Shared Syslog Headers](Parsers~System~Linux~Shared~Linux_Shared_Syslog_Headers.md)|
|Parser|[/Parsers/System/ManageEngine/ADAuditPlus Syslog](Parsers~System~ManageEngine~ADAuditPlus_Syslog.md)|
|Parser|[/Parsers/System/McAfee/McAfee CEF](Parsers~System~McAfee~McAfee_CEF.md)|
|Parser|[/Parsers/System/McAfee/McAfee EPO XML](Parsers~System~McAfee~McAfee_EPO_XML.md)|
|Parser|[/Parsers/System/McAfee/McAfee LEEF](Parsers~System~McAfee~McAfee_LEEF.md)|
|Parser|[/Parsers/System/McAfee/McAfee Mvision ENS](Parsers~System~McAfee~McAfee_Mvision_ENS.md)|
|Parser|[/Parsers/System/McAfee/McAfee Network Security](Parsers~System~McAfee~McAfee_Network_Security.md)|
|Parser|[/Parsers/System/McAfee/McAfee Web Gateway CSV](Parsers~System~McAfee~McAfee_Web_Gateway_CSV.md)|
|Dependency|[/Parsers/System/McAfee/Shared/Syslog Headers McAfee](Parsers~System~McAfee~Shared~Syslog_Headers_McAfee.md)|
|Parser|[/Parsers/System/Microsoft/Azure Storage Analytics](Parsers~System~Microsoft~Azure_Storage_Analytics.md)|
|Parser|[/Parsers/System/Microsoft/Azure Virtual Network](Parsers~System~Microsoft~Azure_Virtual_Network.md)|
|Parser|[/Parsers/System/Microsoft/Exchange](Parsers~System~Microsoft~Exchange.md)|
|Parser|[/Parsers/System/Microsoft/Graph Security Alert API](Parsers~System~Microsoft~Graph_Security_Alert_API.md)|
|Parser|[/Parsers/System/Microsoft/Microsoft Azure JSON](Parsers~System~Microsoft~Microsoft_Azure_JSON.md)|
|Parser|[/Parsers/System/Microsoft/Microsoft Azure Nested JSON](Parsers~System~Microsoft~Microsoft_Azure_Nested_JSON.md)|
|Parser|[/Parsers/System/Microsoft/Microsoft Defender Advanced Hunting](Parsers~System~Microsoft~Microsoft_Defender_Advanced_Hunting.md)|
|Parser|[/Parsers/System/Microsoft/Microsoft IIS](Parsers~System~Microsoft~Microsoft_IIS.md)|
|Parser|[/Parsers/System/Microsoft/Microsoft SQL Server](Parsers~System~Microsoft~Microsoft_SQL_Server.md)|
|Parser|[/Parsers/System/Microsoft/O365 Exchange Message Trace C2C](Parsers~System~Microsoft~O365_Exchange_Message_Trace_C2C.md)|
|Parser|[/Parsers/System/Microsoft/Office 365](Parsers~System~Microsoft~Office_365.md)|
|Dependency|[/Parsers/System/Microsoft/Shared/Syslog Headers Microsoft](Parsers~System~Microsoft~Shared~Syslog_Headers_Microsoft.md)|
|Dependency|[/Parsers/System/Microsoft/Shared/Windows Field Renames](Parsers~System~Microsoft~Shared~Windows_Field_Renames.md)|
|Dependency|[/Parsers/System/Microsoft/Shared/Windows Forwarding Headers](Parsers~System~Microsoft~Shared~Windows_Forwarding_Headers.md)|
|Dependency|[/Parsers/System/Microsoft/Shared/Windows Text Transforms - Security](Parsers~System~Microsoft~Shared~Windows_Text_Transforms_-_Security.md)|
|Parser|[/Parsers/System/Microsoft/Sysmon-JSON](Parsers~System~Microsoft~Sysmon-JSON.md)|
|Parser|[/Parsers/System/Microsoft/Windows DNS](Parsers~System~Microsoft~Windows_DNS.md)|
|Parser|[/Parsers/System/Microsoft/Windows Defender ATP Alert JSON](Parsers~System~Microsoft~Windows_Defender_ATP_Alert_JSON.md)|
|Parser|[/Parsers/System/Microsoft/Windows Defender SCCM DB CSV](Parsers~System~Microsoft~Windows_Defender_SCCM_DB_CSV.md)|
|Parser|[/Parsers/System/Microsoft/Windows Firewall Syslog](Parsers~System~Microsoft~Windows_Firewall_Syslog.md)|
|Parser|[/Parsers/System/Microsoft/Windows PowerShell-JSON](Parsers~System~Microsoft~Windows_PowerShell-JSON.md)|
|Parser|[/Parsers/System/Microsoft/Windows PowerShell-Syslog](Parsers~System~Microsoft~Windows_PowerShell-Syslog.md)|
|Parser|[/Parsers/System/Microsoft/Windows XML from Azure](Parsers~System~Microsoft~Windows_XML_from_Azure.md)|
|Parser|[/Parsers/System/Microsoft/Windows-JSON](Parsers~System~Microsoft~Windows-JSON.md)|
|Parser|[/Parsers/System/Microsoft/Windows-JSON-Open Telemetry](Parsers~System~Microsoft~Windows-JSON-Open_Telemetry.md)|
|Parser|[/Parsers/System/Microsoft/Windows-NXLog](Parsers~System~Microsoft~Windows-NXLog.md)|
|Parser|[/Parsers/System/Microsoft/Windows-Syslog](Parsers~System~Microsoft~Windows-Syslog.md)|
|Parser|[/Parsers/System/Microsoft/Windows-Syslog Multiline](Parsers~System~Microsoft~Windows-Syslog_Multiline.md)|
|Parser|[/Parsers/System/Microsoft/Windows-Syslog Snare](Parsers~System~Microsoft~Windows-Syslog_Snare.md)|
|Parser|[/Parsers/System/Microsoft/Windows-Syslog Tenable LCE](Parsers~System~Microsoft~Windows-Syslog_Tenable_LCE.md)|
|Parser|[/Parsers/System/Microsoft/Windows-Syslog WinCollect](Parsers~System~Microsoft~Windows-Syslog_WinCollect.md)|
|Parser|[/Parsers/System/Microsoft/Windows-XML](Parsers~System~Microsoft~Windows-XML.md)|
|Parser|[/Parsers/System/Mimecast/Mimecast](Parsers~System~Mimecast~Mimecast.md)|
|Parser|[/Parsers/System/Mindpoint Group/Mindpoint Group Keeper](Parsers~System~Mindpoint_Group~Mindpoint_Group_Keeper.md)|
|Parser|[/Parsers/System/Miro/Miro Audit C2C](Parsers~System~Miro~Miro_Audit_C2C.md)|
|Parser|[/Parsers/System/Netskope/Netskope Security Cloud JSON](Parsers~System~Netskope~Netskope_Security_Cloud_JSON.md)|
|Parser|[/Parsers/System/Netskope/Netskope WebTx](Parsers~System~Netskope~Netskope_WebTx.md)|
|Parser|[/Parsers/System/Nginx/Nginx Syslog](Parsers~System~Nginx~Nginx_Syslog.md)|
|Parser|[/Parsers/System/OCSF/OCSF](Parsers~System~OCSF~OCSF.md)|
|Parser|[/Parsers/System/OSSEC/OSSEC JSON](Parsers~System~OSSEC~OSSEC_JSON.md)|
|Parser|[/Parsers/System/Okta/Okta](Parsers~System~Okta~Okta.md)|
|Parser|[/Parsers/System/OneLogin/OneLogin SSO JSON](Parsers~System~OneLogin~OneLogin_SSO_JSON.md)|
|Parser|[/Parsers/System/OpenAI/OpenAI Audit](Parsers~System~OpenAI~OpenAI_Audit.md)|
|Parser|[/Parsers/System/OpenVPN/OpenVPN Syslog](Parsers~System~OpenVPN~OpenVPN_Syslog.md)|
|Parser|[/Parsers/System/Oracle/Oracle Cloud Infrastructure](Parsers~System~Oracle~Oracle_Cloud_Infrastructure.md)|
|Parser|[/Parsers/System/Orca Security/Orca Security](Parsers~System~Orca_Security~Orca_Security.md)|
|Parser|[/Parsers/System/Osquery/Osquery JSON](Parsers~System~Osquery~Osquery_JSON.md)|
|Parser|[/Parsers/System/Palo Alto/PAN Firewall CEF](Parsers~System~Palo_Alto~PAN_Firewall_CEF.md)|
|Parser|[/Parsers/System/Palo Alto/PAN Firewall CSV](Parsers~System~Palo_Alto~PAN_Firewall_CSV.md)|
|Parser|[/Parsers/System/Palo Alto/PAN Firewall LEEF](Parsers~System~Palo_Alto~PAN_Firewall_LEEF.md)|
|Parser|[/Parsers/System/Palo Alto/PAN Prisma Cloud JSON](Parsers~System~Palo_Alto~PAN_Prisma_Cloud_JSON.md)|
|Parser|[/Parsers/System/Parser Templates/CEF Template](Parsers~System~Parser_Templates~CEF_Template.md)|
|Parser|[/Parsers/System/Parser Templates/CEF Template Commented](Parsers~System~Parser_Templates~CEF_Template_Commented.md)|
|Parser|[/Parsers/System/Parser Templates/CSV Template](Parsers~System~Parser_Templates~CSV_Template.md)|
|Parser|[/Parsers/System/Parser Templates/CSV Template Commented](Parsers~System~Parser_Templates~CSV_Template_Commented.md)|
|Parser|[/Parsers/System/Parser Templates/JSON Template](Parsers~System~Parser_Templates~JSON_Template.md)|
|Parser|[/Parsers/System/Parser Templates/JSON Template Commented](Parsers~System~Parser_Templates~JSON_Template_Commented.md)|
|Parser|[/Parsers/System/Parser Templates/Key Value Pair Template](Parsers~System~Parser_Templates~Key_Value_Pair_Template.md)|
|Parser|[/Parsers/System/Parser Templates/Key Value Pair Template Commented](Parsers~System~Parser_Templates~Key_Value_Pair_Template_Commented.md)|
|Parser|[/Parsers/System/Parser Templates/LEEF Template](Parsers~System~Parser_Templates~LEEF_Template.md)|
|Parser|[/Parsers/System/Parser Templates/LEEF Template Commented](Parsers~System~Parser_Templates~LEEF_Template_Commented.md)|
|Parser|[/Parsers/System/Parser Templates/Unstructured Template](Parsers~System~Parser_Templates~Unstructured_Template.md)|
|Parser|[/Parsers/System/Parser Templates/Unstructured Template Commented](Parsers~System~Parser_Templates~Unstructured_Template_Commented.md)|
|Parser|[/Parsers/System/Parser Templates/Windows XML Template](Parsers~System~Parser_Templates~Windows_XML_Template.md)|
|Parser|[/Parsers/System/Parser Templates/Windows XML Template Commented](Parsers~System~Parser_Templates~Windows_XML_Template_Commented.md)|
|Parser|[/Parsers/System/Parser Templates/XML Template](Parsers~System~Parser_Templates~XML_Template.md)|
|Parser|[/Parsers/System/Parser Templates/XML Template Commented](Parsers~System~Parser_Templates~XML_Template_Commented.md)|
|Parser|[/Parsers/System/Pfsense/Pfsense Firewall](Parsers~System~Pfsense~Pfsense_Firewall.md)|
|Parser|[/Parsers/System/PingIdentity/PingFederate](Parsers~System~PingIdentity~PingFederate.md)|
|Parser|[/Parsers/System/PingIdentity/PingIdentity MFA](Parsers~System~PingIdentity~PingIdentity_MFA.md)|
|Parser|[/Parsers/System/Pulse Secure/Pulse Secure Appliance](Parsers~System~Pulse_Secure~Pulse_Secure_Appliance.md)|
|Parser|[/Parsers/System/Qualys/Qualys Vulnerability Data](Parsers~System~Qualys~Qualys_Vulnerability_Data.md)|
|Parser|[/Parsers/System/Qumulo/Qumulo Core](Parsers~System~Qumulo~Qumulo_Core.md)|
|Parser|[/Parsers/System/RSA/RSA SecurID Runtime CSV](Parsers~System~RSA~RSA_SecurID_Runtime_CSV.md)|
|Parser|[/Parsers/System/RSA/RSA SecurID SinglePoint](Parsers~System~RSA~RSA_SecurID_SinglePoint.md)|
|Parser|[/Parsers/System/Radiant Logic/Radiant Logic VDS](Parsers~System~Radiant_Logic~Radiant_Logic_VDS.md)|
|Parser|[/Parsers/System/Salesforce/Salesforce](Parsers~System~Salesforce~Salesforce.md)|
|Parser|[/Parsers/System/SentinelOne/SentinelOne CEF](Parsers~System~SentinelOne~SentinelOne_CEF.md)|
|Parser|[/Parsers/System/SentinelOne/SentinelOne MGMT API](Parsers~System~SentinelOne~SentinelOne_MGMT_API.md)|
|Parser|[/Parsers/System/SentinelOne/SentinelOne Syslog](Parsers~System~SentinelOne~SentinelOne_Syslog.md)|
|Dependency|[/Parsers/System/Shared/Formatter](Parsers~System~Shared~Formatter.md)|
|Dependency|[/Parsers/System/Shared/Process CEF Fields](Parsers~System~Shared~Process_CEF_Fields.md)|
|Dependency|[/Parsers/System/Shared/Syslog Headers](Parsers~System~Shared~Syslog_Headers.md)|
|Parser|[/Parsers/System/Signal Science/Signal Science WAF](Parsers~System~Signal_Science~Signal_Science_WAF.md)|
|Parser|[/Parsers/System/Slack/Slack Enterprise Audit](Parsers~System~Slack~Slack_Enterprise_Audit.md)|
|Parser|[/Parsers/System/Snort/Snort](Parsers~System~Snort~Snort.md)|
|Parser|[/Parsers/System/Snowflake/Snowflake](Parsers~System~Snowflake~Snowflake.md)|
|Parser|[/Parsers/System/SonicWall/SonicWall Firewall](Parsers~System~SonicWall~SonicWall_Firewall.md)|
|Parser|[/Parsers/System/Sophos/Sophos Central C2C JSON](Parsers~System~Sophos~Sophos_Central_C2C_JSON.md)|
|Parser|[/Parsers/System/Sophos/Sophos UTM](Parsers~System~Sophos~Sophos_UTM.md)|
|Parser|[/Parsers/System/Squid/Squid Proxy Syslog](Parsers~System~Squid~Squid_Proxy_Syslog.md)|
|Parser|[/Parsers/System/Sucuri/Sucuri WAF](Parsers~System~Sucuri~Sucuri_WAF.md)|
|Parser|[/Parsers/System/SurePass/SurePass](Parsers~System~SurePass~SurePass.md)|
|Parser|[/Parsers/System/Suricata/Suricata Syslog](Parsers~System~Suricata~Suricata_Syslog.md)|
|Parser|[/Parsers/System/Symantec/Data Loss Prevention/Symantec DLP](Parsers~System~Symantec~Data_Loss_Prevention~Symantec_DLP.md)|
|Parser|[/Parsers/System/Symantec/Symantec Endpoint Protection/Symantec Endpoint Protection-Syslog](Parsers~System~Symantec~Symantec_Endpoint_Protection~Symantec_Endpoint_Protection-Syslog.md)|
|Parser|[/Parsers/System/Symantec/Symantec Endpoint Security](Parsers~System~Symantec~Symantec_Endpoint_Security.md)|
|Parser|[/Parsers/System/Sysdig/Sysdig JSON](Parsers~System~Sysdig~Sysdig_JSON.md)|
|Parser|[/Parsers/System/Sysdig/Sysdig Secure](Parsers~System~Sysdig~Sysdig_Secure.md)|
|Parser|[/Parsers/System/Tanium/Tanium CEF](Parsers~System~Tanium~Tanium_CEF.md)|
|Parser|[/Parsers/System/Tanium/Tanium JSON](Parsers~System~Tanium~Tanium_JSON.md)|
|Parser|[/Parsers/System/Tanium/Tanium Syslog](Parsers~System~Tanium~Tanium_Syslog.md)|
|Parser|[/Parsers/System/Teramind/Teramind Teraserver](Parsers~System~Teramind~Teramind_Teraserver.md)|
|Parser|[/Parsers/System/Thinkst Canary/Thinkst Canary](Parsers~System~Thinkst_Canary~Thinkst_Canary.md)|
|Parser|[/Parsers/System/Thinkst Canary/Thinkst Canary JSON](Parsers~System~Thinkst_Canary~Thinkst_Canary_JSON.md)|
|Parser|[/Parsers/System/TippingPoint/TippingPoint TPS Cloud](Parsers~System~TippingPoint~TippingPoint_TPS_Cloud.md)|
|Parser|[/Parsers/System/Trellix/Trellix MVision EPO](Parsers~System~Trellix~Trellix_MVision_EPO.md)|
|Parser|[/Parsers/System/Trend Micro/Trend Micro Deep Security - CEF](Parsers~System~Trend_Micro~Trend_Micro_Deep_Security_-_CEF.md)|
|Parser|[/Parsers/System/Trend Micro/Trend Micro Vision One](Parsers~System~Trend_Micro~Trend_Micro_Vision_One.md)|
|Parser|[/Parsers/System/Trust Login/Trust Login](Parsers~System~Trust_Login~Trust_Login.md)|
|Parser|[/Parsers/System/Twistlock/Twistlock](Parsers~System~Twistlock~Twistlock.md)|
|Parser|[/Parsers/System/Ubiquiti/Ubiquiti Unifi](Parsers~System~Ubiquiti~Ubiquiti_Unifi.md)|
|Parser|[/Parsers/System/VMware/Carbon Black Cloud](Parsers~System~VMware~Carbon_Black_Cloud.md)|
|Parser|[/Parsers/System/VMware/VMware Avi Load Balancer](Parsers~System~VMware~VMware_Avi_Load_Balancer.md)|
|Parser|[/Parsers/System/VMware/VMware ESXi](Parsers~System~VMware~VMware_ESXi.md)|
|Parser|[/Parsers/System/VMware/VMware NSX](Parsers~System~VMware~VMware_NSX.md)|
|Parser|[/Parsers/System/VMware/vSphere Web Services](Parsers~System~VMware~vSphere_Web_Services.md)|
|Parser|[/Parsers/System/Varonis/Varonis Alert JSON](Parsers~System~Varonis~Varonis_Alert_JSON.md)|
|Parser|[/Parsers/System/Varonis/Varonis DatAlert Syslog](Parsers~System~Varonis~Varonis_DatAlert_Syslog.md)|
|Parser|[/Parsers/System/Vectra/Vectra AI](Parsers~System~Vectra~Vectra_AI.md)|
|Parser|[/Parsers/System/WatchGuard/WatchGuard Fireware](Parsers~System~WatchGuard~WatchGuard_Fireware.md)|
|Parser|[/Parsers/System/Wiz/Wiz](Parsers~System~Wiz~Wiz.md)|
|Parser|[/Parsers/System/Workday/Workday](Parsers~System~Workday~Workday.md)|
|Parser|[/Parsers/System/Zeek/Zeek](Parsers~System~Zeek~Zeek.md)|
|Parser|[/Parsers/System/Zendesk/Zendesk](Parsers~System~Zendesk~Zendesk.md)|
|Parser|[/Parsers/System/Zero Networks/Zero Networks Segment](Parsers~System~Zero_Networks~Zero_Networks_Segment.md)|
|Parser|[/Parsers/System/Zoom/Zoom](Parsers~System~Zoom~Zoom.md)|
|Parser|[/Parsers/System/Zscaler/Zscaler Nanolog Streaming Service/Zscaler Nanolog Streaming Service-CEF](Parsers~System~Zscaler~Zscaler_Nanolog_Streaming_Service~Zscaler_Nanolog_Streaming_Service-CEF.md)|
|Parser|[/Parsers/System/Zscaler/Zscaler Nanolog Streaming Service/Zscaler Nanolog Streaming Service-JSON](Parsers~System~Zscaler~Zscaler_Nanolog_Streaming_Service~Zscaler_Nanolog_Streaming_Service-JSON.md)|
|Parser|[/Parsers/System/Zscaler/Zscaler Nanolog Streaming Service/Zscaler Nanolog Streaming Service-LEEF](Parsers~System~Zscaler~Zscaler_Nanolog_Streaming_Service~Zscaler_Nanolog_Streaming_Service-LEEF.md)|
|Parser|[/Parsers/System/Zscaler/Zscaler Next Generation Firewall/Firewall-JSON](Parsers~System~Zscaler~Zscaler_Next_Generation_Firewall~Firewall-JSON.md)|
|Parser|[/Parsers/System/Zscaler/Zscaler Next Generation Firewall/Firewall-Syslog](Parsers~System~Zscaler~Zscaler_Next_Generation_Firewall~Firewall-Syslog.md)|
|Parser|[/Parsers/System/Zscaler/Zscaler Private Access/Zscaler Private Access-JSON](Parsers~System~Zscaler~Zscaler_Private_Access~Zscaler_Private_Access-JSON.md)|
|Parser|[/Parsers/System/Zscaler/Zscaler Workload Segmentation/Zscaler Workload Segmentation JSON](Parsers~System~Zscaler~Zscaler_Workload_Segmentation~Zscaler_Workload_Segmentation_JSON.md)|
