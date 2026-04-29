---
description: ListUnfinishedLargeFilesResponse schema from Backblaze B2 Native API
layout: schema
name: ListUnfinishedLargeFilesResponse
properties_list:
- description: ''
  name: files
  type: array
- description: ''
  name: nextFileId
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-list-unfinished-large-files-response-schema.json
slug: b2-native-api-list-unfinished-large-files-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-unfinished-large-files-response-schema.json\",\n  \"title\": \"ListUnfinishedLargeFilesResponse\",\n  \"description\": \"ListUnfinishedLargeFilesResponse schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"files\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FileInfo\"\n      }\n    },\n    \"nextFileId\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-unfinished-large-files-response-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: ListUnfinishedLargeFilesResponse
---
