---
description: CreateBucketRequest schema from Backblaze B2 Native API
layout: schema
name: CreateBucketRequest
properties_list:
- description: The account ID
  name: accountId
  type: string
- description: The name of the new bucket
  name: bucketName
  type: string
- description: Privacy setting for the bucket
  name: bucketType
  type: string
- description: User-defined info to store with the bucket
  name: bucketInfo
  type: object
- description: CORS rules for the bucket
  name: corsRules
  type: array
- description: Lifecycle rules for the bucket
  name: lifecycleRules
  type: array
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-create-bucket-request-schema.json
slug: b2-native-api-create-bucket-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-create-bucket-request-schema.json\",\n  \"title\": \"CreateBucketRequest\",\n  \"description\": \"CreateBucketRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The account ID\",\n      \"example\": \"abc123def456\"\n    },\n    \"bucketName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the new bucket\",\n      \"example\": \"my-media-bucket\"\n    },\n    \"bucketType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"allPublic\",\n        \"allPrivate\"\n      ],\n      \"description\": \"Privacy setting for the bucket\",\n      \"example\": \"allPrivate\"\n    },\n    \"bucketInfo\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"User-defined info to store with the bucket\"\n    },\n    \"corsRules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"CORS rules for the bucket\"\n    },\n    \"lifecycleRules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Lifecycle rules for the bucket\"\n    }\n  },\n  \"required\": [\n    \"accountId\",\n    \"bucketName\",\n    \"bucketType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-create-bucket-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: CreateBucketRequest
---
