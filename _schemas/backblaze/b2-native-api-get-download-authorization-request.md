---
description: GetDownloadAuthorizationRequest schema from Backblaze B2 Native API
layout: schema
name: GetDownloadAuthorizationRequest
properties_list:
- description: Bucket to authorize downloads from
  name: bucketId
  type: string
- description: Files must have this name prefix
  name: fileNamePrefix
  type: string
- description: Duration (1 to 604800) the token is valid
  name: validDurationInSeconds
  type: integer
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-get-download-authorization-request-schema.json
slug: b2-native-api-get-download-authorization-request
source_filename: b2-native-api-get-download-authorization-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-get-download-authorization-request-schema.json\",\n  \"title\": \"GetDownloadAuthorizationRequest\",\n  \"description\": \"GetDownloadAuthorizationRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"description\": \"Bucket to authorize downloads from\",\n      \"example\": \"e73ede9969c64355ef8b\"\n    },\n    \"fileNamePrefix\": {\n      \"type\": \"string\",\n      \"description\": \"Files must have this name prefix\",\n      \"example\": \"photos/\"\n    },\n    \"validDurationInSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration (1 to 604800) the token is valid\",\n      \"example\": 3600\n    }\n  },\n  \"required\": [\n    \"bucketId\",\n    \"fileNamePrefix\",\n \
  \   \"validDurationInSeconds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-get-download-authorization-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: GetDownloadAuthorizationRequest
---
