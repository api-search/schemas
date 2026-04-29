---
description: AddUploadBufferInput schema from Amazon Storage Gateway API
layout: schema
name: AddUploadBufferInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: DiskIds
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-add-upload-buffer-input-schema.json
slug: amazon-storage-gateway-add-upload-buffer-input
source_filename: amazon-storage-gateway-add-upload-buffer-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-add-upload-buffer-input-schema.json\",\n  \"title\": \"AddUploadBufferInput\",\n  \"description\": \"AddUploadBufferInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"DiskIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DiskIds\"\n        },\n        {\n          \"description\": \"An array of strings that identify disks that are to be configured as working storage. Each string has a minimum length of 1 and maximum length of 300. You can get the disk IDs from the <a>ListLocalDisks</a> API.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\",\n    \"DiskIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-add-upload-buffer-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: AddUploadBufferInput
---
