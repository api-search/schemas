---
description: GetUploadPartUrlResponse schema from Backblaze B2 Native API
layout: schema
name: GetUploadPartUrlResponse
properties_list:
- description: ''
  name: fileId
  type: string
- description: ''
  name: uploadUrl
  type: string
- description: ''
  name: authorizationToken
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-get-upload-part-url-response-schema.json
slug: b2-native-api-get-upload-part-url-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-get-upload-part-url-response-schema.json\",\n  \"title\": \"GetUploadPartUrlResponse\",\n  \"description\": \"GetUploadPartUrlResponse schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileId\": {\n      \"type\": \"string\",\n      \"example\": \"4_za71c4725f4f4a14a14a14a14a\"\n    },\n    \"uploadUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://pod-000-1005-03.backblaze.com/b2api/v4/b2_upload_part\"\n    },\n    \"authorizationToken\": {\n      \"type\": \"string\",\n      \"example\": \"3_en0Y0j2f-0r0BVLS8vN9GJTWA-pLEP\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-get-upload-part-url-response-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: GetUploadPartUrlResponse
---
