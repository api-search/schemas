---
description: ListBucketsResponse schema from Backblaze B2 Native API
layout: schema
name: ListBucketsResponse
properties_list:
- description: ''
  name: buckets
  type: array
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-list-buckets-response-schema.json
slug: b2-native-api-list-buckets-response
source_filename: b2-native-api-list-buckets-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-buckets-response-schema.json\",\n  \"title\": \"ListBucketsResponse\",\n  \"description\": \"ListBucketsResponse schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"buckets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Bucket\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-list-buckets-response-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: ListBucketsResponse
---
