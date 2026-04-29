---
description: HideFileRequest schema from Backblaze B2 Native API
layout: schema
name: HideFileRequest
properties_list:
- description: The bucket containing the file
  name: bucketId
  type: string
- description: The name of the file to hide
  name: fileName
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-hide-file-request-schema.json
slug: b2-native-api-hide-file-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-hide-file-request-schema.json\",\n  \"title\": \"HideFileRequest\",\n  \"description\": \"HideFileRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"description\": \"The bucket containing the file\",\n      \"example\": \"e73ede9969c64355ef8b\"\n    },\n    \"fileName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the file to hide\",\n      \"example\": \"photos/image.jpg\"\n    }\n  },\n  \"required\": [\n    \"bucketId\",\n    \"fileName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-hide-file-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: HideFileRequest
---
