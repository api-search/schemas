---
description: What the credentials allow
layout: schema
name: AllowedCapabilities
properties_list:
- description: A list of capabilities
  name: capabilities
  type: array
- description: Bucket ID restricted to, or null
  name: bucketId
  type: string
- description: Bucket name restricted to, or null
  name: bucketName
  type: string
- description: File name prefix restriction, or null
  name: namePrefix
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-allowed-capabilities-schema.json
slug: b2-native-api-allowed-capabilities
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-allowed-capabilities-schema.json\",\n  \"title\": \"AllowedCapabilities\",\n  \"description\": \"What the credentials allow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"capabilities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A list of capabilities\"\n    },\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Bucket ID restricted to, or null\"\n    },\n    \"bucketName\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Bucket name restricted to, or null\"\n    },\n    \"namePrefix\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"File name prefix restriction, or null\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-allowed-capabilities-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: AllowedCapabilities
---
