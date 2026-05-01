---
description: ''
layout: schema
name: Parts
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-parts-schema.json
slug: s3-parts
source_filename: s3-parts-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Parts\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"PartNumber\": {},\n      \"LastModified\": {},\n      \"ETag\": {},\n      \"Size\": {},\n      \"ChecksumCRC32\": {},\n      \"ChecksumCRC32C\": {},\n      \"ChecksumSHA1\": {},\n      \"ChecksumSHA256\": {}\n    },\n    \"description\": \"Container for elements related to a part.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-parts-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: Parts
---
