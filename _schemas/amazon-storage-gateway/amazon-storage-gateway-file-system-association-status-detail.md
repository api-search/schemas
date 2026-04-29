---
description: Detailed information on file system association status.
layout: schema
name: FileSystemAssociationStatusDetail
properties_list:
- description: ''
  name: ErrorCode
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-file-system-association-status-detail-schema.json
slug: amazon-storage-gateway-file-system-association-status-detail
source_filename: amazon-storage-gateway-file-system-association-status-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-file-system-association-status-detail-schema.json\",\n  \"title\": \"FileSystemAssociationStatusDetail\",\n  \"description\": \"Detailed information on file system association status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSystemAssociationSyncErrorCode\"\n        },\n        {\n          \"description\": \"The error code for a given file system association status.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-file-system-association-status-detail-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: FileSystemAssociationStatusDetail
---
