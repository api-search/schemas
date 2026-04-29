---
description: DeleteFileVersionRequest schema from Backblaze B2 Native API
layout: schema
name: DeleteFileVersionRequest
properties_list:
- description: The name of the file
  name: fileName
  type: string
- description: The ID of the file version to delete
  name: fileId
  type: string
- description: Set to true to bypass object lock governance mode
  name: bypassGovernance
  type: boolean
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-delete-file-version-request-schema.json
slug: b2-native-api-delete-file-version-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-delete-file-version-request-schema.json\",\n  \"title\": \"DeleteFileVersionRequest\",\n  \"description\": \"DeleteFileVersionRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the file\",\n      \"example\": \"photos/image.jpg\"\n    },\n    \"fileId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the file version to delete\",\n      \"example\": \"4_h4a48fe8875c6214145260818\"\n    },\n    \"bypassGovernance\": {\n      \"type\": \"boolean\",\n      \"description\": \"Set to true to bypass object lock governance mode\"\n    }\n  },\n  \"required\": [\n    \"fileName\",\n    \"fileId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-delete-file-version-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: DeleteFileVersionRequest
---
