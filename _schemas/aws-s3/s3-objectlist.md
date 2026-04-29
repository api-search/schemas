---
description: ''
layout: schema
name: ObjectList
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-objectlist-schema.json
slug: s3-objectlist
source_filename: s3-objectlist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"Key\": {},\n      \"LastModified\": {},\n      \"ETag\": {},\n      \"ChecksumAlgorithm\": {},\n      \"Size\": {},\n      \"StorageClass\": {},\n      \"Owner\": {}\n    },\n    \"description\": \"An object consists of data and its descriptive metadata.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-objectlist-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ObjectList
---
