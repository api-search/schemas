---
description: Describes a file share. Only supported S3 File Gateway.
layout: schema
name: FileShareInfo
properties_list:
- description: ''
  name: FileShareType
  type: object
- description: ''
  name: FileShareARN
  type: object
- description: ''
  name: FileShareId
  type: object
- description: ''
  name: FileShareStatus
  type: object
- description: ''
  name: GatewayARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-file-share-info-schema.json
slug: amazon-storage-gateway-file-share-info
source_filename: amazon-storage-gateway-file-share-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-file-share-info-schema.json\",\n  \"title\": \"FileShareInfo\",\n  \"description\": \"Describes a file share. Only supported S3 File Gateway.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileShareType\": {\n      \"$ref\": \"#/components/schemas/FileShareType\"\n    },\n    \"FileShareARN\": {\n      \"$ref\": \"#/components/schemas/FileShareARN\"\n    },\n    \"FileShareId\": {\n      \"$ref\": \"#/components/schemas/FileShareId\"\n    },\n    \"FileShareStatus\": {\n      \"$ref\": \"#/components/schemas/FileShareStatus\"\n    },\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-file-share-info-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: FileShareInfo
---
