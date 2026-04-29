---
description: ''
layout: schema
name: ChecksumAlgorithmList
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-checksumalgorithmlist-schema.json
slug: s3-checksumalgorithmlist
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChecksumAlgorithmList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"enum\": [\n      \"CRC32\",\n      \"CRC32C\",\n      \"SHA1\",\n      \"SHA256\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-checksumalgorithmlist-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ChecksumAlgorithmList
---
