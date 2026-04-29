---
description: ListFileNamesResponse schema from Backblaze B2 Native API
layout: schema
name: ListFileNamesResponse
properties_list:
- description: ''
  name: files
  type: array
- description: Next file name for pagination
  name: nextFileName
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-list-file-names-response-schema.json
slug: b2-native-api-list-file-names-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-file-names-response-schema.json\",\n  \"title\": \"ListFileNamesResponse\",\n  \"description\": \"ListFileNamesResponse schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"files\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FileInfo\"\n      }\n    },\n    \"nextFileName\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Next file name for pagination\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-file-names-response-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: ListFileNamesResponse
---
