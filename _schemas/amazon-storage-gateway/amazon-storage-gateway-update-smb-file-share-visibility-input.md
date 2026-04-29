---
description: UpdateSMBFileShareVisibilityInput schema from Amazon Storage Gateway API
layout: schema
name: UpdateSMBFileShareVisibilityInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: FileSharesVisible
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-update-smb-file-share-visibility-input-schema.json
slug: amazon-storage-gateway-update-smb-file-share-visibility-input
source_filename: amazon-storage-gateway-update-smb-file-share-visibility-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-smb-file-share-visibility-input-schema.json\",\n  \"title\": \"UpdateSMBFileShareVisibilityInput\",\n  \"description\": \"UpdateSMBFileShareVisibilityInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"FileSharesVisible\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"The shares on this gateway appear when listing shares.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\",\n    \"FileSharesVisible\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-smb-file-share-visibility-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: UpdateSMBFileShareVisibilityInput
---
