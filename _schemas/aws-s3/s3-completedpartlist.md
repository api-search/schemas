---
description: ''
layout: schema
name: CompletedPartList
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-completedpartlist-schema.json
slug: s3-completedpartlist
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompletedPartList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"ETag\": {},\n      \"ChecksumCRC32\": {},\n      \"ChecksumCRC32C\": {},\n      \"ChecksumSHA1\": {},\n      \"ChecksumSHA256\": {},\n      \"PartNumber\": {}\n    },\n    \"description\": \"Details of the parts that were uploaded.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-completedpartlist-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: CompletedPartList
---
