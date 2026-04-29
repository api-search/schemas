---
description: UpdateSMBSecurityStrategyInput schema from Amazon Storage Gateway API
layout: schema
name: UpdateSMBSecurityStrategyInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: SMBSecurityStrategy
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-update-smb-security-strategy-input-schema.json
slug: amazon-storage-gateway-update-smb-security-strategy-input
source_filename: amazon-storage-gateway-update-smb-security-strategy-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-smb-security-strategy-input-schema.json\",\n  \"title\": \"UpdateSMBSecurityStrategyInput\",\n  \"description\": \"UpdateSMBSecurityStrategyInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"SMBSecurityStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SMBSecurityStrategy\"\n        },\n        {\n          \"description\": \"<p>Specifies the type of security strategy.</p> <p>ClientSpecified: if you use this option, requests are established based on what is negotiated by the client. This option is recommended when you want to maximize compatibility across different clients in your environment. Supported\
  \ only in S3 File Gateway.</p> <p>MandatorySigning: if you use this option, file gateway only allows connections from SMBv2 or SMBv3 clients that have signing enabled. This option works with SMB clients on Microsoft Windows Vista, Windows Server 2008 or newer.</p> <p>MandatoryEncryption: if you use this option, file gateway only allows connections from SMBv3 clients that have encryption enabled. This option is highly recommended for environments that handle sensitive data. This option works with SMB clients on Microsoft Windows 8, Windows Server 2012 or newer.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\",\n    \"SMBSecurityStrategy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-smb-security-strategy-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: UpdateSMBSecurityStrategyInput
---
