---
description: CreateSMBFileShareOutput
layout: schema
name: CreateSMBFileShareOutput
properties_list:
- description: ''
  name: FileShareARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-create-smb-file-share-output-schema.json
slug: amazon-storage-gateway-create-smb-file-share-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-smb-file-share-output-schema.json\",\n  \"title\": \"CreateSMBFileShareOutput\",\n  \"description\": \"CreateSMBFileShareOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileShareARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileShareARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the newly created file share.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-smb-file-share-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: CreateSMBFileShareOutput
---
