---
description: ''
layout: schema
name: Errors
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-errors-schema.json
slug: s3-errors
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Errors\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"Key\": {},\n      \"VersionId\": {},\n      \"Code\": {},\n      \"Message\": {}\n    },\n    \"description\": \"Container for all error elements.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-errors-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: Errors
---
