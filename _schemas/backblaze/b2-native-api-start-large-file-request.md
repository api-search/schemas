---
description: StartLargeFileRequest schema from Backblaze B2 Native API
layout: schema
name: StartLargeFileRequest
properties_list:
- description: ''
  name: bucketId
  type: string
- description: ''
  name: fileName
  type: string
- description: ''
  name: contentType
  type: string
- description: Custom file info
  name: fileInfo
  type: object
- description: Server side encryption settings
  name: serverSideEncryption
  type: object
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-start-large-file-request-schema.json
slug: b2-native-api-start-large-file-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-start-large-file-request-schema.json\",\n  \"title\": \"StartLargeFileRequest\",\n  \"description\": \"StartLargeFileRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"example\": \"e73ede9969c64355ef8b\"\n    },\n    \"fileName\": {\n      \"type\": \"string\",\n      \"example\": \"videos/large-video.mp4\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"example\": \"video/mp4\"\n    },\n    \"fileInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Custom file info\"\n    },\n    \"serverSideEncryption\": {\n      \"type\": \"object\",\n      \"description\": \"Server side encryption settings\"\n    }\n  },\n  \"required\": [\n    \"bucketId\",\n    \"fileName\"\
  ,\n    \"contentType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-start-large-file-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: StartLargeFileRequest
---
