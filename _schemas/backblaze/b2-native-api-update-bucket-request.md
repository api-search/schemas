---
description: UpdateBucketRequest schema from Backblaze B2 Native API
layout: schema
name: UpdateBucketRequest
properties_list:
- description: The account ID
  name: accountId
  type: string
- description: The ID of the bucket to update
  name: bucketId
  type: string
- description: New privacy setting
  name: bucketType
  type: string
- description: New bucket info
  name: bucketInfo
  type: object
- description: New CORS rules
  name: corsRules
  type: array
- description: New lifecycle rules
  name: lifecycleRules
  type: array
- description: Only update if bucket revision matches this value
  name: ifRevisionIs
  type: integer
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-update-bucket-request-schema.json
slug: b2-native-api-update-bucket-request
source_filename: b2-native-api-update-bucket-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-update-bucket-request-schema.json\",\n  \"title\": \"UpdateBucketRequest\",\n  \"description\": \"UpdateBucketRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The account ID\",\n      \"example\": \"abc123def456\"\n    },\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the bucket to update\",\n      \"example\": \"e73ede9969c64355ef8b\"\n    },\n    \"bucketType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"allPublic\",\n        \"allPrivate\"\n      ],\n      \"description\": \"New privacy setting\"\n    },\n    \"bucketInfo\": {\n      \"type\": \"object\",\n      \"description\": \"New bucket info\"\n    },\n    \"corsRules\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"New CORS rules\"\n    },\n    \"lifecycleRules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"New lifecycle rules\"\n    },\n    \"ifRevisionIs\": {\n      \"type\": \"integer\",\n      \"description\": \"Only update if bucket revision matches this value\"\n    }\n  },\n  \"required\": [\n    \"accountId\",\n    \"bucketId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-update-bucket-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: UpdateBucketRequest
---
