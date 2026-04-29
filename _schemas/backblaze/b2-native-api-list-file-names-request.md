---
description: ListFileNamesRequest schema from Backblaze B2 Native API
layout: schema
name: ListFileNamesRequest
properties_list:
- description: The bucket to list
  name: bucketId
  type: string
- description: Start listing from this file name
  name: startFileName
  type: string
- description: Maximum number of files to return (1-10000)
  name: maxFileCount
  type: integer
- description: Prefix to filter file names
  name: prefix
  type: string
- description: Delimiter used for virtual folder simulation
  name: delimiter
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-list-file-names-request-schema.json
slug: b2-native-api-list-file-names-request
source_filename: b2-native-api-list-file-names-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-file-names-request-schema.json\",\n  \"title\": \"ListFileNamesRequest\",\n  \"description\": \"ListFileNamesRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"description\": \"The bucket to list\",\n      \"example\": \"e73ede9969c64355ef8b\"\n    },\n    \"startFileName\": {\n      \"type\": \"string\",\n      \"description\": \"Start listing from this file name\"\n    },\n    \"maxFileCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of files to return (1-10000)\",\n      \"example\": 100\n    },\n    \"prefix\": {\n      \"type\": \"string\",\n      \"description\": \"Prefix to filter file names\"\n    },\n    \"delimiter\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Delimiter used for virtual folder simulation\"\n    }\n  },\n  \"required\": [\n    \"bucketId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-file-names-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: ListFileNamesRequest
---
