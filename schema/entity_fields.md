# [Schema](README.md): Entity Fields

Here is a list of schema fields which Cloud SIEM considers entites and the type of entity. All Cloud SIEM mappers require you map at least one entity field.

|Field|Entity Type|
|-----|-----------|
|baseImage|_process|
|commandLine|_command|
|device_hostname|_hostname|
|device_hostname_raw|_hostname|
|device_ip|_ip|
|device_k8s_normalizedDeploymentName|_deployment|
|device_k8s_normalizedPodName|_pod|
|device_k8s_normalizedReplicaSetName|_replicaset|
|device_mac|_mac|
|device_natIp|_ip|
|dns_replyIp|_ip|
|dstDevice_hostname|_hostname|
|dstDevice_hostname_raw|_hostname|
|dstDevice_ip|_ip|
|dstDevice_k8s_normalizedDeploymentName|_deployment|
|dstDevice_k8s_normalizedPodName|_pod|
|dstDevice_k8s_normalizedReplicaSetName|_replicaset|
|dstDevice_mac|_mac|
|dstDevice_natIp|_ip|
|file_basename|_file|
|file_hash_imphash|_hash|
|file_hash_md5|_hash|
|file_hash_pehash|_hash|
|file_hash_sha1|_hash|
|file_hash_sha256|_hash|
|file_hash_ssdeep|_hash|
|file_path|_file|
|http_referer_fqdn|_domain|
|http_url|_url|
|http_url_fqdn|_domain|
|http_userAgent|_useragent|
|parentBaseImage|_process|
|repository|_file|
|resource|_resource|
|srcDevice_hostname|_hostname|
|srcDevice_hostname_raw|_hostname|
|srcDevice_ip|_ip|
|srcDevice_k8s_normalizedDeploymentName|_deployment|
|srcDevice_k8s_normalizedPodName|_pod|
|srcDevice_k8s_normalizedReplicaSetName|_replicaset|
|srcDevice_mac|_mac|
|srcDevice_natIp|_ip|
|targetUser_email|_email|
|targetUser_username|_username|
|targetUser_username_raw|_username|
|user_email|_email|
|user_username|_username|
|user_username_raw|_username|


