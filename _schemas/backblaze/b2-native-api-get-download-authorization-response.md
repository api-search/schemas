---
description: GetDownloadAuthorizationResponse schema from Backblaze B2 Native API
layout: schema
name: GetDownloadAuthorizationResponse
properties_list:
- description: ''
  name: bucketId
  type: string
- description: ''
  name: fileNamePrefix
  type: string
- description: ''
  name: authorizationToken
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-get-download-authorization-response-schema.json
slug: b2-native-api-get-download-authorization-response
source_filename: b2-native-api-get-download-authorization-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-get-download-authorization-response-schema.json\",\n  \"title\": \"GetDownloadAuthorizationResponse\",\n  \"description\": \"GetDownloadAuthorizationResponse schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"example\": \"e73ede9969c64355ef8b\"\n    },\n    \"fileNamePrefix\": {\n      \"type\": \"string\",\n      \"example\": \"photos/\"\n    },\n    \"authorizationToken\": {\n      \"type\": \"string\",\n      \"example\": \"3_en0Y0j2f-0r0BVLS8vN9GJTWA-pLEP\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-get-download-authorization-response-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: GetDownloadAuthorizationResponse
---
