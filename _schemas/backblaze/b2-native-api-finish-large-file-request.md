---
description: FinishLargeFileRequest schema from Backblaze B2 Native API
layout: schema
name: FinishLargeFileRequest
properties_list:
- description: The file ID from b2_start_large_file
  name: fileId
  type: string
- description: SHA1 checksums of each part in order
  name: partSha1Array
  type: array
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-finish-large-file-request-schema.json
slug: b2-native-api-finish-large-file-request
source_filename: b2-native-api-finish-large-file-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-finish-large-file-request-schema.json\",\n  \"title\": \"FinishLargeFileRequest\",\n  \"description\": \"FinishLargeFileRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileId\": {\n      \"type\": \"string\",\n      \"description\": \"The file ID from b2_start_large_file\",\n      \"example\": \"4_za71c4725f4f4a14a14a14a14a\"\n    },\n    \"partSha1Array\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"SHA1 checksums of each part in order\"\n    }\n  },\n  \"required\": [\n    \"fileId\",\n    \"partSha1Array\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-finish-large-file-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: FinishLargeFileRequest
---
