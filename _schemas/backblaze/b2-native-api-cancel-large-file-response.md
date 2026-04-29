---
description: CancelLargeFileResponse schema from Backblaze B2 Native API
layout: schema
name: CancelLargeFileResponse
properties_list:
- description: ''
  name: fileId
  type: string
- description: ''
  name: accountId
  type: string
- description: ''
  name: bucketId
  type: string
- description: ''
  name: fileName
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-cancel-large-file-response-schema.json
slug: b2-native-api-cancel-large-file-response
source_filename: b2-native-api-cancel-large-file-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-cancel-large-file-response-schema.json\",\n  \"title\": \"CancelLargeFileResponse\",\n  \"description\": \"CancelLargeFileResponse schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileId\": {\n      \"type\": \"string\",\n      \"example\": \"4_za71c4725f4f4a14a14a14a14a\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"example\": \"abc123def456\"\n    },\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"example\": \"e73ede9969c64355ef8b\"\n    },\n    \"fileName\": {\n      \"type\": \"string\",\n      \"example\": \"videos/large-video.mp4\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-cancel-large-file-response-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: CancelLargeFileResponse
---
