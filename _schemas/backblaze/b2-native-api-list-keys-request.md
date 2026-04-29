---
description: ListKeysRequest schema from Backblaze B2 Native API
layout: schema
name: ListKeysRequest
properties_list:
- description: ''
  name: accountId
  type: string
- description: Maximum number of keys to return
  name: maxKeyCount
  type: integer
- description: Start listing from this key ID
  name: startApplicationKeyId
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-list-keys-request-schema.json
slug: b2-native-api-list-keys-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-keys-request-schema.json\",\n  \"title\": \"ListKeysRequest\",\n  \"description\": \"ListKeysRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"example\": \"abc123def456\"\n    },\n    \"maxKeyCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of keys to return\"\n    },\n    \"startApplicationKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"Start listing from this key ID\"\n    }\n  },\n  \"required\": [\n    \"accountId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-keys-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: ListKeysRequest
---
