---
description: Represents a B2 bucket
layout: schema
name: Bucket
properties_list:
- description: The account that owns the bucket
  name: accountId
  type: string
- description: The unique ID of the bucket
  name: bucketId
  type: string
- description: The unique name of the bucket
  name: bucketName
  type: string
- description: The bucket privacy setting
  name: bucketType
  type: string
- description: User-defined information stored with the bucket
  name: bucketInfo
  type: object
- description: CORS rules for the bucket
  name: corsRules
  type: array
- description: Lifecycle rules for the bucket
  name: lifecycleRules
  type: array
- description: The number of times the bucket info has been modified
  name: revision
  type: integer
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-bucket-schema.json
slug: b2-native-api-bucket
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-bucket-schema.json\",\n  \"title\": \"Bucket\",\n  \"description\": \"Represents a B2 bucket\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The account that owns the bucket\",\n      \"example\": \"abc123def456\"\n    },\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID of the bucket\",\n      \"example\": \"e73ede9969c64355ef8b\"\n    },\n    \"bucketName\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name of the bucket\",\n      \"example\": \"my-media-bucket\"\n    },\n    \"bucketType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"allPublic\",\n        \"allPrivate\",\n        \"snapshot\"\n      ],\n      \"description\": \"The bucket\
  \ privacy setting\",\n      \"example\": \"allPrivate\"\n    },\n    \"bucketInfo\": {\n      \"type\": \"object\",\n      \"description\": \"User-defined information stored with the bucket\"\n    },\n    \"corsRules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"CORS rules for the bucket\"\n    },\n    \"lifecycleRules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Lifecycle rules for the bucket\"\n    },\n    \"revision\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of times the bucket info has been modified\",\n      \"example\": 1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-bucket-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: Bucket
---
