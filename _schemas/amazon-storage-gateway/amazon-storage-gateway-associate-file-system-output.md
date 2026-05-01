---
description: AssociateFileSystemOutput schema from Amazon Storage Gateway API
layout: schema
name: AssociateFileSystemOutput
properties_list:
- description: ''
  name: FileSystemAssociationARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-associate-file-system-output-schema.json
slug: amazon-storage-gateway-associate-file-system-output
source_filename: amazon-storage-gateway-associate-file-system-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-associate-file-system-output-schema.json\",\n  \"title\": \"AssociateFileSystemOutput\",\n  \"description\": \"AssociateFileSystemOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileSystemAssociationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSystemAssociationARN\"\n        },\n        {\n          \"description\": \"The ARN of the newly created file system association.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-associate-file-system-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: AssociateFileSystemOutput
---
