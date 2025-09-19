# Rules

## Useful CSVs

|File|Description|
|----|-----------|
|[rules.csv](rules.csv)|The entire rule set in a CSV|
|[threat_rules.csv](threat_rules.csv)|Each [normalized threat rule](https://help.sumologic.com/docs/cse/rules/normalized-threat-rules/) and its associated mappings using the `threat_ruleType` schema field.|
|[auth_rules.csv](auth_rules.csv)|Each [normalized authentication rule](https://help.sumologic.com/docs/cse/rules/normalized-authentication-rules/) and its associated mappings using the `normalizedAction` schema field.|

## All Rules

|Rule ID|Name|
|----|----|
|MATCH-S00574|[.NET Framework Remote Code Execution Vulnerability](MATCH-S00574.md)|
|MATCH-S00458|[ADPassHunt Tool](MATCH-S00458.md)|
|MATCH-S00307|[AWS - Excessive OAuth Application Permissions Scope](MATCH-S00307.md)|
|MATCH-S00306|[AWS - New UserPoolClient Created](MATCH-S00306.md)|
|MATCH-S00922|[AWS Bedrock Agent Created](MATCH-S00922.md)|
|MATCH-S00924|[AWS Bedrock Guardrail Deleted](MATCH-S00924.md)|
|MATCH-S00923|[AWS Bedrock Model Invocation Denied for User](MATCH-S00923.md)|
|MATCH-S00921|[AWS Bedrock Model Invocation Logging Configuration Change Observed](MATCH-S00921.md)|
|MATCH-S00715|[AWS Cloud Storage Deletion](MATCH-S00715.md)|
|AGGREGATION-S00002|[AWS CloudTrail - Aggressive Reconnaissance](AGGREGATION-S00002.md)|
|LEGACY-S00207|[AWS CloudTrail - Customer Master Key Disabled or Scheduled for Deletion](LEGACY-S00207.md)|
|MATCH-S00261|[AWS CloudTrail - Database Snapshot Created](MATCH-S00261.md)|
|MATCH-S00208|[AWS CloudTrail - EC2 Access Key Action Detected](MATCH-S00208.md)|
|MATCH-S00246|[AWS CloudTrail - GetSecretValue from non Amazon IP](MATCH-S00246.md)|
|MATCH-S00111|[AWS CloudTrail - IAM CreateUser Action Observed](MATCH-S00111.md)|
|LEGACY-S00206|[AWS CloudTrail - IAM Policy Applied](LEGACY-S00206.md)|
|MATCH-S00101|[AWS CloudTrail - IAM Privileged Policy Applied to Group](MATCH-S00101.md)|
|MATCH-S00102|[AWS CloudTrail - IAM Privileged Policy Applied to Group (Username)](MATCH-S00102.md)|
|MATCH-S00104|[AWS CloudTrail - IAM Privileged Policy Applied to Role](MATCH-S00104.md)|
|MATCH-S00099|[AWS CloudTrail - IAM Privileged Policy Applied to User](MATCH-S00099.md)|
|THRESHOLD-S00051|[AWS CloudTrail - IAM User Generating AccessDenied Errors Across Multiple Actions](THRESHOLD-S00051.md)|
|MATCH-S00113|[AWS CloudTrail - Logging Configuration Change Observed](MATCH-S00113.md)|
|MATCH-S00308|[AWS CloudTrail - OpsWorks Describe Permissions Event](MATCH-S00308.md)|
|MATCH-S00109|[AWS CloudTrail - Permissions Boundary Lifted](MATCH-S00109.md)|
|MATCH-S00105|[AWS CloudTrail - Public S3 Bucket Exposed](MATCH-S00105.md)|
|MATCH-S00213|[AWS CloudTrail - Reconnaissance related event](MATCH-S00213.md)|
|MATCH-S00096|[AWS CloudTrail - Root Console Successful Login Observed](MATCH-S00096.md)|
|MATCH-S00764|[AWS CloudTrail - S3 Bucket Public Access Block Disabled](MATCH-S00764.md)|
|MATCH-S00210|[AWS CloudTrail - SQS List Queues Event](MATCH-S00210.md)|
|MATCH-S00240|[AWS CloudTrail - ScheduleKeyDeletion in KMS](MATCH-S00240.md)|
|MATCH-S00247|[AWS CloudTrail - Secrets Manager sensitive admin action observed](MATCH-S00247.md)|
|MATCH-S00238|[AWS CloudTrail - sensitive activity in KMS](MATCH-S00238.md)|
|MATCH-S00540|[AWS CloudTrail Network Access Control List Deleted](MATCH-S00540.md)|
|MATCH-S00664|[AWS CloudWatch Alarm Actions Disabled](MATCH-S00664.md)|
|MATCH-S00663|[AWS CloudWatch Alarm Deletion](MATCH-S00663.md)|
|MATCH-S00662|[AWS CloudWatch Anomaly Detector Deletion](MATCH-S00662.md)|
|MATCH-S00665|[AWS CloudWatch Log Group Deletion](MATCH-S00665.md)|
|MATCH-S00661|[AWS CloudWatch Log Stream Deletion](MATCH-S00661.md)|
|MATCH-S00671|[AWS Config Recorder Deletion](MATCH-S00671.md)|
|MATCH-S00672|[AWS Config Recorder Stopped](MATCH-S00672.md)|
|MATCH-S00670|[AWS Config Service Tampering](MATCH-S00670.md)|
|OUTLIER-S00024|[AWS DynamoDB Outlier in GetItem Events from User](OUTLIER-S00024.md)|
|OUTLIER-S00033|[AWS DynamoDB Outlier in PutItem Events from User](OUTLIER-S00033.md)|
|MATCH-S00654|[AWS ECS Cluster Deleted](MATCH-S00654.md)|
|MATCH-S00873|[AWS EKS Cluster Configuration Updated](MATCH-S00873.md)|
|MATCH-S00872|[AWS EKS Failed Curl Authentication Attempt](MATCH-S00872.md)|
|MATCH-S00871|[AWS EKS Pod Shared Object Modification or Creation](MATCH-S00871.md)|
|MATCH-S00870|[AWS EKS Secrets Created](MATCH-S00870.md)|
|MATCH-S00869|[AWS EKS Secrets Deleted](MATCH-S00869.md)|
|MATCH-S00716|[AWS Image Creation](MATCH-S00716.md)|
|MATCH-S00717|[AWS Image Deletion](MATCH-S00717.md)|
|THRESHOLD-S00106|[AWS Image Discovery](THRESHOLD-S00106.md)|
|MATCH-S00718|[AWS Image Modification](MATCH-S00718.md)|
|MATCH-S00719|[AWS Instance Creation](MATCH-S00719.md)|
|MATCH-S00720|[AWS Instance Deletion](MATCH-S00720.md)|
|THRESHOLD-S00107|[AWS Instance Discovery](THRESHOLD-S00107.md)|
|MATCH-S00721|[AWS Instance Modification](MATCH-S00721.md)|
|MATCH-S00874|[AWS Lambda Function Recon](MATCH-S00874.md)|
|MATCH-S00679|[AWS Route 53 Domain Registered](MATCH-S00679.md)|
|THRESHOLD-S00093|[AWS Route 53 Reconnaissance](THRESHOLD-S00093.md)|
|MATCH-S00677|[AWS Route 53 Service Tampering](MATCH-S00677.md)|
|MATCH-S00680|[AWS Route 53 TestDNSAnswer](MATCH-S00680.md)|
|MATCH-S00678|[AWS Route 53 Traffic Policy Creation](MATCH-S00678.md)|
|OUTLIER-S00025|[AWS S3 Outlier in PutObject Denied Events](OUTLIER-S00025.md)|
|MATCH-S00825|[AWS Secrets Manager Enumeration](MATCH-S00825.md)|
|MATCH-S00875|[AWS VPC FLow Log Deletion](MATCH-S00875.md)|
|MATCH-S00674|[AWS WAF Access Control List Updated](MATCH-S00674.md)|
|THRESHOLD-S00092|[AWS WAF Reconnaissance](THRESHOLD-S00092.md)|
|MATCH-S00676|[AWS WAF Rule Group Updated](MATCH-S00676.md)|
|MATCH-S00675|[AWS WAF Rule Updated](MATCH-S00675.md)|
|MATCH-S00673|[AWS WAF Service Tampering](MATCH-S00673.md)|
|MATCH-S00814|[Abnormal Child Process - sdiagnhost.exe - CVE-2022-30190](MATCH-S00814.md)|
|MATCH-S00139|[Abnormal Parent-Child Process Combination](MATCH-S00139.md)|
|MATCH-S00511|[Accessibility Executables Replaced](MATCH-S00511.md)|
|THRESHOLD-S00062|[Active Directory Domain Enumeration](THRESHOLD-S00062.md)|
|LEGACY-S00067|[Administrator Login via RDP](LEGACY-S00067.md)|
|MATCH-S00600|[Alibaba ActionTrail Access Key Action Detected](MATCH-S00600.md)|
|MATCH-S00601|[Alibaba ActionTrail IAM CreateUser Observed](MATCH-S00601.md)|
|MATCH-S00594|[Alibaba ActionTrail KMS Activity](MATCH-S00594.md)|
|MATCH-S00597|[Alibaba ActionTrail Key Deleted or Disabled](MATCH-S00597.md)|
|MATCH-S00593|[Alibaba ActionTrail ListQueues](MATCH-S00593.md)|
|MATCH-S00598|[Alibaba ActionTrail Logging Configuration Change Observed](MATCH-S00598.md)|
|MATCH-S00589|[Alibaba ActionTrail Network Access Control List Deleted](MATCH-S00589.md)|
|MATCH-S00599|[Alibaba ActionTrail Root Login](MATCH-S00599.md)|
|MATCH-S00596|[Alibaba ActionTrail Secrets Manager Activity](MATCH-S00596.md)|
|THRESHOLD-S00608|[Alibaba ActionTrail Unauthorized API Calls](THRESHOLD-S00608.md)|
|MATCH-S00553|[Allowed Inbound RDP Traffic](MATCH-S00553.md)|
|THRESHOLD-S00003|[Amazon VPC - Network Scan](THRESHOLD-S00003.md)|
|THRESHOLD-S00004|[Amazon VPC - Port Scan](THRESHOLD-S00004.md)|
|MATCH-S00660|[Anomalous AWS User Executed a Command on ECS Container](MATCH-S00660.md)|
|MATCH-S00516|[Antivirus Ransomware Detection](MATCH-S00516.md)|
|MATCH-S00510|[Attempt to Add Certificate to Store](MATCH-S00510.md)|
|MATCH-S00415|[Attempt to Clear Windows Event Logs Using Wevtutil](MATCH-S00415.md)|
|MATCH-S00390|[Attempted Credential Dump From Registry Via Reg.Exe](MATCH-S00390.md)|
|MATCH-S00417|[Attrib.exe use to Hide Files and Folders](MATCH-S00417.md)|
|MATCH-S00215|[Auth0 - High Risk Event](MATCH-S00215.md)|
|MATCH-S00685|[Authentication Without MFA](MATCH-S00685.md)|
|CHAIN-S00018|[Autorun file created after USB disk mount on host](CHAIN-S00018.md)|
|MATCH-S00564|[Azorult Malware Registry Key](MATCH-S00564.md)|
|MATCH-S00226|[Azure - Add Member to Group](MATCH-S00226.md)|
|MATCH-S00220|[Azure - Add Member to Role Outside of PIM](MATCH-S00220.md)|
|MATCH-S00798|[Azure - Anonymous Blob Access](MATCH-S00798.md)|
|MATCH-S00805|[Azure - Bastion Host Created/Modified](MATCH-S00805.md)|
|MATCH-S00806|[Azure - Bastion Host Deleted](MATCH-S00806.md)|
|MATCH-S00785|[Azure - Blob Container Deletion](MATCH-S00785.md)|
|MATCH-S00808|[Azure - Container Instance Creation/Modification](MATCH-S00808.md)|
|MATCH-S00809|[Azure - Container Start](MATCH-S00809.md)|
|MATCH-S00235|[Azure - Create User](MATCH-S00235.md)|
|MATCH-S00795|[Azure - Diagnostic Setting Deleted](MATCH-S00795.md)|
|MATCH-S00796|[Azure - Diagnostic Setting Modified](MATCH-S00796.md)|
|MATCH-S00797|[Azure - Event Hub Deleted](MATCH-S00797.md)|
|THRESHOLD-S00109|[Azure - Excessive Key Vault Get Requests](THRESHOLD-S00109.md)|
|MATCH-S00260|[Azure - External User Invitation Redeemed](MATCH-S00260.md)|
|MATCH-S00256|[Azure - External User Invited](MATCH-S00256.md)|
|MATCH-S00254|[Azure - Group Information Downloaded](MATCH-S00254.md)|
|MATCH-S00243|[Azure - High Risk Sign-In (Aggregate)](MATCH-S00243.md)|
|MATCH-S00245|[Azure - High Risk Sign-In (Real Time)](MATCH-S00245.md)|
|MATCH-S00807|[Azure - Image Created/Modified](MATCH-S00807.md)|
|MATCH-S00810|[Azure - Image Deleted](MATCH-S00810.md)|
|MATCH-S00788|[Azure - Key Deletion](MATCH-S00788.md)|
|MATCH-S00789|[Azure - Key Purged](MATCH-S00789.md)|
|MATCH-S00792|[Azure - Key Vault Deleted](MATCH-S00792.md)|
|MATCH-S00231|[Azure - Member Added to Global Administrator Role](MATCH-S00231.md)|
|MATCH-S00233|[Azure - Member Added to Global Administrator Role Non-PIM](MATCH-S00233.md)|
|MATCH-S00229|[Azure - Member Added to Non-Global Administrator Role](MATCH-S00229.md)|
|MATCH-S00140|[Azure - Policy Added](MATCH-S00140.md)|
|MATCH-S00142|[Azure - Policy Deleted](MATCH-S00142.md)|
|MATCH-S00144|[Azure - Policy Updated](MATCH-S00144.md)|
|MATCH-S00787|[Azure - Protected Item Deletion Attempt](MATCH-S00787.md)|
|MATCH-S00224|[Azure - Risky User State : User Confirmed Compromised](MATCH-S00224.md)|
|MATCH-S00786|[Azure - SQL Database Export](MATCH-S00786.md)|
|MATCH-S00794|[Azure - Secret Backup](MATCH-S00794.md)|
|MATCH-S00791|[Azure - Secret Deleted](MATCH-S00791.md)|
|MATCH-S00790|[Azure - Secret Purged](MATCH-S00790.md)|
|MATCH-S00800|[Azure - Storage Deletion](MATCH-S00800.md)|
|MATCH-S00799|[Azure - Storage Modification](MATCH-S00799.md)|
|MATCH-S00250|[Azure - Suspicious User Risk State Associated with Login](MATCH-S00250.md)|
|MATCH-S00303|[Azure - Unauthorized OAuth Application](MATCH-S00303.md)|
|MATCH-S00252|[Azure - User Information Downloaded](MATCH-S00252.md)|
|MATCH-S00803|[Azure - Virtual Machine Creation/Modification](MATCH-S00803.md)|
|MATCH-S00804|[Azure - Virtual Machine Deleted](MATCH-S00804.md)|
|MATCH-S00801|[Azure - Virtual Machine Started](MATCH-S00801.md)|
|MATCH-S00802|[Azure - Virtual Machine Stopped](MATCH-S00802.md)|
|MATCH-S00838|[Azure Active Directory Authentication Method Changed](MATCH-S00838.md)|
|MATCH-S00896|[Azure Authentication Policy Change](MATCH-S00896.md)|
|MATCH-S00836|[Azure Conditional Access Policy Disabled](MATCH-S00836.md)|
|CHAIN-S00022|[Azure DevOps - Agent Pool Created and Deleted within a Short Period](CHAIN-S00022.md)|
|MATCH-S00997|[Azure DevOps - Browser Observed in Personal Access Token (PAT) Use](MATCH-S00997.md)|
|MATCH-S00995|[Azure DevOps - Change Made to Administrator Group](MATCH-S00995.md)|
|FIRST-S00098|[Azure DevOps - First Seen Pull Request Policy Bypassed](FIRST-S00098.md)|
|FIRST-S00099|[Azure DevOps - First Seen User Creating Agent Pool](FIRST-S00099.md)|
|FIRST-S00092|[Azure DevOps - First Seen User Creating Release Pipeline](FIRST-S00092.md)|
|FIRST-S00097|[Azure DevOps - First Seen User Modifying Build Variables](FIRST-S00097.md)|
|FIRST-S00096|[Azure DevOps - First Seen User Modifying Release Pipeline](FIRST-S00096.md)|
|MATCH-S00998|[Azure DevOps - Known Malicious Tooling Detected ADOKit](MATCH-S00998.md)|
|MATCH-S00994|[Azure DevOps - Member Added to Sensitive Group](MATCH-S00994.md)|
|FIRST-S00095|[Azure DevOps - New Agent OS Added to Agent Pool](FIRST-S00095.md)|
|FIRST-S00094|[Azure DevOps - New Extension Installed](FIRST-S00094.md)|
|OUTLIER-S00030|[Azure DevOps - Outlier in Pools Deleted Rapidly](OUTLIER-S00030.md)|
|MATCH-S00996|[Azure DevOps - Personal Access Token (PAT) Misuse Observed](MATCH-S00996.md)|
|CHAIN-S00021|[Azure DevOps - Pipeline Created and Deleted within a Short Period](CHAIN-S00021.md)|
|MATCH-S00993|[Azure DevOps - Pipeline Retention Settings Reduced](MATCH-S00993.md)|
|MATCH-S00864|[Azure Firewall Rule Modified](MATCH-S00864.md)|
|MATCH-S00891|[Azure OAUTH Application Consent from User](MATCH-S00891.md)|
|MATCH-S00818|[Azure PRT Token Issued via Non Interactive Login](MATCH-S00818.md)|
|MATCH-S00839|[Azure Virtual Machine RunCommand Issued](MATCH-S00839.md)|
|MATCH-S00708|[AzureDevOps - Project Visibility Changed to Public](MATCH-S00708.md)|
|MATCH-S00486|[Backdoor.HTTP.BEACON.[CSBundle CDN GET]](MATCH-S00486.md)|
|MATCH-S00485|[Backdoor.HTTP.BEACON.[CSBundle MSOffice GET]](MATCH-S00485.md)|
|MATCH-S00484|[Backdoor.HTTP.BEACON.[CSBundle MSOffice POST]](MATCH-S00484.md)|
|MATCH-S00490|[Backdoor.HTTP.BEACON.[CSBundle NYTIMES GET]](MATCH-S00490.md)|
|MATCH-S00496|[Backdoor.HTTP.BEACON.[CSBundle NYTIMES Server]](MATCH-S00496.md)|
|MATCH-S00495|[Backdoor.HTTP.BEACON.[CSBundle Original GET]](MATCH-S00495.md)|
|MATCH-S00489|[Backdoor.HTTP.BEACON.[CSBundle Original POST]](MATCH-S00489.md)|
|MATCH-S00491|[Backdoor.HTTP.BEACON.[CSBundle Original Stager]](MATCH-S00491.md)|
|MATCH-S00488|[Backdoor.HTTP.BEACON.[CSBundle USAToday GET]](MATCH-S00488.md)|
|MATCH-S00487|[Backdoor.HTTP.BEACON.[CSBundle USAToday Server]](MATCH-S00487.md)|
|MATCH-S00474|[Backdoor.HTTP.BEACON.[Yelp GET]](MATCH-S00474.md)|
|MATCH-S00494|[Backdoor.HTTP.BEACON.[Yelp Request]](MATCH-S00494.md)|
|MATCH-S00497|[Backdoor.HTTP.GORAT.[POST]](MATCH-S00497.md)|
|MATCH-S00492|[Backdoor.HTTP.GORAT.[SID1]](MATCH-S00492.md)|
|MATCH-S00493|[Backdoor.SSL.BEACON.[CSBundle Ajax]](MATCH-S00493.md)|
|LEGACY-S00003|[Base32 in DNS Query](LEGACY-S00003.md)|
|MATCH-S00686|[Base64 Decode in Command Line](MATCH-S00686.md)|
|MATCH-S00688|[Bash History Tampering](MATCH-S00688.md)|
|MATCH-S00541|[Batch File Write To System32](MATCH-S00541.md)|
|LEGACY-S00004|[Bitsadmin to Uncommon TLD](LEGACY-S00004.md)|
|LEGACY-S00006|[Blocked Email Host](LEGACY-S00006.md)|
|LEGACY-S00007|[Blocked Email Message](LEGACY-S00007.md)|
|MATCH-S00373|[BlueMashroom DLL Load](MATCH-S00373.md)|
|LEGACY-S00009|[Bluecoat Proxy - Suspicious or Malicious Categories](LEGACY-S00009.md)|
|LEGACY-S00010|[Browser Exploitation Framework (BeEF) Hook](LEGACY-S00010.md)|
|THRESHOLD-S00096|[Brute Force Attempt](THRESHOLD-S00096.md)|
|MATCH-S00388|[COMPlus_ETWEnabled Command Line Arguments](MATCH-S00388.md)|
|MATCH-S00727|[CPL File Executed from Temp Directory](MATCH-S00727.md)|
|MATCH-S00209|[CVE-2021-44228 Log4j2 Java Library 0-Day Attempt](MATCH-S00209.md)|
|CHAIN-S00017|[Change of Azure MFA Method followed by Risky SignIn](CHAIN-S00017.md)|
|MATCH-S00821|[Chromium Browser History Access by Non-Browser Process](MATCH-S00821.md)|
|MATCH-S00897|[Chromium Extension Installed](MATCH-S00897.md)|
|MATCH-S00819|[Chromium Process Started With Debugging Port](MATCH-S00819.md)|
|MATCH-S00074|[Cisco Stealthwatch Template Alerts](MATCH-S00074.md)|
|LEGACY-S00190|[Cisco Umbrella - DNS Request Category: Adware](LEGACY-S00190.md)|
|LEGACY-S00191|[Cisco Umbrella - DNS Request Category: Command and Control](LEGACY-S00191.md)|
|LEGACY-S00192|[Cisco Umbrella - DNS Request Category: Cryptomining](LEGACY-S00192.md)|
|LEGACY-S00193|[Cisco Umbrella - DNS Request Category: DNS Tunneling VPN](LEGACY-S00193.md)|
|LEGACY-S00194|[Cisco Umbrella - DNS Request Category: Dynamic DNS](LEGACY-S00194.md)|
|LEGACY-S00195|[Cisco Umbrella - DNS Request Category: Hacking](LEGACY-S00195.md)|
|LEGACY-S00196|[Cisco Umbrella - DNS Request Category: Malware](LEGACY-S00196.md)|
|LEGACY-S00197|[Cisco Umbrella - DNS Request Category: Newly Seen Domains](LEGACY-S00197.md)|
|LEGACY-S00198|[Cisco Umbrella - DNS Request Category: P2P/File sharing](LEGACY-S00198.md)|
|LEGACY-S00199|[Cisco Umbrella - DNS Request Category: Personal VPN](LEGACY-S00199.md)|
|LEGACY-S00200|[Cisco Umbrella - DNS Request Category: Phishing](LEGACY-S00200.md)|
|LEGACY-S00201|[Cisco Umbrella - DNS Request Category: Potentially Harmful](LEGACY-S00201.md)|
|LEGACY-S00202|[Cisco Umbrella - DNS Request Category: Proxy/Anonymizer](LEGACY-S00202.md)|
|LEGACY-S00203|[Cisco Umbrella - Proxy Logs with Cisco AMP Detections](LEGACY-S00203.md)|
|MATCH-S00269|[Clipboard Copied](MATCH-S00269.md)|
|MATCH-S00820|[Cloud Credential File Accessed](MATCH-S00820.md)|
|MATCH-S00412|[Command Line Execution with Suspicious URL and AppData Strings](MATCH-S00412.md)|
|LEGACY-S00013|[Connection to High Entropy Domain](LEGACY-S00013.md)|
|MATCH-S00658|[Container Management Utility in Container](MATCH-S00658.md)|
|MATCH-S00657|[Container Running as Root](MATCH-S00657.md)|
|MATCH-S00410|[Copy from Admin Share](MATCH-S00410.md)|
|MATCH-S00758|[CrashControl Registry Modification](MATCH-S00758.md)|
|MATCH-S00443|[Create Windows Share](MATCH-S00443.md)|
|MATCH-S00591|[Cred Dump-Tools Named Pipes](MATCH-S00591.md)|
|MATCH-S00525|[Credential Dumping Via Copy Command From Shadow Copy](MATCH-S00525.md)|
|MATCH-S00526|[Credential Dumping Via Symlink To Shadow Copy](MATCH-S00526.md)|
|MATCH-S00586|[Credential Dumping by LaZagne](MATCH-S00586.md)|
|MATCH-S00513|[Critical Severity Intrusion Signature](MATCH-S00513.md)|
|LEGACY-S00189|[Crypto Miner HTTP User Agent](LEGACY-S00189.md)|
|MATCH-S00592|[Crypto Miner User Agent](MATCH-S00592.md)|
|MATCH-S00348|[Curl Start Combination](MATCH-S00348.md)|
|LEGACY-S00014|[Cylance Protect - Event Severity 1](LEGACY-S00014.md)|
|LEGACY-S00015|[Cylance Protect - Event Severity 2](LEGACY-S00015.md)|
|LEGACY-S00016|[Cylance Protect - Event Severity 3](LEGACY-S00016.md)|
|LEGACY-S00017|[Cylance Protect - Event Severity 4](LEGACY-S00017.md)|
|LEGACY-S00018|[Cylance Protect - Event Severity 5](LEGACY-S00018.md)|
|LEGACY-S00019|[Cylance Protect - Event Severity 6](LEGACY-S00019.md)|
|LEGACY-S00020|[Cylance Protect - Event Severity 7](LEGACY-S00020.md)|
|LEGACY-S00021|[Cylance Protect - Event Severity 8](LEGACY-S00021.md)|
|LEGACY-S00022|[Cylance Protect - Event Severity 9](LEGACY-S00022.md)|
|LEGACY-S00024|[DCE-RPC Service Control Call](LEGACY-S00024.md)|
|LEGACY-S00023|[DCERPC - SAMR Enumeration of All Users](LEGACY-S00023.md)|
|THRESHOLD-S00044|[DNS DGA Lookup Behavior - NXDOMAIN Responses](THRESHOLD-S00044.md)|
|LEGACY-S00026|[DNS Lookup of High Entropy Domain](LEGACY-S00026.md)|
|MATCH-S00375|[DNS RCE Exploit CVE-2020-1350](MATCH-S00375.md)|
|MATCH-S00211|[DNS.EXE Observed as Parent Process](MATCH-S00211.md)|
|MATCH-S00695|[DPAPI Key Manipulation - Backup of Backup Key](MATCH-S00695.md)|
|MATCH-S00696|[DPAPI Key Manipulation - Extracting Backup Key](MATCH-S00696.md)|
|MATCH-S00385|[DTRACK Process Creation](MATCH-S00385.md)|
|MATCH-S00441|[Delete Windows Share](MATCH-S00441.md)|
|MATCH-S00543|[Detect Psexec With Accepteula Flag](MATCH-S00543.md)|
|MATCH-S00565|[Direct Outbound DNS Traffic](MATCH-S00565.md)|
|LEGACY-S00028|[Directory Traversal - Successful](LEGACY-S00028.md)|
|THRESHOLD-S00009|[Directory Traversal - Unsuccessful](THRESHOLD-S00009.md)|
|LEGACY-S00029|[Disabled Account Logon Attempt](LEGACY-S00029.md)|
|MATCH-S00544|[Disabling Remote User Account Control](MATCH-S00544.md)|
|MATCH-S00568|[Dnscat Execution](MATCH-S00568.md)|
|AGGREGATION-S00006|[Docker Enumeration Detected on Host](AGGREGATION-S00006.md)|
|THRESHOLD-S00103|[Domain Brute Force Attempt](THRESHOLD-S00103.md)|
|THRESHOLD-S00102|[Domain Password Attack](THRESHOLD-S00102.md)|
|LEGACY-S00030|[Domain Resolution in Non-Standard TLD](LEGACY-S00030.md)|
|LEGACY-S00031|[Doublepulsar scan - likely not infected](LEGACY-S00031.md)|
|MATCH-S00319|[Dridex Process Pattern](MATCH-S00319.md)|
|MATCH-S00590|[Elise Backdoor](MATCH-S00590.md)|
|MATCH-S00527|[Email Files Written Outside Of The Outlook Directory](MATCH-S00527.md)|
|MATCH-S00572|[Emotet Process Creation](MATCH-S00572.md)|
|MATCH-S00587|[Empire PowerShell Launch Parameters](MATCH-S00587.md)|
|MATCH-S00576|[Equation Group DLL_U Load](MATCH-S00576.md)|
|MATCH-S00479|[Excavator Utility](MATCH-S00479.md)|
|THRESHOLD-S00074|[Excessive Firewall Denies](THRESHOLD-S00074.md)|
|THRESHOLD-S00085|[Excessive Outbound Firewall Blocks](THRESHOLD-S00085.md)|
|MATCH-S00682|[Excessive Use of Escape Characters in Command Line](MATCH-S00682.md)|
|LEGACY-S00033|[Executable Downloaded - Content-Type Mismatch](LEGACY-S00033.md)|
|MATCH-S00360|[Exfiltration and Tunneling Tools Execution](MATCH-S00360.md)|
|MATCH-S00827|[Exposed AWS SNS Topic Created](MATCH-S00827.md)|
|MATCH-S00823|[Exposed AWS SQS Queue Created](MATCH-S00823.md)|
|MATCH-S00304|[External Device Installation Denied](MATCH-S00304.md)|
|MATCH-S00392|[File or Folder Permissions Modifications](MATCH-S00392.md)|
|MATCH-S00394|[Findstr Launching .lnk File](MATCH-S00394.md)|
|MATCH-S00454|[Firewall Allowed SMB Traffic](MATCH-S00454.md)|
|FIRST-S00047|[First Seen ASN Associated with User for a Successful Azure AD Sign In Event](FIRST-S00047.md)|
|FIRST-S00002|[First Seen AWS API Call from User](FIRST-S00002.md)|
|FIRST-S00023|[First Seen AWS API Gateway Enumeration by User](FIRST-S00023.md)|
|FIRST-S00084|[First Seen AWS Bedrock API Call from User](FIRST-S00084.md)|
|FIRST-S00071|[First Seen AWS ConsoleLogin by User](FIRST-S00071.md)|
|FIRST-S00036|[First Seen AWS EKS API Call via CloudTrail from User](FIRST-S00036.md)|
|FIRST-S00037|[First Seen AWS EKS Admission Controller Created by IP Address](FIRST-S00037.md)|
|FIRST-S00035|[First Seen AWS EKS Secrets Enumeration from IP Address](FIRST-S00035.md)|
|FIRST-S00024|[First Seen AWS SSM RunShellScript SendCommand From User](FIRST-S00024.md)|
|FIRST-S00003|[First Seen AWS Secrets Manager API Call from User](FIRST-S00003.md)|
|LEGACY-S00036|[First Seen Access - SMB Share](LEGACY-S00036.md)|
|FIRST-S00001|[First Seen Administrative Privileges Granted for User](FIRST-S00001.md)|
|FIRST-S00026|[First Seen Anonymous Logon Change Activity to Domain Controller](FIRST-S00026.md)|
|FIRST-S00044|[First Seen AppID Generating MailItemsAccessed Event from User](FIRST-S00044.md)|
|FIRST-S00048|[First Seen Azure Device Code Authentication from User](FIRST-S00048.md)|
|FIRST-S00019|[First Seen Azure Member Addition to Group from User](FIRST-S00019.md)|
|FIRST-S00020|[First Seen Azure OAUTH Application Consent from User](FIRST-S00020.md)|
|FIRST-S00080|[First Seen Azure Portal access by User](FIRST-S00080.md)|
|FIRST-S00021|[First Seen Azure Virtual Machine Run Command Issued by User](FIRST-S00021.md)|
|FIRST-S00064|[First Seen Certificate Thumbprint in Successful Kerberos Authentication](FIRST-S00064.md)|
|FIRST-S00046|[First Seen Client Generating MailItemsAccessed Event from User](FIRST-S00046.md)|
|FIRST-S00028|[First Seen Common Windows Recon Commands From User](FIRST-S00028.md)|
|FIRST-S00013|[First Seen Driver Load - Global](FIRST-S00013.md)|
|FIRST-S00014|[First Seen Driver Load - Host](FIRST-S00014.md)|
|FIRST-S00007|[First Seen DynamoDB Enumeration from User](FIRST-S00007.md)|
|FIRST-S00073|[First Seen Get-ADDefaultDomainPasswordPolicy](FIRST-S00073.md)|
|FIRST-S00072|[First Seen Group Policy Discovery Operation](FIRST-S00072.md)|
|FIRST-S00062|[First Seen IP Address Connecting to Active Directory Certificate Services Process](FIRST-S00062.md)|
|FIRST-S00086|[First Seen IP Address Performing Trufflehog AWS Credential Verification](FIRST-S00086.md)|
|FIRST-S00027|[First Seen InstallUtil Allow List Bypass From User](FIRST-S00027.md)|
|FIRST-S00042|[First Seen Ioreg Usage from User](FIRST-S00042.md)|
|FIRST-S00017|[First Seen Kerberoasting Attempt from User - Global](FIRST-S00017.md)|
|FIRST-S00018|[First Seen Kerberoasting Attempt from User - Host](FIRST-S00018.md)|
|FIRST-S00032|[First Seen Kubectl Command From User](FIRST-S00032.md)|
|FIRST-S00004|[First Seen Local Group Addition by User](FIRST-S00004.md)|
|FIRST-S00015|[First Seen Macro Execution from User](FIRST-S00015.md)|
|FIRST-S00081|[First Seen Model ID in AWS Bedrock Put Entitlement by User](FIRST-S00081.md)|
|FIRST-S00088|[First Seen NTLM Authentication to Host (User)](FIRST-S00088.md)|
|FIRST-S00076|[First Seen Net Command Use on Host](FIRST-S00076.md)|
|FIRST-S00016|[First Seen Non-Network/Non-System Logon from User](FIRST-S00016.md)|
|FIRST-S00030|[First Seen Outbound Connection to External IP Address on Port 445 from IP Address](FIRST-S00030.md)|
|FIRST-S00010|[First Seen PowerShell Execution from Computer](FIRST-S00010.md)|
|FIRST-S00009|[First Seen RDP Logon From User](FIRST-S00009.md)|
|FIRST-S00085|[First Seen Role Creating AWS Bedrock Agent](FIRST-S00085.md)|
|FIRST-S00022|[First Seen S3 Bucket ACL Enumeration by User](FIRST-S00022.md)|
|FIRST-S00025|[First Seen SMB Allowed Traffic From IP](FIRST-S00025.md)|
|FIRST-S00034|[First Seen Session Token Granted to User from New IP](FIRST-S00034.md)|
|FIRST-S00065|[First Seen Successful Authentication From Unexpected Country](FIRST-S00065.md)|
|FIRST-S00033|[First Seen Terminal-Attached Pod Deployed to EKS](FIRST-S00033.md)|
|FIRST-S00061|[First Seen USB device in use on Windows host](FIRST-S00061.md)|
|FIRST-S00087|[First Seen User Creating or Modifying EC2 Launch Template](FIRST-S00087.md)|
|FIRST-S00005|[First Seen User Creation From User](FIRST-S00005.md)|
|FIRST-S00082|[First Seen User Enumerating AWS Bedrock Models](FIRST-S00082.md)|
|FIRST-S00100|[First Seen User Enumerating Custom AWS Bedrock Models](FIRST-S00100.md)|
|FIRST-S00006|[First Seen Weak Kerberos Encryption from User](FIRST-S00006.md)|
|FIRST-S00038|[First Seen Wget Usage from User](FIRST-S00038.md)|
|FIRST-S00040|[First Seen cURL execution from User](FIRST-S00040.md)|
|FIRST-S00074|[First Seen driverquery execution on host](FIRST-S00074.md)|
|FIRST-S00059|[First Seen esentutl command From User](FIRST-S00059.md)|
|FIRST-S00079|[First Seen gpresult execution on host](FIRST-S00079.md)|
|FIRST-S00039|[First Seen mdfind Usage from User](FIRST-S00039.md)|
|FIRST-S00041|[First Seen networksetup Usage from User](FIRST-S00041.md)|
|FIRST-S00043|[First Seen pbpaste Usage from User](FIRST-S00043.md)|
|FIRST-S00058|[First Seen vssadmin command From User](FIRST-S00058.md)|
|FIRST-S00060|[First Seen wbadmin command From User](FIRST-S00060.md)|
|FIRST-S00008|[First Seen whoami command From User](FIRST-S00008.md)|
|LEGACY-S00037|[Fortinet Critical App-Risk](LEGACY-S00037.md)|
|LEGACY-S00038|[Fortinet High App-Risk](LEGACY-S00038.md)|
|MATCH-S00117|[G Suite - Access - Access Transparency](MATCH-S00117.md)|
|MATCH-S00115|[G Suite - Admin - User Settings - Turn Off 2SV](MATCH-S00115.md)|
|MATCH-S00133|[G Suite - Admin Activity](MATCH-S00133.md)|
|MATCH-S00125|[G Suite - Drive - Drive Open To Public](MATCH-S00125.md)|
|MATCH-S00301|[G Suite - Excessive OAuth Application Permissions Scope](MATCH-S00301.md)|
|MATCH-S00128|[G Suite - Login - Account Warning](MATCH-S00128.md)|
|MATCH-S00129|[G Suite - Login - Government Attack Warning](MATCH-S00129.md)|
|MATCH-S00121|[G Suite - Mobile - Suspicious Activity](MATCH-S00121.md)|
|MATCH-S00227|[G Suite - Unauthorized OAuth Application](MATCH-S00227.md)|
|MATCH-S00120|[G Suite - User Accounts - 2SV Disabled](MATCH-S00120.md)|
|MATCH-S00620|[GCP Audit Cloud SQL Database Modified](MATCH-S00620.md)|
|MATCH-S00621|[GCP Audit GCE Firewall Rule Modified](MATCH-S00621.md)|
|MATCH-S00622|[GCP Audit GCE Network Route Created or Modified](MATCH-S00622.md)|
|MATCH-S00623|[GCP Audit GCE VPC Network Modified](MATCH-S00623.md)|
|MATCH-S00615|[GCP Audit IAM CreateServiceAccount Observed](MATCH-S00615.md)|
|MATCH-S00624|[GCP Audit IAM Custom Role Created or Modified](MATCH-S00624.md)|
|MATCH-S00631|[GCP Audit IAM Custom Role Deletion](MATCH-S00631.md)|
|MATCH-S00630|[GCP Audit IAM DeleteServiceAccount Observed](MATCH-S00630.md)|
|MATCH-S00629|[GCP Audit IAM DisableServiceAccount Observed](MATCH-S00629.md)|
|MATCH-S00614|[GCP Audit KMS Activity](MATCH-S00614.md)|
|MATCH-S00613|[GCP Audit Key Deleted or Disabled](MATCH-S00613.md)|
|MATCH-S00611|[GCP Audit ListQueues](MATCH-S00611.md)|
|MATCH-S00626|[GCP Audit Logging Sink Modified](MATCH-S00626.md)|
|MATCH-S00627|[GCP Audit Pub/Sub Subscriber Modified](MATCH-S00627.md)|
|MATCH-S00628|[GCP Audit Pub/Sub Topic Deleted](MATCH-S00628.md)|
|THRESHOLD-S00088|[GCP Audit Reconnaissance Activity](THRESHOLD-S00088.md)|
|MATCH-S00612|[GCP Audit Secrets Manager Activity](MATCH-S00612.md)|
|THRESHOLD-S00089|[GCP Audit Unauthorized API Calls](THRESHOLD-S00089.md)|
|MATCH-S00618|[GCP Bucket Enumerated](MATCH-S00618.md)|
|MATCH-S00619|[GCP Bucket Modified](MATCH-S00619.md)|
|MATCH-S00616|[GCP Bucket Open](MATCH-S00616.md)|
|MATCH-S00617|[GCP GCPloit Exploitation Framework Used](MATCH-S00617.md)|
|CHAIN-S00013|[GCP IDS Detection Followed by API Call](CHAIN-S00013.md)|
|MATCH-S00709|[GCP Image Creation](MATCH-S00709.md)|
|MATCH-S00710|[GCP Image Deletion](MATCH-S00710.md)|
|THRESHOLD-S00104|[GCP Image Discovery](THRESHOLD-S00104.md)|
|MATCH-S00711|[GCP Image Modification](MATCH-S00711.md)|
|MATCH-S00712|[GCP Instance Creation](MATCH-S00712.md)|
|MATCH-S00713|[GCP Instance Deletion](MATCH-S00713.md)|
|THRESHOLD-S00105|[GCP Instance Discovery](THRESHOLD-S00105.md)|
|MATCH-S00714|[GCP Instance Modification](MATCH-S00714.md)|
|MATCH-S00625|[GCP Permission Denied](MATCH-S00625.md)|
|THRESHOLD-S00091|[GCP Port Scan](THRESHOLD-S00091.md)|
|THRESHOLD-S00090|[GCP Port Sweep](THRESHOLD-S00090.md)|
|MATCH-S00952|[GitHub - Administrator Added or Invited](MATCH-S00952.md)|
|MATCH-S00953|[GitHub - Audit Logging Modification](MATCH-S00953.md)|
|MATCH-S00954|[GitHub - Copilot Seat Cancelled by GitHub](MATCH-S00954.md)|
|FIRST-S00091|[GitHub - First Seen Activity From Country for User](FIRST-S00091.md)|
|FIRST-S00090|[GitHub - First Seen Application Interacting with API](FIRST-S00090.md)|
|MATCH-S00950|[GitHub - Member Invitation or Addition](MATCH-S00950.md)|
|MATCH-S00955|[GitHub - Member Permissions Modification](MATCH-S00955.md)|
|MATCH-S00956|[GitHub - OAuth Application Activity](MATCH-S00956.md)|
|MATCH-S00957|[GitHub - Organization Transfer](MATCH-S00957.md)|
|OUTLIER-S00026|[GitHub - Outlier in Distinct User Agent Strings by User](OUTLIER-S00026.md)|
|OUTLIER-S00028|[GitHub - Outlier in Removal Actions by User](OUTLIER-S00028.md)|
|OUTLIER-S00027|[GitHub - Outlier in Repository Cloning or Downloads](OUTLIER-S00027.md)|
|MATCH-S00958|[GitHub - PR Review Requirement Removed](MATCH-S00958.md)|
|MATCH-S00959|[GitHub - Repository Public Key Deletion](MATCH-S00959.md)|
|MATCH-S00960|[GitHub - Repository Transfer](MATCH-S00960.md)|
|MATCH-S00961|[GitHub - Repository Visibility Changed to Public](MATCH-S00961.md)|
|MATCH-S00962|[GitHub - Repository Visibility Permissions Changed](MATCH-S00962.md)|
|MATCH-S00963|[GitHub - SSH Key Created for Private Repo](MATCH-S00963.md)|
|MATCH-S00964|[GitHub - SSO Recovery Codes Access Activity](MATCH-S00964.md)|
|MATCH-S00951|[GitHub - Secret Scanning Alert](MATCH-S00951.md)|
|MATCH-S00965|[GitHub - Secret Scanning Potentially Disabled](MATCH-S00965.md)|
|MATCH-S00966|[GitHub - Two-Factor Authentication Disabled for Organization](MATCH-S00966.md)|
|MATCH-S00949|[GitHub - Vulnerability Alerts](MATCH-S00949.md)|
|LEGACY-S00039|[GitHub Raw URL Resource Request](LEGACY-S00039.md)|
|MATCH-S00098|[Global YARA Rule](MATCH-S00098.md)|
|MATCH-S00535|[Golden SAML Indicator : Certificate Export](MATCH-S00535.md)|
|MATCH-S00414|[Grabbing Sensitive Hives via Reg Utility](MATCH-S00414.md)|
|MATCH-S00325|[Greenbug Campaign Indicators](MATCH-S00325.md)|
|MATCH-S00894|[HAR file creation observed on host](MATCH-S00894.md)|
|LEGACY-S00040|[HTTP CloudFlare Protocol Violation or Empty Response](LEGACY-S00040.md)|
|LEGACY-S00041|[HTTP External Request to PowerShell Extension](LEGACY-S00041.md)|
|LEGACY-S00042|[HTTP Request to Domain in Non-Standard TLD](LEGACY-S00042.md)|
|LEGACY-S00043|[HTTP Request with Single Header](LEGACY-S00043.md)|
|THRESHOLD-S00015|[HTTP Response Error Spike - External](THRESHOLD-S00015.md)|
|THRESHOLD-S00016|[HTTP Response Error Spike - Internal](THRESHOLD-S00016.md)|
|THRESHOLD-S00114|[HTTP Response Error Spike to AWS EKS](THRESHOLD-S00114.md)|
|LEGACY-S00044|[HTTP Shell Script Download Disguised as a Common Web File](LEGACY-S00044.md)|
|MATCH-S00203|[HTTP activity over port 53 - Possible SIGRED](MATCH-S00203.md)|
|LEGACY-S00045|[HTTP request for single character file name](LEGACY-S00045.md)|
|LEGACY-S00046|[Hexadecimal User-Agent](LEGACY-S00046.md)|
|LEGACY-S00027|[Hexadecimal in DNS Query Domain](LEGACY-S00027.md)|
|MATCH-S00666|[High Severity Intrusion Signature](MATCH-S00666.md)|
|THRESHOLD-S00078|[High Volume of DNS 'Any' Queries](THRESHOLD-S00078.md)|
|LEGACY-S00047|[High risk file extension download without hostname and referrer](LEGACY-S00047.md)|
|LEGACY-S00048|[Houdini/Iniduoh/njRAT User-Agent](LEGACY-S00048.md)|
|MATCH-S01050|[IIS - Executable File Added to Directory](MATCH-S01050.md)|
|LEGACY-S00049|[IP Address Scan - External](LEGACY-S00049.md)|
|LEGACY-S00050|[IP Address Scan - Internal](LEGACY-S00050.md)|
|MATCH-S00367|[Impacket Lateralization Detection](MATCH-S00367.md)|
|MATCH-S00482|[Impacket-Obfuscation SMBEXEC Utility](MATCH-S00482.md)|
|MATCH-S00483|[Impacket-Obfuscation WMIEXEC Utility](MATCH-S00483.md)|
|THRESHOLD-S00097|[Impossible Travel - Successful](THRESHOLD-S00097.md)|
|THRESHOLD-S00098|[Impossible Travel - Unsuccessful](THRESHOLD-S00098.md)|
|THRESHOLD-S00079|[Inbound Port Scan](THRESHOLD-S00079.md)|
|MATCH-S00669|[Informational Severity Intrusion Signature](MATCH-S00669.md)|
|MATCH-S00816|[Interactive Logon to Domain Controller](MATCH-S00816.md)|
|MATCH-S00138|[Interactive Logon with Service Account](MATCH-S00138.md)|
|LEGACY-S00053|[Internal Communication on Unassigned Low Ports - Destination Match](LEGACY-S00053.md)|
|THRESHOLD-S00080|[Internal Port Scan](THRESHOLD-S00080.md)|
|THRESHOLD-S00081|[Internal Port Sweep](THRESHOLD-S00081.md)|
|THRESHOLD-S00514|[Intrusion Scan - Targeted](THRESHOLD-S00514.md)|
|THRESHOLD-S00515|[Intrusion Sweep](THRESHOLD-S00515.md)|
|MATCH-S00322|[Judgement Panda Credential Access Activity](MATCH-S00322.md)|
|MATCH-S00334|[Judgement Panda Exfil Activity](MATCH-S00334.md)|
|MATCH-S00700|[KeePass Brute Force Tool Detection](MATCH-S00700.md)|
|MATCH-S00703|[KeeThief Detection](MATCH-S00703.md)|
|MATCH-S00364|[Kerberos Manipulation](MATCH-S00364.md)|
|MATCH-S00702|[Keychain Credential Dumping](MATCH-S00702.md)|
|MATCH-S00701|[Keychain Directory Zipped](MATCH-S00701.md)|
|MATCH-S00445|[Known Ransomware File Extensions](MATCH-S00445.md)|
|MATCH-S00653|[Kubernetes AWS Suspicious kubectl Calls](MATCH-S00653.md)|
|MATCH-S00639|[Kubernetes Anonymous Request Authorized](MATCH-S00639.md)|
|MATCH-S00651|[Kubernetes CreateCronjob](MATCH-S00651.md)|
|MATCH-S00652|[Kubernetes DeleteCronjob](MATCH-S00652.md)|
|MATCH-S00650|[Kubernetes ListCronjobs](MATCH-S00650.md)|
|MATCH-S00648|[Kubernetes ListSecrets](MATCH-S00648.md)|
|MATCH-S00640|[Kubernetes Pod Created in Kube Namespace](MATCH-S00640.md)|
|MATCH-S00641|[Kubernetes Pod Created with hostNetwork](MATCH-S00641.md)|
|MATCH-S00647|[Kubernetes Pod Deletion](MATCH-S00647.md)|
|MATCH-S00837|[Kubernetes Secrets Enumeration via Kubectl](MATCH-S00837.md)|
|MATCH-S00642|[Kubernetes Service Account Created in Kube Namespace](MATCH-S00642.md)|
|MATCH-S00649|[Kubernetes Service Account Token File Accessed](MATCH-S00649.md)|
|MATCH-S00643|[Kubernetes Service Created with NodePort](MATCH-S00643.md)|
|MATCH-S00645|[Kubernetes User Attached to a Pod](MATCH-S00645.md)|
|MATCH-S00646|[Kubernetes User Exec into a Pod](MATCH-S00646.md)|
|MATCH-S00461|[LNKSmasher Utility Commands](MATCH-S00461.md)|
|MATCH-S00340|[LSASS Memory Dump](MATCH-S00340.md)|
|MATCH-S00429|[LSASS Memory Dumping](MATCH-S00429.md)|
|MATCH-S00457|[Large File Upload](MATCH-S00457.md)|
|MATCH-S00396|[Large Outbound ICMP Packets](MATCH-S00396.md)|
|MATCH-S00844|[LastPass - Account Created](MATCH-S00844.md)|
|MATCH-S00854|[LastPass - Failed Login](MATCH-S00854.md)|
|MATCH-S00846|[LastPass - Folder Permissions Updated](MATCH-S00846.md)|
|MATCH-S00855|[LastPass - Login](MATCH-S00855.md)|
|MATCH-S00847|[LastPass - Master Password Changed](MATCH-S00847.md)|
|MATCH-S00848|[LastPass - Password Changed](MATCH-S00848.md)|
|MATCH-S00849|[LastPass - Personal Share](MATCH-S00849.md)|
|MATCH-S00850|[LastPass - Policy Added](MATCH-S00850.md)|
|MATCH-S00851|[LastPass - Policy Deleted](MATCH-S00851.md)|
|MATCH-S00852|[LastPass - Shared Folder Created](MATCH-S00852.md)|
|MATCH-S00853|[LastPass - Super Admin Password Reset](MATCH-S00853.md)|
|CHAIN-S00004|[Lateral Movement Using the Windows Hidden Admin Share](CHAIN-S00004.md)|
|LEGACY-S00054|[Likely doublepulsar Infected](LEGACY-S00054.md)|
|MATCH-S00784|[Linux Host Entered Promiscuous Mode](MATCH-S00784.md)|
|MATCH-S00687|[Linux Security Tool Usage](MATCH-S00687.md)|
|MATCH-S00746|[Loadable Kernel Module Dependency Install](MATCH-S00746.md)|
|MATCH-S00745|[Loadable Kernel Module Enumeration](MATCH-S00745.md)|
|MATCH-S00723|[Loadable Kernel Module Modifications](MATCH-S00723.md)|
|MATCH-S00505|[Local User Created](MATCH-S00505.md)|
|MATCH-S00509|[Logon with Local Credentials](MATCH-S00509.md)|
|THRESHOLD-S00099|[Long URL Containing SQL Commands](THRESHOLD-S00099.md)|
|MATCH-S00668|[Low Severity Intrusion Signature](MATCH-S00668.md)|
|MATCH-S00578|[Lsass Registry Key Modified](MATCH-S00578.md)|
|MATCH-S00573|[MS Office Memory Corruption Vulnerability Exploit](MATCH-S00573.md)|
|MATCH-S00811|[MS Office Product Spawning Msdt.exe - CVE-2022-30190](MATCH-S00811.md)|
|THRESHOLD-S00018|[MS-LSAT Username Enumeration](THRESHOLD-S00018.md)|
|MATCH-S00352|[MSHTA Suspicious Execution](MATCH-S00352.md)|
|MATCH-S00534|[MacOS - Re-Opened Applications](MATCH-S00534.md)|
|MATCH-S00729|[MacOS Gatekeeper Bypass](MATCH-S00729.md)|
|MATCH-S00731|[MacOS System Integrity Protection Disabled](MATCH-S00731.md)|
|MATCH-S00579|[Malicious Named Pipes](MATCH-S00579.md)|
|MATCH-S00161|[Malicious PowerShell Get Commands](MATCH-S00161.md)|
|MATCH-S00190|[Malicious PowerShell Invoke Commands](MATCH-S00190.md)|
|MATCH-S00198|[Malicious PowerShell Keywords](MATCH-S00198.md)|
|MATCH-S00582|[Malicious Service Installs](MATCH-S00582.md)|
|MATCH-S00519|[Malware Cleaned](MATCH-S00519.md)|
|MATCH-S00518|[Malware Not Cleaned](MATCH-S00518.md)|
|THRESHOLD-S00517|[Malware Outbreak](THRESHOLD-S00517.md)|
|MATCH-S00331|[MavInject Process Injection](MATCH-S00331.md)|
|MATCH-S00042|[McAfee Web Gateway - Poor Reputation](MATCH-S00042.md)|
|MATCH-S00638|[McAfee Web Gateway - Suspicious or Malicious Categories](MATCH-S00638.md)|
|MATCH-S00667|[Medium Severity Intrusion Signature](MATCH-S00667.md)|
|MATCH-S00355|[Meterpreter or Cobalt Strike Getsystem Service Start](MATCH-S00355.md)|
|MATCH-S00725|[Microsoft CHM File Observed](MATCH-S00725.md)|
|MATCH-S00763|[Microsoft Office Add-In Persistence](MATCH-S00763.md)|
|MATCH-S00813|[Microsoft Support Diagnostic Tool Invoking PowerShell - CVE-2022-30190](MATCH-S00813.md)|
|MATCH-S00812|[Microsoft Support Diagnostic Tool with BrowseForFile - CVE-2022-30190](MATCH-S00812.md)|
|MATCH-S00888|[Microsoft Teams External Access Enabled](MATCH-S00888.md)|
|MATCH-S00889|[Microsoft Teams Guest Access Enabled](MATCH-S00889.md)|
|LEGACY-S00183|[Mimecast - Message with Virus Detections from IP](LEGACY-S00183.md)|
|LEGACY-S00184|[Mimecast - Message with Virus Detections to Recipient](LEGACY-S00184.md)|
|LEGACY-S00185|[Mimecast - SPAM Message from IP](LEGACY-S00185.md)|
|LEGACY-S00186|[Mimecast - SPAM Message to Recipient](LEGACY-S00186.md)|
|MATCH-S00681|[Mimecast Message Held](MATCH-S00681.md)|
|MATCH-S00397|[Mimikatz Loaded Images Detected](MATCH-S00397.md)|
|MATCH-S00404|[Mimikatz via Powershell and EventID 4703](MATCH-S00404.md)|
|MATCH-S00750|[Modification of Windows Network Logon Scripts](MATCH-S00750.md)|
|MATCH-S00466|[MsiExec Web Install](MATCH-S00466.md)|
|THRESHOLD-S00112|[Multiple Azure Firewall Deny Events for IP](THRESHOLD-S00112.md)|
|THRESHOLD-S00113|[Multiple Azure Firewall Deny Events for URL](THRESHOLD-S00113.md)|
|MATCH-S00419|[Multiple File Extensions](MATCH-S00419.md)|
|THRESHOLD-S00077|[Multiple Windows Account Lockouts On Endpoint](THRESHOLD-S00077.md)|
|MATCH-S00743|[Network Connection from Control Panel - Sysmon](MATCH-S00743.md)|
|MATCH-S00736|[Network Connection from InstallUtil - Sysmon](MATCH-S00736.md)|
|MATCH-S00737|[Network Connection from MSHTA - Sysmon](MATCH-S00737.md)|
|MATCH-S00738|[Network Connection from Msiexec - Sysmon](MATCH-S00738.md)|
|MATCH-S00744|[Network Connection from Odbcconf - Sysmon](MATCH-S00744.md)|
|MATCH-S00740|[Network Connection from Regsvcs/Regasm - Sysmon](MATCH-S00740.md)|
|MATCH-S00742|[Network Connection from Regsvr32 - Sysmon](MATCH-S00742.md)|
|MATCH-S00741|[Network Connection from Rundll32 - Sysmon](MATCH-S00741.md)|
|MATCH-S00739|[Network Connection from Verclsid - Sysmon](MATCH-S00739.md)|
|THRESHOLD-S00059|[Network Share Scan](THRESHOLD-S00059.md)|
|THRESHOLD-S00060|[Network Share Sweep](THRESHOLD-S00060.md)|
|MATCH-S00868|[New Binding Role Created on AWS EKS](MATCH-S00868.md)|
|MATCH-S00867|[New Cluster Admin Binding Role Created on AWS EKS](MATCH-S00867.md)|
|MATCH-S00655|[New Container Uploaded to AWS ECR](MATCH-S00655.md)|
|MATCH-S00644|[New Kubernetes Namespace Created](MATCH-S00644.md)|
|MATCH-S00156|[New Suspicious cmd.exe / regedit.exe / powershell.exe Service Launch](MATCH-S00156.md)|
|MATCH-S00152|[New or Renamed Windows User Account Mimicking a Machine Account](MATCH-S00152.md)|
|MATCH-S00895|[NinjaCopy Usage Detected](MATCH-S00895.md)|
|LEGACY-S00181|[Noncompliant Protocol Tunnel Over Common Service Port](LEGACY-S00181.md)|
|MATCH-S00402|[Normalized Security Signal](MATCH-S00402.md)|
|MATCH-S00288|[NotPetya Ransomware Activity](MATCH-S00288.md)|
|MATCH-S00455|[O365 - Successful Authentication with PowerShell User Agent](MATCH-S00455.md)|
|MATCH-S00068|[O365 - Users Password Changed](MATCH-S00068.md)|
|MATCH-S00069|[O365 - Users Password Reset](MATCH-S00069.md)|
|MATCH-S01053|[OCSF Compliance Finding](MATCH-S01053.md)|
|MATCH-S01054|[OCSF Detection Finding](MATCH-S01054.md)|
|MATCH-S01055|[OCSF Vulnerability Finding](MATCH-S01055.md)|
|MATCH-S00828|[Office 365 Exchange Transport Rule Created](MATCH-S00828.md)|
|MATCH-S00829|[Office 365 Exchange Transport Rule Enabled](MATCH-S00829.md)|
|MATCH-S00830|[Office 365 Forwarding Rule Created](MATCH-S00830.md)|
|MATCH-S00833|[Office 365 Inbox Rule Created](MATCH-S00833.md)|
|MATCH-S00832|[Office 365 Inbox Rule Updated](MATCH-S00832.md)|
|MATCH-S00831|[Office 365 Unified Audit Logging Disabled](MATCH-S00831.md)|
|MATCH-S00137|[Office Application or Browser Launching Shell](MATCH-S00137.md)|
|MATCH-S00906|[Okta - Application Created](MATCH-S00906.md)|
|MATCH-S00903|[Okta - Device Added To User](MATCH-S00903.md)|
|MATCH-S00904|[Okta - Device Removed From User](MATCH-S00904.md)|
|FIRST-S00070|[Okta - First Seen Application Accessed by User](FIRST-S00070.md)|
|FIRST-S00067|[Okta - First Seen Client ID/ASN combo in successful OIDC token grant](FIRST-S00067.md)|
|FIRST-S00068|[Okta - First Seen User Accessing Admin Application](FIRST-S00068.md)|
|FIRST-S00066|[Okta - First Seen User Requesting Report](FIRST-S00066.md)|
|CHAIN-S00020|[Okta - MFA Denied Followed by Successful Logon](CHAIN-S00020.md)|
|MATCH-S00908|[Okta - MFA Request Denied by User](MATCH-S00908.md)|
|OUTLIER-S00018|[Okta - Outlier in ASNs Used to Access Applications](OUTLIER-S00018.md)|
|OUTLIER-S00017|[Okta - Outlier in MFA Attempts Denied by User](OUTLIER-S00017.md)|
|OUTLIER-S00016|[Okta - Outlier in OIDC token request failures](OUTLIER-S00016.md)|
|MATCH-S00907|[Okta - Policy Rule Added](MATCH-S00907.md)|
|MATCH-S00905|[Okta - Programmatic Access to Users API Endpoint](MATCH-S00905.md)|
|AGGREGATION-S00008|[Okta - Session Anomaly (Multiple ASNs)](AGGREGATION-S00008.md)|
|AGGREGATION-S00007|[Okta - Session Anomaly (Multiple Operating Systems)](AGGREGATION-S00007.md)|
|AGGREGATION-S00009|[Okta - Session Anomaly (Multiple User Agents)](AGGREGATION-S00009.md)|
|MATCH-S00635|[Okta API Token Created](MATCH-S00635.md)|
|MATCH-S00433|[Okta Account Lockout](MATCH-S00433.md)|
|MATCH-S00769|[Okta Account Primary Email Address Update](MATCH-S00769.md)|
|MATCH-S00634|[Okta Admin App Access Attempt Failed](MATCH-S00634.md)|
|MATCH-S00633|[Okta Admin App Accessed](MATCH-S00633.md)|
|MATCH-S00632|[Okta Administrator Access Granted](MATCH-S00632.md)|
|MATCH-S00765|[Okta Credential Access User Impersonation](MATCH-S00765.md)|
|MATCH-S00768|[Okta MFA Bypass Attempt](MATCH-S00768.md)|
|MATCH-S00766|[Okta MFA Deactivated for User](MATCH-S00766.md)|
|MATCH-S00767|[Okta MFA Device Reset](MATCH-S00767.md)|
|MATCH-S00636|[Okta User Attempted to Access Unauthorized App](MATCH-S00636.md)|
|MATCH-S00605|[OneLogin - API Credentials - New Key Created](MATCH-S00605.md)|
|MATCH-S00609|[OneLogin - Login Failed - MFA Unsuccessful](MATCH-S00609.md)|
|MATCH-S00556|[Outbound Data Transfer Protocol Over Non-standard Port](MATCH-S00556.md)|
|MATCH-S00554|[Outbound IRC Traffic](MATCH-S00554.md)|
|LEGACY-S00056|[Outbound TFTP Traffic](LEGACY-S00056.md)|
|THRESHOLD-S00048|[Outbound Traffic to Countries Outside the United States](THRESHOLD-S00048.md)|
|OUTLIER-S00019|[Outlier in AWS Bedrock API Calls from User](OUTLIER-S00019.md)|
|OUTLIER-S00022|[Outlier in AWS Bedrock Foundation Model Enumeration Calls from User ](OUTLIER-S00022.md)|
|OUTLIER-S00013|[Outlier in Data Outbound Per Day by Admin or Sensitive Device](OUTLIER-S00013.md)|
|OUTLIER-S00015|[Outlier in Data Outbound Per Hour by Admin or Sensitive Device](OUTLIER-S00015.md)|
|OUTLIER-S00032|[Outlier in Data Transferred from an S3 Bucket by User](OUTLIER-S00032.md)|
|OUTLIER-S00031|[Outlier in Data Transferred into an S3 Bucket by User](OUTLIER-S00031.md)|
|MATCH-S00755|[Outlook Form Creation](MATCH-S00755.md)|
|MATCH-S00756|[Outlook Homepage Modification](MATCH-S00756.md)|
|MATCH-S00683|[Overly Permissive Chmod Command](MATCH-S00683.md)|
|MATCH-S00900|[Overly-Permissive Active Directory Certificate Template Loaded](MATCH-S00900.md)|
|MATCH-S00890|[Owner Added to Azure Service Principal](MATCH-S00890.md)|
|MATCH-S00698|[PATH Set to Current Directory](MATCH-S00698.md)|
|MATCH-S00610|[PSExec Named Pipe Created by Non-PsExec Process](MATCH-S00610.md)|
|MATCH-S00465|[PXELoot Utility](MATCH-S00465.md)|
|MATCH-S00659|[Package Management Utility in Container](MATCH-S00659.md)|
|THRESHOLD-S00095|[Password Attack from Host](THRESHOLD-S00095.md)|
|THRESHOLD-S00116|[Password Attack from IP](THRESHOLD-S00116.md)|
|LEGACY-S00058|[Pastebin Raw URL Resource Request](LEGACY-S00058.md)|
|MATCH-S00704|[Persistence Registry Key Modification](MATCH-S00704.md)|
|THRESHOLD-S00520|[Persistent Malware Infection](THRESHOLD-S00520.md)|
|MATCH-S00697|[Pkexec Privilege Escalation - CVE-2021-4034](MATCH-S00697.md)|
|MATCH-S00887|[Port Forwarding Enabled via Visual Studio Code](MATCH-S00887.md)|
|LEGACY-S00059|[Port Scan - External](LEGACY-S00059.md)|
|LEGACY-S00060|[Port Scan - Internal](LEGACY-S00060.md)|
|LEGACY-S00005|[Possible Black Energy Command and Control](LEGACY-S00005.md)|
|THRESHOLD-S00026|[Possible Credential Abuse](THRESHOLD-S00026.md)|
|LEGACY-S00061|[Possible DNS Data Exfiltration](LEGACY-S00061.md)|
|THRESHOLD-S00040|[Possible DNS over TLS (DoT) Activity](THRESHOLD-S00040.md)|
|LEGACY-S00008|[Possible Dynamic DNS Domain](LEGACY-S00008.md)|
|MATCH-S00835|[Possible Dynamic URL Domain](MATCH-S00835.md)|
|MATCH-S00637|[Possible Malicious Download](MATCH-S00637.md)|
|MATCH-S00451|[Possible Malicious Nirsoft Tool Usage](MATCH-S00451.md)|
|THRESHOLD-S00028|[Possible TOR Connection](THRESHOLD-S00028.md)|
|MATCH-S00876|[Potential AWS Security Credential Access via curl](MATCH-S00876.md)|
|CHAIN-S00019|[Potential Active Directory Certificate Services Enrollment Agent Misconfiguration](CHAIN-S00019.md)|
|CHAIN-S00012|[Potential Azure Persistence via Automation Accounts](CHAIN-S00012.md)|
|MATCH-S00459|[Potential Cobalt Strike Profile](MATCH-S00459.md)|
|MATCH-S00865|[Potential Docker Escape via Command Line](MATCH-S00865.md)|
|CHAIN-S00014|[Potential Docker container escape via Cgroups](CHAIN-S00014.md)|
|MATCH-S00558|[Potential Inbound VNC Traffic](MATCH-S00558.md)|
|CHAIN-S00011|[Potential InstallUtil Allow List Bypass](CHAIN-S00011.md)|
|MATCH-S00822|[Potential Microsoft Office In-Memory Token Theft](MATCH-S00822.md)|
|MATCH-S00753|[Potential Microsoft Office Template Abuse](MATCH-S00753.md)|
|MATCH-S00200|[Potential Pass the Hash Activity](MATCH-S00200.md)|
|MATCH-S00546|[Potential Reconnaissance Obfuscation](MATCH-S00546.md)|
|MATCH-S00824|[Potential XMRig Execution with Traffic](MATCH-S00824.md)|
|LEGACY-S00062|[Potential malicious JVM download](LEGACY-S00062.md)|
|LEGACY-S00063|[Potential malicious document executed](LEGACY-S00063.md)|
|MATCH-S00898|[Potentially Misconfigured Active Directory Certificate Template Loaded](MATCH-S00898.md)|
|MATCH-S00901|[Potentially Vulnerable Active Directory Certificate Services Template Loaded](MATCH-S00901.md)|
|LEGACY-S00064|[Potentially vulnerable software detected](LEGACY-S00064.md)|
|MATCH-S00136|[PowerShell Encoded Command](MATCH-S00136.md)|
|MATCH-S00149|[PowerShell File Download](MATCH-S00149.md)|
|LEGACY-S00066|[PowerShell Remote Administration](LEGACY-S00066.md)|
|MATCH-S00425|[PowerShell Rundll32 Remote Thread Creation](MATCH-S00425.md)|
|LEGACY-S00065|[PowerShell via SMB](LEGACY-S00065.md)|
|MATCH-S00449|[Powershell Execution Policy Bypass](MATCH-S00449.md)|
|MATCH-S00580|[Powerview Add-DomainObjectAcl DCSync AD Extend Right](MATCH-S00580.md)|
|MATCH-S00866|[Privileged Pod Created on AWS EKS](MATCH-S00866.md)|
|MATCH-S00427|[Process Dump via Rundll32 and Comsvcs.dll](MATCH-S00427.md)|
|MATCH-S00187|[Process Execution Inside Webserver Root Folder](MATCH-S00187.md)|
|MATCH-S00691|[Productivity App Spawning Rundll32 or Regsvr32](MATCH-S00691.md)|
|MATCH-S00694|[Proofpoint POD Suspicious Email](MATCH-S00694.md)|
|MATCH-S00078|[Proofpoint TAP - IP Sent Email with Malware](MATCH-S00078.md)|
|MATCH-S00079|[Proofpoint TAP - IP Sent Email with Malware Link](MATCH-S00079.md)|
|MATCH-S00080|[Proofpoint TAP - IP Sent Email with Phishing Link](MATCH-S00080.md)|
|MATCH-S00081|[Proofpoint TAP - IP Sent Impostor Email](MATCH-S00081.md)|
|MATCH-S00082|[Proofpoint TAP - IP Sent Phishing Email](MATCH-S00082.md)|
|MATCH-S00084|[Proofpoint TAP - User Clicked Malware Link in Email](MATCH-S00084.md)|
|MATCH-S00085|[Proofpoint TAP - User Clicked Phishing Link in Email](MATCH-S00085.md)|
|MATCH-S00083|[Proofpoint TAP - User Received Email with Malware](MATCH-S00083.md)|
|MATCH-S00086|[Proofpoint TAP - User Received Impostor Email](MATCH-S00086.md)|
|MATCH-S00087|[Proofpoint TAP - User Received Phishing Email](MATCH-S00087.md)|
|LEGACY-S00057|[PsExec Admin Tool Detection](LEGACY-S00057.md)|
|MATCH-S00439|[Psr.exe Capture Screenshots](MATCH-S00439.md)|
|MATCH-S00584|[Pwndrp Access](MATCH-S00584.md)|
|MATCH-S00575|[QBot Process Creation](MATCH-S00575.md)|
|MATCH-S00265|[QuarksPwDump Dump File Observed](MATCH-S00265.md)|
|LEGACY-S00068|[RDP Brute Force - Success](LEGACY-S00068.md)|
|THRESHOLD-S00031|[RDP Brute Force Attempt](THRESHOLD-S00031.md)|
|LEGACY-S00069|[RDP Error Messages](LEGACY-S00069.md)|
|MATCH-S00176|[RDP Login from Localhost](MATCH-S00176.md)|
|MATCH-S00502|[RDP Traffic to Unexpected Host](MATCH-S00502.md)|
|LEGACY-S00071|[RDP with non-standard client](LEGACY-S00071.md)|
|MATCH-S00167|[Recon Using Common Windows Commands](MATCH-S00167.md)|
|MATCH-S00545|[Registry Keys For Creating Shim Databases](MATCH-S00545.md)|
|MATCH-S00747|[Registry Modification - Active Setup](MATCH-S00747.md)|
|MATCH-S00705|[Registry Modification - Authentication Package](MATCH-S00705.md)|
|MATCH-S00730|[Registry Modification - Code Signing](MATCH-S00730.md)|
|MATCH-S00754|[Registry Modification - Microsoft Office Test Function Registry Entry](MATCH-S00754.md)|
|MATCH-S00733|[Registry Modification - Print Processors](MATCH-S00733.md)|
|MATCH-S00735|[Registry Modification - SIP or Trust Provider](MATCH-S00735.md)|
|MATCH-S00722|[Registry Modification - Security Support Provider](MATCH-S00722.md)|
|MATCH-S00706|[Registry Modification - Time Providers](MATCH-S00706.md)|
|MATCH-S00749|[Registry Modification - Windows Logon Script](MATCH-S00749.md)|
|MATCH-S00707|[Registry Modification - Winlogon Helper DLL](MATCH-S00707.md)|
|MATCH-S00569|[Registry Persistence Mechanisms](MATCH-S00569.md)|
|MATCH-S00689|[Regsvr32.exe Silent Mode from TEMP Directory](MATCH-S00689.md)|
|MATCH-S00475|[Renamed MSBUILD.EXE by Arguments](MATCH-S00475.md)|
|LEGACY-S00001|[Request to Anomalous Web Server Software](LEGACY-S00001.md)|
|LEGACY-S00072|[Request to DNS over HTTPS (DoH) Service Provider](LEGACY-S00072.md)|
|MATCH-S00501|[Rogue DHCP Server - Cisco](MATCH-S00501.md)|
|MATCH-S00328|[Rubeus Hack Tool](MATCH-S00328.md)|
|MATCH-S00498|[Rubeus Hack Tool Logon Process Name](MATCH-S00498.md)|
|MATCH-S00690|[Rundll32.exe Load from TEMP Directory with By Ordinal Load](MATCH-S00690.md)|
|MATCH-S00346|[Ryuk Ransomware Endpoint Indicator](MATCH-S00346.md)|
|MATCH-S00506|[SC Exe Manipulating Windows Services](MATCH-S00506.md)|
|LEGACY-S00075|[SMB - Remote execution and/or persistence via scheduled task using ATSVC ](LEGACY-S00075.md)|
|THRESHOLD-S00032|[SMB Brute Force Attempt](THRESHOLD-S00032.md)|
|LEGACY-S00073|[SMB External to Internal File Share Access](LEGACY-S00073.md)|
|LEGACY-S00074|[SMB Internal to External traffic](LEGACY-S00074.md)|
|THRESHOLD-S00033|[SMB Scanning Detected](THRESHOLD-S00033.md)|
|LEGACY-S00076|[SMB write to hidden admin share](LEGACY-S00076.md)|
|MATCH-S00560|[SMTP Traffic from Non-SMTP Servers](MATCH-S00560.md)|
|LEGACY-S00077|[SQL Injection Attacker](LEGACY-S00077.md)|
|LEGACY-S00078|[SQL Injection Victim](LEGACY-S00078.md)|
|LEGACY-S00079|[SQL-Select-From](LEGACY-S00079.md)|
|THRESHOLD-S00034|[SSH Authentication Failures](THRESHOLD-S00034.md)|
|LEGACY-S00080|[SSH Interesting Hostname Login](LEGACY-S00080.md)|
|MATCH-S00826|[SSH Keys Added to EC2 Instance](MATCH-S00826.md)|
|LEGACY-S00084|[SSL Certificate Expired](LEGACY-S00084.md)|
|LEGACY-S00085|[SSL Certificate Expires Soon](LEGACY-S00085.md)|
|LEGACY-S00086|[SSL Certificate Not Valid Yet](LEGACY-S00086.md)|
|LEGACY-S00087|[SSL Heartbleed Attack](LEGACY-S00087.md)|
|LEGACY-S00088|[SSL Heartbleed Attack Successful](LEGACY-S00088.md)|
|LEGACY-S00089|[SSL Heartbleed Many Requests](LEGACY-S00089.md)|
|LEGACY-S00090|[SSL Heartbleed Odd Length](LEGACY-S00090.md)|
|LEGACY-S00091|[SSL Invalid Server Cert](LEGACY-S00091.md)|
|THRESHOLD-S00061|[SYSVOL Share Sweep](THRESHOLD-S00061.md)|
|MATCH-S00468|[SafetyKatz Credential Stealer](MATCH-S00468.md)|
|MATCH-S00774|[Salesforce Custom Permission Creation](MATCH-S00774.md)|
|THRESHOLD-S00108|[Salesforce Excessive Documents Downloaded](THRESHOLD-S00108.md)|
|MATCH-S00770|[Salesforce Login Attempt from Disabled Account](MATCH-S00770.md)|
|MATCH-S00773|[Salesforce LoginAs Event](MATCH-S00773.md)|
|MATCH-S00780|[Salesforce Permission Set Addition](MATCH-S00780.md)|
|MATCH-S00778|[Salesforce Permission Set Assigned](MATCH-S00778.md)|
|MATCH-S00779|[Salesforce Permission Set Creation](MATCH-S00779.md)|
|MATCH-S00782|[Salesforce Permission Set Deletion](MATCH-S00782.md)|
|MATCH-S00781|[Salesforce Permission Set Modification](MATCH-S00781.md)|
|MATCH-S00772|[Salesforce Report Exported](MATCH-S00772.md)|
|MATCH-S00777|[Salesforce Role Creation](MATCH-S00777.md)|
|MATCH-S00775|[Salesforce User Creation](MATCH-S00775.md)|
|MATCH-S00776|[Salesforce User Role Changed](MATCH-S00776.md)|
|MATCH-S00771|[Salesforce WaveDownload Event](MATCH-S00771.md)|
|MATCH-S00528|[Samsam Test File Write](MATCH-S00528.md)|
|MATCH-S00153|[Scheduled Task Created via PowerShell](MATCH-S00153.md)|
|MATCH-S00214|[Scheduled Task Creation with Suspicious Task Executable](MATCH-S00214.md)|
|MATCH-S00529|[Schtasks Scheduling Job On Remote System](MATCH-S00529.md)|
|MATCH-S00530|[Schtasks Used For Forcing A Reboot](MATCH-S00530.md)|
|MATCH-S00547|[Script Execution Via WMI](MATCH-S00547.md)|
|MATCH-S00447|[Script Interpreter Launched by Cmd](MATCH-S00447.md)|
|LEGACY-S00093|[Script/CLI UserAgent string](LEGACY-S00093.md)|
|MATCH-S00478|[Seatbelt Utility](MATCH-S00478.md)|
|MATCH-S00893|[Secret Added to Azure Service Principal](MATCH-S00893.md)|
|MATCH-S00437|[Secure Deletion with SDelete](MATCH-S00437.md)|
|MATCH-S00299|[SecurityXploded Tool](MATCH-S00299.md)|
|LEGACY-S00094|[Self-signed Certificates](LEGACY-S00094.md)|
|MATCH-S00834|[Sensitive Registry Key (WDigest) Edit](MATCH-S00834.md)|
|LEGACY-S00095|[Server-Side Code Injection in URL](LEGACY-S00095.md)|
|CHAIN-S00010|[Service Installation Followed By Elevated CMD Prompt](CHAIN-S00010.md)|
|MATCH-S00296|[Shadow Copies Deletion Using OS Utilities](MATCH-S00296.md)|
|MATCH-S00406|[Shadow Copy Creation](MATCH-S00406.md)|
|MATCH-S00471|[SharPersist A Utility](MATCH-S00471.md)|
|MATCH-S00469|[SharPersist Utility](MATCH-S00469.md)|
|MATCH-S00472|[SharPivot Utility](MATCH-S00472.md)|
|MATCH-S01051|[SharePoint Server ToolShell Exploitation (CVE-2025-53770, CVE-2025-53771)](MATCH-S01051.md)|
|MATCH-S01052|[SharePoint Server ToolShell Web Shell Interaction (CVE-2025-53771)](MATCH-S01052.md)|
|THRESHOLD-S00111|[Sharepoint - Excessive Documents Accessed by External IP](THRESHOLD-S00111.md)|
|THRESHOLD-S00101|[Sharepoint - Excessive Documents Accessed by User](THRESHOLD-S00101.md)|
|THRESHOLD-S00100|[Sharepoint - Excessive Documents Downloaded](THRESHOLD-S00100.md)|
|THRESHOLD-S00110|[Sharepoint - External IP Downloaded Excessive Documents](THRESHOLD-S00110.md)|
|MATCH-S00473|[SharpStomp Utility](MATCH-S00473.md)|
|LEGACY-S00096|[Shellshock](LEGACY-S00096.md)|
|MATCH-S00692|[Silent Regsvr32 Scheduled Task Creation on Command Line](MATCH-S00692.md)|
|THRESHOLD-S00086|[Slack - Mass Download Events](THRESHOLD-S00086.md)|
|THRESHOLD-S00087|[Slack - Possible Session Hijacking](THRESHOLD-S00087.md)|
|MATCH-S00370|[Snatch Ransomware](MATCH-S00370.md)|
|MATCH-S00571|[Sofacy Trojan Loader](MATCH-S00571.md)|
|MATCH-S00480|[Solarwinds Suspicious Child Processes](MATCH-S00480.md)|
|MATCH-S00481|[Solarwinds Suspicious URL Hostname](MATCH-S00481.md)|
|MATCH-S00422|[Spaces Before File Extension](MATCH-S00422.md)|
|OUTLIER-S00005|[Spike in AWS API Call from User](OUTLIER-S00005.md)|
|OUTLIER-S00011|[Spike in AWS AccessDenied Events by assumedrole](OUTLIER-S00011.md)|
|OUTLIER-S00004|[Spike in Azure Firewall Deny Events from Source IP](OUTLIER-S00004.md)|
|OUTLIER-S00006|[Spike in Data Transferred Outbound by User](OUTLIER-S00006.md)|
|OUTLIER-S00008|[Spike in Failed Azure Sign In Attempts Due to Bad Password from IP Address](OUTLIER-S00008.md)|
|OUTLIER-S00003|[Spike in Failed Share Access by User](OUTLIER-S00003.md)|
|OUTLIER-S00001|[Spike in Login Failures from a User](OUTLIER-S00001.md)|
|OUTLIER-S00009|[Spike in PowerShell Command Line Length From Host](OUTLIER-S00009.md)|
|OUTLIER-S00002|[Spike in Successful Distinct Share Access](OUTLIER-S00002.md)|
|OUTLIER-S00010|[Spike in URL Length from IP Address](OUTLIER-S00010.md)|
|OUTLIER-S00007|[Spike in Windows Administrative Privileges Granted for User](OUTLIER-S00007.md)|
|MATCH-S00507|[Spoolsv Child Process Created](MATCH-S00507.md)|
|MATCH-S00783|[Spring4Shell Exploitation - URL](MATCH-S00783.md)|
|CHAIN-S00008|[Successful Brute Force](CHAIN-S00008.md)|
|MATCH-S00196|[Successful Overpass the Hash Attempt](MATCH-S00196.md)|
|MATCH-S00090|[Sumo Logic Scheduled Searches](MATCH-S00090.md)|
|MATCH-S00470|[Sunburst Suspicious File Writes](MATCH-S00470.md)|
|MATCH-S00337|[Suspect Svchost Activity](MATCH-S00337.md)|
|MATCH-S00841|[Suspicious AWS CLI Keys Access on Linux Host](MATCH-S00841.md)|
|AGGREGATION-S00003|[Suspicious AWS Lambda Enumeration](AGGREGATION-S00003.md)|
|MATCH-S00899|[Suspicious Active Directory Certificate Modification](MATCH-S00899.md)|
|MATCH-S00902|[Suspicious Active Directory Certificate Modification - Enrollment Agent](MATCH-S00902.md)|
|MATCH-S00817|[Suspicious Azure Active Directory Device Code Authentication](MATCH-S00817.md)|
|MATCH-S00842|[Suspicious Azure CLI Keys Access on Linux Host](MATCH-S00842.md)|
|MATCH-S00359|[Suspicious Certutil Command](MATCH-S00359.md)|
|MATCH-S00356|[Suspicious Compression Tool Parameters](MATCH-S00356.md)|
|MATCH-S00362|[Suspicious Curl File Upload](MATCH-S00362.md)|
|LEGACY-S00105|[Suspicious DC Logon](LEGACY-S00105.md)|
|MATCH-S00499|[Suspicious Email Attachment Extension](MATCH-S00499.md)|
|LEGACY-S00106|[Suspicious Email Origin](LEGACY-S00106.md)|
|MATCH-S00476|[Suspicious Execution of Search Indexer](MATCH-S00476.md)|
|MATCH-S00293|[Suspicious External Device Installation](MATCH-S00293.md)|
|MATCH-S00843|[Suspicious GCP CLI Keys Access on Linux Host](MATCH-S00843.md)|
|LEGACY-S00182|[Suspicious HTTP User-Agent](LEGACY-S00182.md)|
|AGGREGATION-S00004|[Suspicious K8s Enumeration](AGGREGATION-S00004.md)|
|MATCH-S00840|[Suspicious Lambda Function - IAM Policy Attached](MATCH-S00840.md)|
|CHAIN-S00015|[Suspicious Linux Execution Chain](CHAIN-S00015.md)|
|MATCH-S00464|[Suspicious Non-Standard InstallUtil Execution](MATCH-S00464.md)|
|MATCH-S00917|[Suspicious PowerShell Application Window Discovery COM method ](MATCH-S00917.md)|
|MATCH-S00191|[Suspicious PowerShell Keywords](MATCH-S00191.md)|
|MATCH-S00920|[Suspicious PowerShell Window Discovery Cmdlet execution](MATCH-S00920.md)|
|MATCH-S00135|[Suspicious Registry Key Modification](MATCH-S00135.md)|
|MATCH-S00164|[Suspicious Shells Spawned by Web Servers](MATCH-S00164.md)|
|MATCH-S00500|[Suspicious Shortcut File Launching Process](MATCH-S00500.md)|
|AGGREGATION-S00005|[Suspicious System Enumeration Occurring in Quick Succession](AGGREGATION-S00005.md)|
|MATCH-S00350|[Suspicious Typical Malware Back Connect Ports](MATCH-S00350.md)|
|MATCH-S00431|[Suspicious Use of Procdump](MATCH-S00431.md)|
|MATCH-S00477|[Suspicious Use of Workflow Compiler for Payload Execution](MATCH-S00477.md)|
|MATCH-S00158|[Suspicious Windows ANONYMOUS LOGON Account Created](MATCH-S00158.md)|
|MATCH-S00551|[Suspicious Writes To System Volume Information](MATCH-S00551.md)|
|MATCH-S00550|[Suspicious Writes To Windows Recycle Bin](MATCH-S00550.md)|
|MATCH-S00918|[Suspicious cat of PAM common-password policy](MATCH-S00918.md)|
|MATCH-S00886|[Suspicious chmod Execution](MATCH-S00886.md)|
|MATCH-S00342|[Suspicious use of Dev-Tools-Launcher](MATCH-S00342.md)|
|MATCH-S00699|[Sysmon - RawAccessRead Event](MATCH-S00699.md)|
|MATCH-S00279|[TAIDOOR RAT DLL Load](MATCH-S00279.md)|
|MATCH-S00595|[Telegram API Access](MATCH-S00595.md)|
|LEGACY-S00170|[The Audit Log was Cleared - 1102](LEGACY-S00170.md)|
|MATCH-S01010|[Threat Intel - DNS Query Domain](MATCH-S01010.md)|
|MATCH-S01011|[Threat Intel - DNS Reply Domain](MATCH-S01011.md)|
|MATCH-S01007|[Threat Intel - Destination Device Hostname](MATCH-S01007.md)|
|MATCH-S01024|[Threat Intel - Destination IP Address (High Confidence)](MATCH-S01024.md)|
|MATCH-S01026|[Threat Intel - Destination IP Address (Low Confidence)](MATCH-S01026.md)|
|MATCH-S01028|[Threat Intel - Destination IP Address (Medium Confidence)](MATCH-S01028.md)|
|MATCH-S01006|[Threat Intel - Device Hostname](MATCH-S01006.md)|
|LEGACY-S00110|[Threat Intel - Device IP Matched Threat Intel Domain Name](LEGACY-S00110.md)|
|LEGACY-S00111|[Threat Intel - Device IP Matched Threat Intel URL](LEGACY-S00111.md)|
|MATCH-S01008|[Threat Intel - HTTP Hostname](MATCH-S01008.md)|
|MATCH-S01009|[Threat Intel - HTTP Referer](MATCH-S01009.md)|
|MATCH-S01012|[Threat Intel - HTTP Referer Root Domain](MATCH-S01012.md)|
|MATCH-S01015|[Threat Intel - HTTP URL](MATCH-S01015.md)|
|MATCH-S01014|[Threat Intel - HTTP URL FQDN](MATCH-S01014.md)|
|MATCH-S01013|[Threat Intel - HTTP URL Root Domain](MATCH-S01013.md)|
|MATCH-S00999|[Threat Intel - IMPHASH Match](MATCH-S00999.md)|
|MATCH-S00555|[Threat Intel - Inbound Traffic Context](MATCH-S00555.md)|
|MATCH-S01023|[Threat Intel - Inbound Traffic from Threat Feed IP (High Confidence)](MATCH-S01023.md)|
|MATCH-S01025|[Threat Intel - Inbound Traffic from Threat Feed IP (Low Confidence)](MATCH-S01025.md)|
|MATCH-S01027|[Threat Intel - Inbound Traffic from Threat Feed IP (Medium Confidence)](MATCH-S01027.md)|
|MATCH-S01000|[Threat Intel - MD5 Match](MATCH-S01000.md)|
|LEGACY-S00109|[Threat Intel - Matched Domain Name](LEGACY-S00109.md)|
|LEGACY-S00108|[Threat Intel - Matched File Hash](LEGACY-S00108.md)|
|MATCH-S01020|[Threat Intel - Matched Target Email](MATCH-S01020.md)|
|MATCH-S01019|[Threat Intel - Matched User Email](MATCH-S01019.md)|
|MATCH-S01001|[Threat Intel - PEHASH Match](MATCH-S01001.md)|
|MATCH-S01003|[Threat Intel - SHA1 Match](MATCH-S01003.md)|
|MATCH-S01004|[Threat Intel - SHA256 Match](MATCH-S01004.md)|
|MATCH-S01002|[Threat Intel - SSDEEP Match](MATCH-S01002.md)|
|MATCH-S01005|[Threat Intel - Source Hostname](MATCH-S01005.md)|
|MATCH-S01018|[Threat Intel - Successful Authentication from Threat Feed IP](MATCH-S01018.md)|
|MATCH-S00815|[Threat Intel - Successful Authentication from Threat IP](MATCH-S00815.md)|
|LEGACY-S00107|[Threat Intel Match - IP Address](LEGACY-S00107.md)|
|THRESHOLD-S00075|[Too Many Kerberos Encryption Downgrade SPNs (Kerberoasting)](THRESHOLD-S00075.md)|
|THRESHOLD-S00036|[Too many empty/refused DNS queries](THRESHOLD-S00036.md)|
|MATCH-S00561|[Traffic From Embargoed Countries](MATCH-S00561.md)|
|MATCH-S00562|[Traffic To Embargoed Countries](MATCH-S00562.md)|
|MATCH-S00559|[Traffic to Honeypot IP](MATCH-S00559.md)|
|MATCH-S00563|[Traffic to Proxy Anonymizers](MATCH-S00563.md)|
|MATCH-S00588|[Trickbot Malware Recon Activity](MATCH-S00588.md)|
|MATCH-S00925|[Trufflehog AWS Credential Verification Detected](MATCH-S00925.md)|
|MATCH-S00577|[Turla Group Commands](MATCH-S00577.md)|
|MATCH-S00542|[Unauthorized Access Attempt Detected](MATCH-S00542.md)|
|MATCH-S00313|[Unauthorized External Device Installation](MATCH-S00313.md)|
|MATCH-S00751|[Unix/Linux RC Script Modification](MATCH-S00751.md)|
|MATCH-S00531|[Unload Sysmon Filter Driver](MATCH-S00531.md)|
|MATCH-S00656|[Unrecognized Container Image](MATCH-S00656.md)|
|MATCH-S00757|[Unsafe Outlook Rule Creation Enabled](MATCH-S00757.md)|
|MATCH-S00344|[Unsigned Image Loaded by LSASS](MATCH-S00344.md)|
|MATCH-S00762|[Unusual Staging Directory - PolicyDefinitions](MATCH-S00762.md)|
|MATCH-S00567|[Ursnif Malware Registry Key](MATCH-S00567.md)|
|THRESHOLD-S00064|[User Account Created and Deleted in 24 Hours](THRESHOLD-S00064.md)|
|MATCH-S00504|[User Added to Local Administrators](MATCH-S00504.md)|
|CHAIN-S00007|[User Created and Quickly Deleted on Linux Machine](CHAIN-S00007.md)|
|MATCH-S00463|[UserInit Process Launched by MSBuild.exe](MATCH-S00463.md)|
|LEGACY-S00165|[VBS file downloaded from Internet](LEGACY-S00165.md)|
|MATCH-S00892|[Value Added to Azure NSG Group](MATCH-S00892.md)|
|MATCH-S00761|[Volume Shadow Copy Service Stopped](MATCH-S00761.md)|
|MATCH-S00583|[WCE wceaux.dll Access](MATCH-S00583.md)|
|MATCH-S00150|[WMI Launching Shell](MATCH-S00150.md)|
|MATCH-S00147|[WMI Managed Object Format (MOF) Process Execution](MATCH-S00147.md)|
|MATCH-S00523|[WMI Permanent Event Subscription](MATCH-S00523.md)|
|MATCH-S00524|[WMI Permanent Event Subscription - Sysmon](MATCH-S00524.md)|
|MATCH-S00760|[WMI Ping Sweep](MATCH-S00760.md)|
|MATCH-S00146|[WMI Process Call Create](MATCH-S00146.md)|
|MATCH-S00151|[WMI Process Get Brief](MATCH-S00151.md)|
|MATCH-S00522|[WMI Temporary Event Subscription](MATCH-S00522.md)|
|MATCH-S00379|[WMIExec VBS Script](MATCH-S00379.md)|
|MATCH-S00570|[WMIPRVSE Spawning Process](MATCH-S00570.md)|
|MATCH-S00316|[WannaCry Ransomware](MATCH-S00316.md)|
|MATCH-S00400|[Web Download via Office Binaries](MATCH-S00400.md)|
|MATCH-S00557|[Web Request to IP Address](MATCH-S00557.md)|
|MATCH-S00566|[Web Request to Punycode Domain](MATCH-S00566.md)|
|MATCH-S00539|[Web Servers Executing Suspicious Processes](MATCH-S00539.md)|
|MATCH-S00174|[Web Services Executing Common Web Shell Commands](MATCH-S00174.md)|
|THRESHOLD-S00041|[Websense - Blocked Activity Threshold](THRESHOLD-S00041.md)|
|MATCH-S00684|[Wget Passed to Script Execution Command](MATCH-S00684.md)|
|MATCH-S00521|[Windows - Critical Service Disabled via Command Line](MATCH-S00521.md)|
|MATCH-S00284|[Windows - Delete Windows Backup Catalog](MATCH-S00284.md)|
|MATCH-S00693|[Windows - Denied RDP](MATCH-S00693.md)|
|MATCH-S00181|[Windows - Domain Trust Discovery](MATCH-S00181.md)|
|THRESHOLD-S00065|[Windows - Excessive User Interactive Logons Across Multiple Hosts](THRESHOLD-S00065.md)|
|MATCH-S00202|[Windows - Incoming LSASS Network Connection - Zerologon Behavior(CVE-2020-1472)](MATCH-S00202.md)|
|MATCH-S00168|[Windows - Local System executing whoami.exe](MATCH-S00168.md)|
|MATCH-S00169|[Windows - Microsoft Office Add-In File Created](MATCH-S00169.md)|
|MATCH-S00310|[Windows - Network Connection from CMSTP](MATCH-S00310.md)|
|MATCH-S00162|[Windows - Network trace capture using netsh.exe](MATCH-S00162.md)|
|MATCH-S00159|[Windows - Permissions Group Discovery](MATCH-S00159.md)|
|MATCH-S00268|[Windows - Possible Impersonation Token Creation Using Runas](MATCH-S00268.md)|
|MATCH-S00276|[Windows - Possible Squiblydoo Technique Observed](MATCH-S00276.md)|
|MATCH-S00281|[Windows - PowerShell Process Discovery](MATCH-S00281.md)|
|MATCH-S00171|[Windows - Powershell Scheduled Task Creation from PowerSploit or Empire](MATCH-S00171.md)|
|MATCH-S00185|[Windows - Remote System Discovery](MATCH-S00185.md)|
|MATCH-S00272|[Windows - Rogue Domain Controller - dcshadow](MATCH-S00272.md)|
|MATCH-S00170|[Windows - Scheduled Task Creation](MATCH-S00170.md)|
|CHAIN-S00002|[Windows - Suspicious Anonymous Logon Activity - Zerologon Behavior(CVE-2020-1472)](CHAIN-S00002.md)|
|MATCH-S00285|[Windows - Suspicious CMSTP Process Spawn](MATCH-S00285.md)|
|MATCH-S00192|[Windows - System Network Configuration Discovery](MATCH-S00192.md)|
|MATCH-S00194|[Windows - System Time Discovery](MATCH-S00194.md)|
|MATCH-S00107|[Windows - User Adds Self to Security Group](MATCH-S00107.md)|
|MATCH-S00172|[Windows - WiFi Credential Harvesting with netsh](MATCH-S00172.md)|
|LEGACY-S00169|[Windows Account Added To Privileged Security Group](LEGACY-S00169.md)|
|LEGACY-S00168|[Windows Account Locked Out - 4740](LEGACY-S00168.md)|
|MATCH-S00532|[Windows Adfind Exe](MATCH-S00532.md)|
|MATCH-S00189|[Windows Admin User Remote Logon](MATCH-S00189.md)|
|MATCH-S00552|[Windows Connhost Started Forcefully](MATCH-S00552.md)|
|MATCH-S00274|[Windows Credential Editor (WCE) Tool Use Detected](MATCH-S00274.md)|
|MATCH-S00291|[Windows Credential Editor (WCE) in use](MATCH-S00291.md)|
|MATCH-S00398|[Windows Defender Download Activity](MATCH-S00398.md)|
|MATCH-S00549|[Windows Disable Antispyware Registry](MATCH-S00549.md)|
|MATCH-S00538|[Windows Firewall Rule Added](MATCH-S00538.md)|
|MATCH-S00537|[Windows Firewall Rule Deleted](MATCH-S00537.md)|
|MATCH-S00536|[Windows Firewall Rule Modified](MATCH-S00536.md)|
|MATCH-S00179|[Windows Network Sniffing](MATCH-S00179.md)|
|MATCH-S00732|[Windows Port Monitor Modification](MATCH-S00732.md)|
|MATCH-S00157|[Windows Process Name Impersonation](MATCH-S00157.md)|
|MATCH-S00178|[Windows Query Registry](MATCH-S00178.md)|
|MATCH-S00533|[Windows Security Account Manager Stopped](MATCH-S00533.md)|
|LEGACY-S00171|[Windows Service Executed from Nonstandard Execution Path](LEGACY-S00171.md)|
|LEGACY-S00167|[Windows Temp Directory Access Via SMB](LEGACY-S00167.md)|
|MATCH-S00724|[Windows Update Agent DLL Changed](MATCH-S00724.md)|
|MATCH-S00134|[Windows User Account Created with Abnormal Naming Convention](MATCH-S00134.md)|
|MATCH-S00382|[Winnti Pipemon Characteristics](MATCH-S00382.md)|
|LEGACY-S00172|[Write-only SNMP attempt from external](LEGACY-S00172.md)|
|MATCH-S00734|[XSD Autostart Entry Modification](MATCH-S00734.md)|
|MATCH-S00435|[XSL Script Processing](MATCH-S00435.md)|
|MATCH-S00222|[ZScaler Proxy-Traffic to Malicious Categorized Domain](MATCH-S00222.md)|
|THRESHOLD-S00067|[ZeroLogon Privilege Escalation Behavior](THRESHOLD-S00067.md)|
|MATCH-S00856|[Zoom - Account Created](MATCH-S00856.md)|
|MATCH-S00857|[Zoom - Account Deleted](MATCH-S00857.md)|
|MATCH-S00858|[Zoom - Group Admin Added](MATCH-S00858.md)|
|MATCH-S00859|[Zoom - Group Admin Deleted](MATCH-S00859.md)|
|MATCH-S00860|[Zoom - Group Changes](MATCH-S00860.md)|
|MATCH-S00861|[Zoom - Information Barrier Policy Changes](MATCH-S00861.md)|
|MATCH-S00862|[Zoom - Meeting Risk Alert](MATCH-S00862.md)|
|MATCH-S00863|[Zoom - Recording Modification](MATCH-S00863.md)|
|MATCH-S00508|[Zoom Child Process](MATCH-S00508.md)|
|MATCH-S00061|[Zscaler - Allowed Elevated Risk Score Events](MATCH-S00061.md)|
|MATCH-S00919|[chage command use on host](MATCH-S00919.md)|
|MATCH-S00263|[iOS Implant URL Pattern](MATCH-S00263.md)|
|MATCH-S00880|[macOS - Entitlement Enumeration via Xattr](MATCH-S00880.md)|
|MATCH-S00883|[macOS - Keychain Enumeration](MATCH-S00883.md)|
|MATCH-S00885|[macOS - Screen Sharing Session Established](MATCH-S00885.md)|
|MATCH-S00879|[macOS - Suspicious Osascript Execution](MATCH-S00879.md)|
|CHAIN-S00016|[macOS - Suspicious Osascript Execution and Network Activity](CHAIN-S00016.md)|
|MATCH-S00878|[macOS - Suspicious Osascript Parent Execution](MATCH-S00878.md)|
|MATCH-S00884|[macOS - Suspicious Python PIP Execution](MATCH-S00884.md)|
|MATCH-S00882|[macOS - System Preference Enumeration via Security Binary](MATCH-S00882.md)|
|MATCH-S00881|[macOS - csrutil status Usage Detected](MATCH-S00881.md)|
|MATCH-S00726|[macOS Kernel Extension Load](MATCH-S00726.md)|
|MATCH-S00748|[macOS Login Items Modification](MATCH-S00748.md)|
|MATCH-S00752|[macOS Startup Items Modifications](MATCH-S00752.md)|
|MATCH-S00581|[smbexec.py Service Installation](MATCH-S00581.md)|
|LEGACY-S00179|[vpnoverdns.com DNS lookup](LEGACY-S00179.md)|
