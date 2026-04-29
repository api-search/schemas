---
description: SetSMBGuestPasswordInput
layout: schema
name: SetSMBGuestPasswordInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: Password
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-set-smb-guest-password-input-schema.json
slug: amazon-storage-gateway-set-smb-guest-password-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-set-smb-guest-password-input-schema.json\",\n  \"title\": \"SetSMBGuestPasswordInput\",\n  \"description\": \"SetSMBGuestPasswordInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the S3 File Gateway the SMB file share is associated with.\"\n        }\n      ]\n    },\n    \"Password\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SMBGuestPassword\"\n        },\n        {\n          \"description\": \"The password that you want to set for your SMB server.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\",\n    \"Password\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-set-smb-guest-password-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: SetSMBGuestPasswordInput
---
