---
description: UpdateFileSystemAssociationOutput schema from Amazon Storage Gateway API
layout: schema
name: UpdateFileSystemAssociationOutput
properties_list:
- description: ''
  name: FileSystemAssociationARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-update-file-system-association-output-schema.json
slug: amazon-storage-gateway-update-file-system-association-output
source_filename: amazon-storage-gateway-update-file-system-association-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-file-system-association-output-schema.json\",\n  \"title\": \"UpdateFileSystemAssociationOutput\",\n  \"description\": \"UpdateFileSystemAssociationOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileSystemAssociationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSystemAssociationARN\"\n        },\n        {\n          \"description\": \"The ARN of the updated file system association.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-file-system-association-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: UpdateFileSystemAssociationOutput
---
