---
description: Information about a stored file
layout: schema
name: FileInfo
properties_list:
- description: The unique identifier for this version of this file
  name: fileId
  type: string
- description: The name of the file
  name: fileName
  type: string
- description: The account that owns the file
  name: accountId
  type: string
- description: The bucket that the file is in
  name: bucketId
  type: string
- description: The size of the file in bytes
  name: contentLength
  type: integer
- description: The SHA1 checksum of the bytes in the file
  name: contentSha1
  type: string
- description: The MIME type of the file
  name: contentType
  type: string
- description: Custom information about the file
  name: fileInfo
  type: object
- description: The action that created this file version
  name: action
  type: string
- description: Milliseconds since midnight, January 1, 1970 UTC
  name: uploadTimestamp
  type: integer
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-file-info-schema.json
slug: b2-native-api-file-info
source_filename: b2-native-api-file-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-file-info-schema.json\",\n  \"title\": \"FileInfo\",\n  \"description\": \"Information about a stored file\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for this version of this file\",\n      \"example\": \"4_h4a48fe8875c6214145260818\"\n    },\n    \"fileName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the file\",\n      \"example\": \"photos/image.jpg\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The account that owns the file\",\n      \"example\": \"abc123def456\"\n    },\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"description\": \"The bucket that the file is in\",\n      \"example\": \"e73ede9969c64355ef8b\"\n\
  \    },\n    \"contentLength\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the file in bytes\",\n      \"example\": 102400\n    },\n    \"contentSha1\": {\n      \"type\": \"string\",\n      \"description\": \"The SHA1 checksum of the bytes in the file\",\n      \"example\": \"a1b2c3d4e5f6a1b2c3d4e5f6a1b2c3d4e5f6a1b2\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The MIME type of the file\",\n      \"example\": \"image/jpeg\"\n    },\n    \"fileInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Custom information about the file\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"upload\",\n        \"hide\",\n        \"start\",\n        \"copy\"\n      ],\n      \"description\": \"The action that created this file version\",\n      \"example\": \"upload\"\n    },\n    \"uploadTimestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Milliseconds since midnight,\
  \ January 1, 1970 UTC\",\n      \"example\": 1660000000000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-file-info-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: FileInfo
---
