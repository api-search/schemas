---
description: ListFileVersionsRequest schema from Backblaze B2 Native API
layout: schema
name: ListFileVersionsRequest
properties_list:
- description: The bucket to list
  name: bucketId
  type: string
- description: ''
  name: startFileName
  type: string
- description: ''
  name: startFileId
  type: string
- description: ''
  name: maxFileCount
  type: integer
- description: ''
  name: prefix
  type: string
- description: ''
  name: delimiter
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-list-file-versions-request-schema.json
slug: b2-native-api-list-file-versions-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-file-versions-request-schema.json\",\n  \"title\": \"ListFileVersionsRequest\",\n  \"description\": \"ListFileVersionsRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"description\": \"The bucket to list\",\n      \"example\": \"e73ede9969c64355ef8b\"\n    },\n    \"startFileName\": {\n      \"type\": \"string\"\n    },\n    \"startFileId\": {\n      \"type\": \"string\"\n    },\n    \"maxFileCount\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"prefix\": {\n      \"type\": \"string\"\n    },\n    \"delimiter\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"bucketId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-file-versions-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: ListFileVersionsRequest
---
