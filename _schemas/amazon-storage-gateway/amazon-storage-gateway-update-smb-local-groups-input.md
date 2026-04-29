---
description: UpdateSMBLocalGroupsInput schema from Amazon Storage Gateway API
layout: schema
name: UpdateSMBLocalGroupsInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: SMBLocalGroups
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-update-smb-local-groups-input-schema.json
slug: amazon-storage-gateway-update-smb-local-groups-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-smb-local-groups-input-schema.json\",\n  \"title\": \"UpdateSMBLocalGroupsInput\",\n  \"description\": \"UpdateSMBLocalGroupsInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"SMBLocalGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SMBLocalGroups\"\n        },\n        {\n          \"description\": \"A list of Active Directory users and groups that you want to grant special permissions for SMB file shares on the gateway.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\",\n    \"SMBLocalGroups\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-smb-local-groups-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: UpdateSMBLocalGroupsInput
---
