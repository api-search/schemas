---
description: ListPartsResponse schema from Backblaze B2 Native API
layout: schema
name: ListPartsResponse
properties_list:
- description: ''
  name: parts
  type: array
- description: ''
  name: nextPartNumber
  type: integer
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-list-parts-response-schema.json
slug: b2-native-api-list-parts-response
source_filename: b2-native-api-list-parts-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-parts-response-schema.json\",\n  \"title\": \"ListPartsResponse\",\n  \"description\": \"ListPartsResponse schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"parts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"fileId\": {\n            \"type\": \"string\"\n          },\n          \"partNumber\": {\n            \"type\": \"integer\"\n          },\n          \"contentLength\": {\n            \"type\": \"integer\"\n          },\n          \"contentSha1\": {\n            \"type\": \"string\"\n          },\n          \"uploadTimestamp\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n    \"nextPartNumber\": {\n      \"type\": \"integer\",\n     \
  \ \"nullable\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-parts-response-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: ListPartsResponse
---
