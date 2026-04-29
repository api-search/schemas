---
description: GetUploadUrlRequest schema from Backblaze B2 Native API
layout: schema
name: GetUploadUrlRequest
properties_list:
- description: The ID of the bucket to upload to
  name: bucketId
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-get-upload-url-request-schema.json
slug: b2-native-api-get-upload-url-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-get-upload-url-request-schema.json\",\n  \"title\": \"GetUploadUrlRequest\",\n  \"description\": \"GetUploadUrlRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the bucket to upload to\",\n      \"example\": \"e73ede9969c64355ef8b\"\n    }\n  },\n  \"required\": [\n    \"bucketId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-get-upload-url-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: GetUploadUrlRequest
---
