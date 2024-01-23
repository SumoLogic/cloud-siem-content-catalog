# [Schema](README.md): Record Types

|Record/Object Type|Description|
|------------------|-----------|
|Audit|Use this record type for log sources that leave a basic audit trail. Whenever possible, it is preferable to use one of these more specific audit record types: AuditChange, AuditFile, or AuditResourceAccess.|
|AuditChange|Use this record type for log sources that leave an audit record indicating a change has occurred on a system.|
|AuditFile|Use this record type for log sources that record information about file changes such as file integrity monitoring.|
|AuditResourceAccess|Use this record type for log sources that track when an entity accesses a resource. For example, the Windows Security-5140 log event indicates when a network share object was accessed.|
|Authentication|Use this record type for log sources that report successful or unsuccessful authentication events.|
|AuthenticationPrivilegeEscalation|Use this record type for authentication log messages that note a user has elevated their privileges.|
|Canary|This is an internal Cloud SIEM record type automatically used to monitor performance. This record type is a SYSTEM type and cannot be used for normalizing log records.|
|Email|Log sources containing email information such as email protection applications and services.|
|Endpoint|Use this record type for log sources based on endpoint behavior. Whenever possible, it is preferable to use one of these more specific endpoint record types: EndpointModuleLoad or EndpointProcess.|
|EndpointModuleLoad|Use this record type for logs that indicate a process is loading one or more modules such as DLL files.|
|EndpointProcess|Use this record type for logs that capture endpoint process auditing.|
|Network|Use this record type for generic log sources that describe network events. Whenever possible, it is preferable to use one of these more specific network record types: NetworkDHCP, NetworkDNS, NetworkFlow, NetworkHTTP, NetworkProxy.|
|NetworkDHCP|Use this record type for network logs generated from a DHCP service.|
|NetworkDNS|Use this record type for network logs generated from a DNS service.|
|NetworkFlow|Use this record type for network logs generated from flow monitoring services such as NetFlow or VPCFlow.|
|NetworkHTTP|Use this record type for network logs generated from HTTP services.|
|NetworkProxy|Use this record type for network logs generated from Proxy services which contains a wide variety of proxy related information.|
|Notification|Use this record type for log sources that report general notifications.|
|NotificationVulnerability|Use this record type for log sources that report notifications about detected vulnerabilities.|
|ParsingFailure|This is an Cloud SIEM record type automatically used when a log record does not match a mapping to generate a Cloud SIEM record. The record contains a reference back to the original log. This record type is a SYSTEM type and cannot be used for normalizing log records.|
