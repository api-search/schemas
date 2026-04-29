---
description: CopyFileRequest schema from Backblaze B2 Native API
layout: schema
name: CopyFileRequest
properties_list:
- description: The ID of the file to copy
  name: sourceFileId
  type: string
- description: The name for the new file
  name: fileName
  type: string
- description: Bucket ID to copy to (defaults to source bucket)
  name: destinationBucketId
  type: string
- description: Byte range to copy
  name: range
  type: string
- description: Whether to copy or replace metadata
  name: metadataDirective
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-copy-file-request-schema.json
slug: b2-native-api-copy-file-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-copy-file-request-schema.json\",\n  \"title\": \"CopyFileRequest\",\n  \"description\": \"CopyFileRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceFileId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the file to copy\",\n      \"example\": \"4_h4a48fe8875c6214145260818\"\n    },\n    \"fileName\": {\n      \"type\": \"string\",\n      \"description\": \"The name for the new file\",\n      \"example\": \"photos/image-copy.jpg\"\n    },\n    \"destinationBucketId\": {\n      \"type\": \"string\",\n      \"description\": \"Bucket ID to copy to (defaults to source bucket)\"\n    },\n    \"range\": {\n      \"type\": \"string\",\n      \"description\": \"Byte range to copy\"\n    },\n    \"metadataDirective\": {\n     \
  \ \"type\": \"string\",\n      \"enum\": [\n        \"COPY\",\n        \"REPLACE\"\n      ],\n      \"description\": \"Whether to copy or replace metadata\"\n    }\n  },\n  \"required\": [\n    \"sourceFileId\",\n    \"fileName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-copy-file-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: CopyFileRequest
---
