---
description: ''
layout: schema
name: ObjectVersionList
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-objectversionlist-schema.json
slug: s3-objectversionlist
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectVersionList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"ETag\": {},\n      \"ChecksumAlgorithm\": {},\n      \"Size\": {},\n      \"StorageClass\": {},\n      \"Key\": {},\n      \"VersionId\": {},\n      \"IsLatest\": {},\n      \"LastModified\": {},\n      \"Owner\": {}\n    },\n    \"description\": \"The version of an object.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-objectversionlist-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ObjectVersionList
---
