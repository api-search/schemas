---
description: ListUnfinishedLargeFilesRequest schema from Backblaze B2 Native API
layout: schema
name: ListUnfinishedLargeFilesRequest
properties_list:
- description: ''
  name: bucketId
  type: string
- description: ''
  name: namePrefix
  type: string
- description: ''
  name: startFileId
  type: string
- description: ''
  name: maxFileCount
  type: integer
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-list-unfinished-large-files-request-schema.json
slug: b2-native-api-list-unfinished-large-files-request
source_filename: b2-native-api-list-unfinished-large-files-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-unfinished-large-files-request-schema.json\",\n  \"title\": \"ListUnfinishedLargeFilesRequest\",\n  \"description\": \"ListUnfinishedLargeFilesRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"example\": \"e73ede9969c64355ef8b\"\n    },\n    \"namePrefix\": {\n      \"type\": \"string\"\n    },\n    \"startFileId\": {\n      \"type\": \"string\"\n    },\n    \"maxFileCount\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"bucketId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-unfinished-large-files-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: ListUnfinishedLargeFilesRequest
---
