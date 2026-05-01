---
description: DescribeSMBSettingsOutput schema from Amazon Storage Gateway API
layout: schema
name: DescribeSMBSettingsOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: DomainName
  type: object
- description: ''
  name: ActiveDirectoryStatus
  type: object
- description: ''
  name: SMBGuestPasswordSet
  type: object
- description: ''
  name: SMBSecurityStrategy
  type: object
- description: ''
  name: FileSharesVisible
  type: object
- description: ''
  name: SMBLocalGroups
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-smb-settings-output-schema.json
slug: amazon-storage-gateway-describe-smb-settings-output
source_filename: amazon-storage-gateway-describe-smb-settings-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-smb-settings-output-schema.json\",\n  \"title\": \"DescribeSMBSettingsOutput\",\n  \"description\": \"DescribeSMBSettingsOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain that the gateway is joined to.\"\n        }\n      ]\n    },\n    \"ActiveDirectoryStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActiveDirectoryStatus\"\n        },\n        {\n          \"description\": \"<p>Indicates the status of a gateway that\
  \ is a member of the Active Directory domain.</p> <ul> <li> <p> <code>ACCESS_DENIED</code>: Indicates that the <code>JoinDomain</code> operation failed due to an authentication error.</p> </li> <li> <p> <code>DETACHED</code>: Indicates that gateway is not joined to a domain.</p> </li> <li> <p> <code>JOINED</code>: Indicates that the gateway has successfully joined a domain.</p> </li> <li> <p> <code>JOINING</code>: Indicates that a <code>JoinDomain</code> operation is in progress.</p> </li> <li> <p> <code>NETWORK_ERROR</code>: Indicates that <code>JoinDomain</code> operation failed due to a network or connectivity error.</p> </li> <li> <p> <code>TIMEOUT</code>: Indicates that the <code>JoinDomain</code> operation failed because the operation didn't complete within the allotted time.</p> </li> <li> <p> <code>UNKNOWN_ERROR</code>: Indicates that the <code>JoinDomain</code> operation failed due to another type of error.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"SMBGuestPasswordSet\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>This value is <code>true</code> if a password for the guest user <code>smbguest</code> is set, otherwise <code>false</code>. Only supported for S3 File Gateways.</p> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n        }\n      ]\n    },\n    \"SMBSecurityStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SMBSecurityStrategy\"\n        },\n        {\n          \"description\": \"<p>The type of security strategy that was specified for file gateway.</p> <ul> <li> <p> <code>ClientSpecified</code>: If you use this option, requests are established based on what is negotiated by the client. This option is recommended when you want to maximize compatibility across different clients in your environment. Only supported for S3 File Gateways.</p> </li> <li> <p> <code>MandatorySigning</code>: If you\
  \ use this option, file gateway only allows connections from SMBv2 or SMBv3 clients that have signing enabled. This option works with SMB clients on Microsoft Windows Vista, Windows Server 2008 or newer.</p> </li> <li> <p> <code>MandatoryEncryption</code>: If you use this option, file gateway only allows connections from SMBv3 clients that have encryption enabled. This option is highly recommended for environments that handle sensitive data. This option works with SMB clients on Microsoft Windows 8, Windows Server 2012 or newer.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"FileSharesVisible\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"The shares on this gateway appear when listing shares. Only supported for S3 File Gateways. \"\n        }\n      ]\n    },\n    \"SMBLocalGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SMBLocalGroups\"\n       \
  \ },\n        {\n          \"description\": \"A list of Active Directory users and groups that have special permissions for SMB file shares on the gateway.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-smb-settings-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeSMBSettingsOutput
---
