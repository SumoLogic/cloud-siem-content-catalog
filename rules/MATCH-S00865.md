# [Rules](README.md): Potential Docker Escape via Command Line

## Description
This rule looks for whether the raw Docker socket was used for container creation as well as a bind mount of /hostfs which could facilitate a container escape and allow command execuiton on the Docker host.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_hostname|
|Signal Name|Potential Docker Escape via Command Line|
|Summary Expression|Potential Docker Escape via Command Line on {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Linux - Sysmon for Linux](../products/b238758d-ade8-41d2-b32d-c99159e9fd74.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|


