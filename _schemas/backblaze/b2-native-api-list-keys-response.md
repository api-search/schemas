---
description: ListKeysResponse schema from Backblaze B2 Native API
layout: schema
name: ListKeysResponse
properties_list:
- description: ''
  name: keys
  type: array
- description: ''
  name: nextApplicationKeyId
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-list-keys-response-schema.json
slug: b2-native-api-list-keys-response
source_filename: b2-native-api-list-keys-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-keys-response-schema.json\",\n  \"title\": \"ListKeysResponse\",\n  \"description\": \"ListKeysResponse schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keys\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ApplicationKey\"\n      }\n    },\n    \"nextApplicationKeyId\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-keys-response-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: ListKeysResponse
---
