---
description: A list of buckets.
layout: schema
name: BucketList
properties_list:
- description: The kind of item this is.
  name: kind
  type: string
- description: The continuation token. Provide this value as the pageToken in a subsequent request to return the next page of results.
  name: nextPageToken
  type: string
- description: The list of buckets.
  name: items
  type: array
provider_name: Google Cloud Storage
provider_slug: gcp-cloud-storage
schema_file: json-schema/gcp-cloud-storage-json-bucket-list-schema.json
slug: gcp-cloud-storage-json-bucket-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BucketList\",\n  \"type\": \"object\",\n  \"description\": \"A list of buckets.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The kind of item this is.\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"The continuation token. Provide this value as the pageToken in a subsequent request to return the next page of results.\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"The list of buckets.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gcp-cloud-storage/refs/heads/main/json-schema/gcp-cloud-storage-json-bucket-list-schema.json
tags:
- Archival
- Backup
- Blob Storage
- Cloud Storage
- Data
- File Storage
- Google Cloud
- Object Storage
- Storage
title: BucketList
---
