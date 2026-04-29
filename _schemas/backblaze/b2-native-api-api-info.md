---
description: API endpoint information
layout: schema
name: ApiInfo
properties_list:
- description: ''
  name: storageApi
  type: object
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-api-info-schema.json
slug: b2-native-api-api-info
source_filename: b2-native-api-api-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-api-info-schema.json\",\n  \"title\": \"ApiInfo\",\n  \"description\": \"API endpoint information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"storageApi\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"absoluteMinimumPartSize\": {\n          \"type\": \"integer\",\n          \"description\": \"Minimum part size in bytes for large files\",\n          \"example\": 5000000\n        },\n        \"recommendedPartSize\": {\n          \"type\": \"integer\",\n          \"description\": \"Recommended part size in bytes\",\n          \"example\": 100000000\n        },\n        \"apiUrl\": {\n          \"type\": \"string\",\n          \"description\": \"URL to use for subsequent API calls\",\n          \"example\": \"https://api005.backblazeb2.com\"\n        },\n        \"\
  downloadUrl\": {\n          \"type\": \"string\",\n          \"description\": \"URL to use for downloading files\",\n          \"example\": \"https://f005.backblazeb2.com\"\n        },\n        \"s3ApiUrl\": {\n          \"type\": \"string\",\n          \"description\": \"S3-compatible API URL\",\n          \"example\": \"https://s3.us-west-004.backblazeb2.com\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-api-info-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: ApiInfo
---
