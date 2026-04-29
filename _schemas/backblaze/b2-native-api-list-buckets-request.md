---
description: ListBucketsRequest schema from Backblaze B2 Native API
layout: schema
name: ListBucketsRequest
properties_list:
- description: The account ID
  name: accountId
  type: string
- description: Filter to a specific bucket
  name: bucketId
  type: string
- description: Filter by bucket name
  name: bucketName
  type: string
- description: Filter by bucket type
  name: bucketTypes
  type: array
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-list-buckets-request-schema.json
slug: b2-native-api-list-buckets-request
source_filename: b2-native-api-list-buckets-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-buckets-request-schema.json\",\n  \"title\": \"ListBucketsRequest\",\n  \"description\": \"ListBucketsRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The account ID\",\n      \"example\": \"abc123def456\"\n    },\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"description\": \"Filter to a specific bucket\"\n    },\n    \"bucketName\": {\n      \"type\": \"string\",\n      \"description\": \"Filter by bucket name\"\n    },\n    \"bucketTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Filter by bucket type\"\n    }\n  },\n  \"required\": [\n    \"accountId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-buckets-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: ListBucketsRequest
---
