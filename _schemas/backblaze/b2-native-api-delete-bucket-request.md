---
description: DeleteBucketRequest schema from Backblaze B2 Native API
layout: schema
name: DeleteBucketRequest
properties_list:
- description: The account ID
  name: accountId
  type: string
- description: The ID of the bucket to delete
  name: bucketId
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-delete-bucket-request-schema.json
slug: b2-native-api-delete-bucket-request
source_filename: b2-native-api-delete-bucket-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-delete-bucket-request-schema.json\",\n  \"title\": \"DeleteBucketRequest\",\n  \"description\": \"DeleteBucketRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The account ID\",\n      \"example\": \"abc123def456\"\n    },\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the bucket to delete\",\n      \"example\": \"e73ede9969c64355ef8b\"\n    }\n  },\n  \"required\": [\n    \"accountId\",\n    \"bucketId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-delete-bucket-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: DeleteBucketRequest
---
