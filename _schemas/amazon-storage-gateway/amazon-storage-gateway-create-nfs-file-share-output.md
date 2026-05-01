---
description: CreateNFSFileShareOutput
layout: schema
name: CreateNFSFileShareOutput
properties_list:
- description: ''
  name: FileShareARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-create-nfs-file-share-output-schema.json
slug: amazon-storage-gateway-create-nfs-file-share-output
source_filename: amazon-storage-gateway-create-nfs-file-share-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-nfs-file-share-output-schema.json\",\n  \"title\": \"CreateNFSFileShareOutput\",\n  \"description\": \"CreateNFSFileShareOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileShareARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileShareARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the newly created file share.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-nfs-file-share-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: CreateNFSFileShareOutput
---
