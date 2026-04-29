---
description: CreateKeyRequest schema from Backblaze B2 Native API
layout: schema
name: CreateKeyRequest
properties_list:
- description: ''
  name: accountId
  type: string
- description: List of capabilities for the key
  name: capabilities
  type: array
- description: A name for the key (letters, numbers, hyphens)
  name: keyName
  type: string
- description: Duration before key expires
  name: validDurationInSeconds
  type: integer
- description: Restrict key to this bucket
  name: bucketId
  type: string
- description: Restrict key to files with this prefix
  name: namePrefix
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-create-key-request-schema.json
slug: b2-native-api-create-key-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-create-key-request-schema.json\",\n  \"title\": \"CreateKeyRequest\",\n  \"description\": \"CreateKeyRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"example\": \"abc123def456\"\n    },\n    \"capabilities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of capabilities for the key\"\n    },\n    \"keyName\": {\n      \"type\": \"string\",\n      \"description\": \"A name for the key (letters, numbers, hyphens)\",\n      \"example\": \"my-app-key\"\n    },\n    \"validDurationInSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration before key expires\"\n    },\n    \"bucketId\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Restrict key to this bucket\"\n    },\n    \"namePrefix\": {\n      \"type\": \"string\",\n      \"description\": \"Restrict key to files with this prefix\"\n    }\n  },\n  \"required\": [\n    \"accountId\",\n    \"capabilities\",\n    \"keyName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-create-key-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: CreateKeyRequest
---
