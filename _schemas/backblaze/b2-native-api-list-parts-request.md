---
description: ListPartsRequest schema from Backblaze B2 Native API
layout: schema
name: ListPartsRequest
properties_list:
- description: ''
  name: fileId
  type: string
- description: Start listing from this part number
  name: startPartNumber
  type: integer
- description: Maximum number of parts to return
  name: maxPartCount
  type: integer
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-list-parts-request-schema.json
slug: b2-native-api-list-parts-request
source_filename: b2-native-api-list-parts-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-parts-request-schema.json\",\n  \"title\": \"ListPartsRequest\",\n  \"description\": \"ListPartsRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileId\": {\n      \"type\": \"string\",\n      \"example\": \"4_za71c4725f4f4a14a14a14a14a\"\n    },\n    \"startPartNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Start listing from this part number\"\n    },\n    \"maxPartCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of parts to return\"\n    }\n  },\n  \"required\": [\n    \"fileId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-parts-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: ListPartsRequest
---
