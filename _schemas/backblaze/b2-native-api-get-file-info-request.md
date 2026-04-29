---
description: GetFileInfoRequest schema from Backblaze B2 Native API
layout: schema
name: GetFileInfoRequest
properties_list:
- description: The ID of the file
  name: fileId
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-get-file-info-request-schema.json
slug: b2-native-api-get-file-info-request
source_filename: b2-native-api-get-file-info-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-get-file-info-request-schema.json\",\n  \"title\": \"GetFileInfoRequest\",\n  \"description\": \"GetFileInfoRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the file\",\n      \"example\": \"4_h4a48fe8875c6214145260818\"\n    }\n  },\n  \"required\": [\n    \"fileId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-get-file-info-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: GetFileInfoRequest
---
