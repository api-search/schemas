---
description: Contains the bucket name, file format, bucket owner (optional), and prefix (optional) where inventory results are published.
layout: schema
name: InventoryS3BucketDestination
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: Bucket
  type: object
- description: ''
  name: Format
  type: object
- description: ''
  name: Prefix
  type: object
- description: ''
  name: Encryption
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-inventorys3bucketdestination-schema.json
slug: s3-inventorys3bucketdestination
source_filename: s3-inventorys3bucketdestination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InventoryS3BucketDestination\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {},\n    \"Bucket\": {},\n    \"Format\": {},\n    \"Prefix\": {},\n    \"Encryption\": {}\n  },\n  \"required\": [\n    \"Bucket\",\n    \"Format\"\n  ],\n  \"description\": \"Contains the bucket name, file format, bucket owner (optional), and prefix (optional) where inventory results are published.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-inventorys3bucketdestination-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: InventoryS3BucketDestination
---
